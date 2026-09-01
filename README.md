# timseo-seo

> Système SEO complet basé sur la doctrine publique de [@Timseo_](https://x.com/Timseo_)
> AI-first (Claude + Obsidian + RAG), 0 outils SEO payants, 20 €/mois de coût total.

## 📚 Contenu du repo

```
timseo-seo/
├── README.md                       # Ce fichier
├── timseo_corpus_rapport.md        # Base de connaissances exhaustive (10 sections, 100+ posts)
├── skill/
│   └── SKILL.md                    # Skill Hermes prêt à déployer (~/.hermes/skills/timseo-seo/)
├── references/
│   └── checklist-deploiement.md    # Checklist courte copiable dans ton vault
└── examples/
    └── AGENTS.md                   # Template AGENTS.md pour vault Obsidian (structure Karpathy)
```

## 🎯 Philosophie (résumé)

**Le SEO en 2026 = un système d'orchestration IA + data propriétaire, pas un empilement d'outils.**

- **5 requêtes stratégiques business > 100 mots-clés** génériques
- **Topical authority** sur une verticale gagnable (ex : « balle de golf d'occasion » → top 1 « balle de golf »)
- **Data propriétaire = seul moat** : appels clients, SAV, avis, comparaisons faites-maison
- **Signaux sociaux (Reddit, LinkedIn, YouTube) > backlinks**
- **Outils SEO classiques = data généraliste quasi obsolète** — sauf GSC + Google Keyword Planner
- **Le SEO technique reste important MAIS délégable à 100 % à l'IA** (Claude + Obsidian)
- **GEO/AEO = ~3 % du trafic aujourd'hui** mais signal structurel fort → investir maintenant

## ⚙️ Stack technique (20 €/mois)

| Composant | Rôle | Coût |
|-----------|------|------|
| **Claude Code** | LLM principal | 20 €/mois |
| **Obsidian** | Vault Karpathy `raw/` + `wiki/` | Gratuit |
| **ChromaDB** + **Sentence-Transformers** | RAG local | Gratuit |
| **Google Search Console** | Données réelles positions/indexation | Gratuit |
| **Google Keyword Planner** | CPC + volume | Gratuit (compte Google Ads) |
| **Resend** | Email transactionnel (100/jour gratuit) | Gratuit |
| **Lighthouse** (local) | Core Web Vitals mobile-first | Gratuit |

**Outils SEO payants STOP** : Semrush, Ahrefs, Majestic, Screaming Frog, etc.

## 🚀 Quick start

### 1. Déployer le skill dans Hermes

```bash
# Copier le skill dans ton dossier Hermes
mkdir -p ~/.hermes/skills/timseo-seo/{references,templates}
cp skill/SKILL.md ~/.hermes/skills/timseo-seo/SKILL.md
cp references/checklist-deploiement.md ~/.hermes/skills/timseo-seo/references/
cp examples/AGENTS.md ~/.hermes/skills/timseo-seo/templates/

# Le skill est auto-chargé par Hermes à la prochaine session
```

### 2. Setup du vault Obsidian (Karpathy)

```bash
mkdir -p vault/{raw,wiki}
cp examples/AGENTS.md vault/AGENTS.md
# Adapter les instructions à ton contexte client
```

### 3. Lancer la stack

```bash
# ChromaDB (RAG)
docker run -d -p 8000:8000 chromadb/chroma

# Embeddings locaux
pip install sentence-transformers
```

## 📋 10 workflows (W0-W10)

| ID | Workflow | Description |
|----|----------|-------------|
| W0 | Setup système | Vault + RAG + 27 automatisations (30 min) |
| W1 | Recherche mots-clés | 5 sources, 3-5 KW business, 10 micro-intentions (2-4h) |
| W2 | Architecture & silos | Univers sémantique + clusters AEO + pSEO sans spam |
| W3 | Maillage interne | Délégué 100% à Claude (62 liens / 30 min) |
| W4 | Cannibalisation | Export GSC 90j complet → 301 obligatoire (jamais 410) |
| W5 | Technique base | 19 points checklist (rendu, sitemap, JSON-LD, perf) |
| W6 | Core Web Vitals | Lighthouse mobile → corrections Claude |
| W7 | Citabilité LLM (GEO) | 7 scores + 2 preuves atomiques / 100 mots |
| W8 | Signaux sociaux | Top 6 plateformes + strat mots-clés compétitifs |
| W9 | Audit complet 7 phases | Site/serp → quick wins → cannibalisation → maillage → plan 90j |
| W10 | Lancement site 15 min | Claude + Resend + indexation GSC |

## 🛑 Garde-fous (NEVER do)

- ❌ Acheter des backlinks
- ❌ Payer 400 €/mois pour un site vitrine + email
- ❌ Suivre trafic / volume / position moyenne / nb BL comme KPIs
- ❌ Automatiser son SEO **avant d'avoir ranké au moins un site**
- ❌ Croire que Claude seul remplace un consultant SEO
- ❌ Publier un article de blog sur une requête dominée par AI Overviews (9/10)
- ❌ Faire du 410 sur page cannibalisée — **toujours 301**
- ❌ Produire « pour produire » sous prétexte d'IA
- ❌ Site SPA pure sans prerender (non crawlable)
- ❌ JSON-LD qui ne correspond pas au contenu visible

## 📊 KPIs à suivre (business-first)

**✅ NOUVEAUX :**
- Proximité de l'offre
- Intention d'achat (Do vs Know)
- CPC
- Faisabilité de ranking
- Capacité à récupérer un email (lead magnet intégré)
- Score RRF (Reciprocal Rank Fusion)

**❌ ANCIENS (vanité) :**
- Trafic brut
- Volume de recherche
- Nombre de backlinks
- Position moyenne

## 📖 Sources

- **100+ publications de @Timseo_** (juin 2025 → août 2026)
- Index complet des posts dans `timseo_corpus_rapport.md` §9
- Compte X public : https://x.com/Timseo_

## 🛠 Maintenance

- **Mise à jour doctrine** : relancer l'analyse @Timseo_ tous les 3-6 mois
- **Versioning** : incrémenter `version` dans `SKILL.md` à chaque modification majeure
- **Skills Hermes** : ce repo est la source de vérité, déploier via `cp -r skill/ ~/.hermes/skills/timseo-seo/`

## 📄 License

MIT — Tu peux librement réutiliser, modifier, distribuer. Crédits : [@Timseo_](https://x.com/Timseo_) pour la doctrine, Octo pour la curation.

---

*Compilé le 1er septembre 2026 par Octo pour Teeflo. Basé sur 100+ publications de @Timseo_ couvrant juin 2025 → août 2026.*
