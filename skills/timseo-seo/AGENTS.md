# AGENTS.md — Template pour vault Obsidian (structure Karpathy)

> Place ce fichier à la racine de ton vault Obsidian : `vault/AGENTS.md`
> Il guide l'IA (Claude Code) sur comment interagir avec ton système SEO.

---

## Instructions pour l'IA (Claude Code)

### Structure du vault (Karpathy)
```
vault/
├── raw/                    # LECTURE SEULE - sources brutes
│   ├── gsc-exports/       # Exports GSC complets (90j)
│   ├── client-calls/      # Transcripts appels clients
│   ├── reddit-threads/    # Threads Reddit pertinents
│   ├── competitor-pages/  # Pages concurrents (HTML/markdown)
│   └── support-tickets/   # Tickets SAV, emails clients
├── wiki/                   # DOMAINE AGENT - lecture/écriture
│   ├── mots-cles/
│   ├── architecture/
│   ├── contenu/
│   ├── geo/
│   ├── signaux-sociaux/
│   ├── veille/
│   ├── audits/
│   ├── cannibalisation/
│   └── systeme/
└── .chroma/               # ChromaDB local (RAG) - ne pas toucher
```

### Règles absolues
1. **Écris UNIQUEMENT dans `vault/wiki/`** — `raw/` est en lecture seule
2. **Utilise des wikilinks `[[concept]]` partout** — pas de liens markdown classiques
3. **Un fichier = un concept atomique** — pas de fichiers fourre-tout
4. **Recharge les 281 faits mémoire** à chaque ouverture de session (`wiki/systeme/281-faits-memoire.md`)
5. **Respecte les 66 procédures** documentées dans `wiki/systeme/66-procedures.md`

### Workflow standard
```
Input utilisateur → Lecture wiki/raw pertinent → Application procédure → Écriture wiki/ → Mise à jour RAG (./kb rebuild) → Réponse
```

### Commandes disponibles
- `./kb rebuild` — Rebuild incrémental index ChromaDB
- `./kb search "requête"` — Recherche sémantique dans le vault
- `./kb stats` — Stats vault (nb notes, taille, dernière MAJ)

### Format des notes (standard)
```markdown
---
concept: nom-du-concept
tags: [tag1, tag2]
source: [post-timseo|client|test-propre]
date: 2026-XX-XX
confiance: [haute|moyenne|basse]
---

# [[nom-du-concept]]

Contenu atomique, actionnable, avec exemples concrets.

## Liens sortants
- [[concept-lié-1]]
- [[concept-lié-2]]

## Références sources
- [@Timseo_ status/XXXX](https://x.com/Timseo_/status/XXXX)
- [Rapport complet](../timseo_corpus_rapport.md#section)
```

### Procédures SEO clés (référence rapide)
| Procédure | Fichier wiki | Description |
|-----------|--------------|-------------|
| W1 Recherche KW | `mots-cles/recherche-mots-cles.md` | 5 sources, 3-5 KW business |
| W2 Architecture | `architecture/cluster-aeo.md` | Silos sémantiques orientés réponses |
| W3 Maillage | `architecture/maillage-systeme.md` | Délégué à Claude |
| W4 Cannibalisation | `cannibalisation/plan-action-<date>.md` | Export GSC 90j, 301 obligatoire |
| W5 Technique | `systeme/checklist-technique.md` | 19 points base |
| W6 CWV | `systeme/audit-cwv.md` | Lighthouse mobile + corrections Claude |
| W7 Citabilité LLM | `geo/geo-audit.md` | 7 scores + preuves atomiques |
| W8 Signaux sociaux | `signaux-sociaux/reddit-cockpit.md` | Top 6 plateformes |
| W9 Audit complet | `audits/audit-<client>-<date>.md` | 7 phases |
| W10 Lancement 15min | `systeme/lancement-rapide.md` | Site full Claude |

### Prompts Claude intégrés (à copier-coller)
Voir `wiki/systeme/prompts-claude.md` pour la bibliothèque complète.

---

## Faits mémoire permanents (exemples)
> Ces 281 faits sont rechargés à chaque session. Format : `fait: description | confiance | source`

- `kw-volume-irrelevant: Le volume de recherche n'est plus un KPI pertinent — c'est la proximité de l'offre qui compte | haute | @Timseo_ 2086703171657932977`
- `bl-unnecessary: Les backlinks ne sont pas nécessaires pour ranker — signaux sociaux suffisent | haute | @Timseo_ 2094097061012541844`
- `cannib-301-only: Sur cannibalisation, toujours 301 vers page gardée, jamais 410 | haute | @Timseo_ 2089743876244529215`
- `geo-3percent: GEO = ~3% du trafic currently mais signal structurel fort | moyenne | @Timseo_ 2070043197590688233`
- `claude-not-consultant: Claude seul ne remplace pas un consultant SEO — il faut skills + workflows + data proprio | haute | @Timseo_ 2093359702167990783`

---

*Template généré depuis skill `timseo-seo` v1.0.0 — adapter à ton contexte client/projet.*