---
name: timseo-seo
description: "SEO system based on Timseo_'s doctrine: AI-first (Claude + Obsidian + RAG), proprietary data moats, 5 strategic queries > 100 keywords, topical authority, social signals over backlinks, GEO/AEO readiness. No paid SEO tools."
version: 1.0.0
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [seo, timseo, claude, obsidian, rag, geo, aeo, keywords, cannibalization, internal-linking, core-web-vitals, structured-data, topical-authority]
    related_skills: [holographic-memory, software-development/plan, software-development/debugging, creative/architecture-diagram]
---

# Timseo_ SEO System

> **Source**: Compte X [@Timseo_](https://x.com/Timseo_) — analyse exhaustive juin 2025 → août 2026 (voir rapport complet `/home/teeflo/timseo_corpus_rapport.md`)
> **Philosophie**: « Vous n'avez plus besoin d'outil, mais d'un système SEO » — 66 procédures, 1528 notes RAG, 281 faits mémoire, 27 automatisations. Coût : 20 €/mois (Claude Code).

---

## CRITICAL RULES

**NEVER do these (Timseo_ « scams »):**
- ❌ Acheter des backlinks — « mythe SEO, remplacés par signaux sociaux »
- ❌ Payer 400 €/mois pour un site vitrine + email — faire en 15 min avec Claude + Resend
- ❌ Suivre le volume de mots-clés / trafic / position moyenne / nb backlinks comme KPI
- ❌ Automatiser son SEO **avant d'avoir ranké au moins un site**
- ❌ Croire que **Claude seul** remplace un consultant SEO
- ❌ Publier un article de blog sur une requête dominée par AI Overviews (9/10 = skip)
- ❌ Faire du 410 sur page cannibalisée — **toujours 301** pour préserver les liens
- ❌ Produire « pour produire » sous prétexte d'IA
- ❌ Site SPA pure sans prerender (non crawlable)
- ❌ JSON-LD qui ne correspond pas au contenu visible

**ALWAYS do these:**
- ✅ 5 requêtes stratégiques business > 100 mots-clés génériques
- ✅ Cibler intentions **Do** (calculer, comparer, acheter, démo) pas **Know** (lire)
- ✅ Data propriétaire = seul moat (appels clients, SAV, avis, comparaisons faites-maison)
- ✅ Topical authority sur une verticale gagnable (ex: « balle de golf d'occasion » → top 1 « balle de golf »)
- ✅ Signaux sociaux (Reddit, LinkedIn, YouTube) > backlinks
- ✅ Système : Claude Code + Obsidian (Karpathy raw/wiki) + RAG ChromaDB + AGENTS.md + wikilinks
- ✅ Audit mensuel indexation + cannibalisation + maillage délégués à Claude

---

## CORE WORKFLOWS

### W0 — Setup du système SEO (prérequis non négociable)

> « L'erreur est d'utiliser Claude tout seul. Le bon setup c'est Claude + Obsidian + skills + un workflow séquencé. »

```bash
# 1. Obsidian vault structure (Karpathy)
mkdir -p vault/{raw,wiki}
# raw/ = lecture seule (sources brutes)
# wiki/ = domaine agent (notes réécrites, wikilinks partout)

# 2. AGENTS.md à la racine du vault
cat > vault/AGENTS.md << 'EOF'
# Instructions pour l'IA
- Lis/écris dans vault/wiki/ uniquement
- Utilise des wikilinks [[concept]] partout
- Respecte la structure Karpathy raw/wiki
- Recharge les 281 faits mémoire à chaque session
EOF

# 3. RAG local (ChromaDB + Sentence-Transformers)
# docker run -d -p 8000:8000 chromadb/chroma
# pip install sentence-transformers

# 4. CLI ./kb + ./kb rebuild (rebuild incrémental)
# Voir rapport §4.1 pour le code complet
```

**Checklist setup :**
- [ ] Vault Obsidian créé avec structure `raw/` + `wiki/`
- [ ] `AGENTS.md` à la racine avec instructions claires
- [ ] RAG ChromaDB opérationnel (port 8000)
- [ ] Embeddings `sentence-transformers/all-MiniLM-L6-v2` ou équivalent
- [ ] `./kb rebuild` fonctionnel (incrémental)
- [ ] 27 automatisations configurées (voir § Automatisations)

---

### W1 — Recherche de mots-clés « sans outil payant »

> Workflow 5 sources : GKP + Reddit + Grok + Data proprio + GSC

```bash
# Étapes séquentielles (pas parallèles)
# 1. Contexte client → data propriétaire dans Obsidian
# 2. Signaux sociaux Reddit/X → vraies questions/objections
# 3. Grok DeepSearch → signaux utilisateurs émergents
# 4. Google Keyword Planner → CPC + volume (seuls indicateurs fiables)
# 5. GSC via Qadence/agent → quick wins + cannibalisation
# 6. Lancer workflow recherche sous Claude
```

**Sorties attendues dans `wiki/mots-cles/` :**
- `mots-cles-decisionnels.md` — 3 à 5 requêtes business + 10 micro-intentions chacune
- `mots-cles-overview.md` — requêtes déclenchant AI Overviews (traiter différemment)
- `mots-cles-resistants-ia.md` — requêtes où l'IA ne peut pas répondre seule
- `peurs-objections.md` — 10 objections par mot-clé business (générées par Claude)

**Prompt clé pour Claude :**
```
Pour chaque mot-clé business, génère 10 micro-intentions format :
- Intention : [Do/Know]
- Requête longue traîne (24 mots avg)
- Objection/peur utilisateur
- Format de page recommandé (comparatif / calculateur / cas d'usage / directory)
```

---

### W2 — Architecture de contenu & Silos sémantiques

> Chaîne : mot-clé business → longue traîne → vecteurs sémantiques → micro-intentions → univers sémantique

**Arborescence cible (`wiki/architecture/`) :**
```
cluster-aeo/          # groupement thématique orienté réponses (vs cocon classique)
modeles-pseo/         # templates réutilisables pSEO sans spam
programmatique-pseo/  # 1 template = 1 variable = centaines de pages
maillage-systeme/     # maillage interne délégué à Claude
roadmap-pseo/         # enchaînement programmation → production → publication
```

**Types de pages à produire par requête stratégique (1-15 pages) :**
- [ ] Cas d'usage concrets
- [ ] Comparatifs (Alternatives à X / Gratuite / Française)
- [ ] Réponses aux objections (FAQ ultra-complètes depuis Reddit/X)
- [ ] Contenus d'expertise (data propriétaire)
- [ ] Directories (prix, tendances, comparatifs solutions)
- [ ] Pages statistiques / calculateurs / simulateurs (lead magnet)

**Règle pSEO « sans spam » :** 1 template + 1 variable + data propriétaire = qualité. Pas de génération de masse sans données uniques.

---

### W3 — Maillage interne (délégué 100% à Claude)

> « 62 liens en 30 minutes » — avec ou sans export GSC

```bash
# Input : crawl complet ou export GSC (requêtes + pages + positions)
# Process : Claude lit tout → propose maillage
# Output : liste de liens (source → cible + ancre + contexte)
# Bonus : mapping visuel via GitHub détourné (voir rapport §4.6)
```

**Skill dédié** : `maillage-systeme` (dans arborescence agent)

---

### W4 — Détection & résolution cannibalisation

> Export GSC 90 jours ENTIER (≈ 1M tokens, pas d'échantillon)

```bash
# Workflow strict (rapport §4.5)
1. Lire export GSC 90j complet
2. Isoler requêtes déclenchant 2+ URLs
3. Classer conflit : mot-clé exact / même intention / proximité sémantique
4. Comparer : position, impressions, clics, CTR des 2 pages
5. Décider action :
   - 301 vers page gardée (TOUJOURS, jamais 410)
   - Fusion contenu
   - Séparation micro-intentions (écrire 2 angles distincts)
   - AUCUNE action si les 2 pages en top 10
```

**Sortie** : `wiki/cannibalisation/plan-action-<date>.md` avec décisions tracées.

---

### W5 — SEO Technique (checklist base à copier-coller)

> « Le SEO technique reste ultra important, SAUF QUE : délégable à 100% à l'IA »

**Checklist obligatoire pour tout site codé avec Claude** (rapport §3.5, post [2087203754324242918](https://x.com/Timseo_/status/2087203754324242918)) :

**Rendu & Crawlabilité :**
- [ ] Pas de SPA pure — 3 options : prerender post-build (`vite build` + `scripts/prerender.mjs`) OU framework SSR/SSG (Next/Astro/Remix) OU prerender headless (Puppeteer/Playwright)
- [ ] Chaque route publique = son propre HTML avec `<title>`, `<meta description>`, `<link rel="canonical">` dans le HTML brut (pas après hydratation JS)

**Fichiers racine :**
- [ ] `sitemap.xml` auto-généré depuis les routes
- [ ] `robots.txt` pointant vers le sitemap
- [ ] Vrai `404.html` retournant un 404 HTTP

**Par page :**
- [ ] `<title>` + `<meta description>` uniques
- [ ] Un seul `<h1>` par page
- [ ] Hiérarchie h2/h3 cohérente
- [ ] Canonical explicite par route
- [ ] Open Graph + Twitter Card complets

**JSON-LD (via Claude, Schema.org) :**
- [ ] `Organization` + `WebSite` sur home
- [ ] `Article` sur posts blog
- [ ] `FAQPage` **seulement si** FAQ visible sur la page
- [ ] **Règle d'or** : jamais de schéma sans contenu visible correspondant

**Performance (mobile-first) :**
- [ ] Lazy-load images avec `width`/`height` explicites
- [ ] `font-display: swap` sur toutes les polices
- [ ] Lighthouse mobile pour Core Web Vitals (LCP, INP, CLS)

---

### W6 — Audit Core Web Vitals (via Claude)

> Processus [2077366949785595919](https://x.com/Timseo_/status/2077366949785595919)

```bash
1. Récupérer sitemap.xml
2. Lancer Lighthouse en LOCAL, MOBILE (mobile-first)
3. Mesurer Core Web Vitals sur échantillon représentatif
4. Claude liste problèmes techniques + corrections
5. Claude CORRIGE le code
6. Sortir TOP 5 pires pages + plan d'action priorisé
```

---

### W7 — Audit sémantique & Score citabilité LLM (GEO/AEO)

> « Pour le moment c'est 3% du trafic le GEO » — mais Google l'intègre dans GSC, signal structurel fort.

**Audit sémantique** [2080348718839066635](https://x.com/Timseo_/status/2080348718839066635) :
```
1. Lister entités sémantiques attendues par Google sur la requête
2. Vérifier lexique sémantique autour du mot-clé
3. Identifier micro-intentions (pour score RRF)
4. Ajouter Information Gain (données uniques, pas dans le top 10)
5. Scorer contenu sur 100
6. Corriger Title/meta/Hn
```

**Score citabilité LLM** (7 dimensions sur 100) [2091926256581587093](https://x.com/Timseo_/status/2091926256581587093) :
| Dimension | Seuil / Règle |
|-----------|---------------|
| Surprise | Info non générique, contre-intuitive |
| Grounding | Sources citées, vérifiables |
| Content Effort | Preuve d'effort éditorial |
| Alignement RRF | Micro-intentions couvertes |
| RAG Structurer | Structure retriever-friendly |
| Freshness Guard | Date maj visible, contenu à jour |
| Atomic Proofs | **≥ 2 triplets [sujet][relation][valeur chiffrée] / 100 mots** |

**Règle critique retriever** : la réponse doit arriver **dans les 30 mots après chaque H2**.

**Workflow itératif** : lire texte entier + requête cible + type page → noter 7 scores → citer phrases exactes problèmes → réécrire en attaquant les 2 scores les plus bas.

---

### W8 — Signaux sociaux (le « nouveau link building »)

> Top 6 plateformes externes : YouTube #1, Reddit #2, LinkedIn #3, X #4, Substack #5, Pinterest #6

**Stratégie mots-clés compétitifs** [2082113849705345533](https://x.com/Timseo_/status/2082113849705345533) :
```bash
1. Choisir mot-clé où ton site n'a AUCUNE chance de ranker
2. Publier post/vidéo OPTIMISÉ sur ce mot-clé sur LinkedIn (ou YouTube)
3. Générer engagement maximal (commentaires, partages, temps lecture)
4. Tester, itérer, répéter — JAMAIS spammer
```

**Stratégie « Extension Chrome = SEO »** [2079149819046863023](https://x.com/Timseo_/status/2079149819046863023) :
```bash
# Chaque fonctionnalité SaaS = 1 extension Chrome
# 1 extension = 1 point d'entrée SEO indépendant
# Résultat : 35 utilisateurs + 1 avis en 14 jours (premier test)
```

**Canaux à maintenir :**
- [ ] YouTube : contenu long, evergreen, démonstration produit
- [ ] Reddit : veille questions réelles, FAQ, engagement authentique
- [ ] LinkedIn : posts optimisés mots-clés, cas clients, thought leadership
- [ ] X : fils courts, veille, communauté
- [ ] Substack : newsletter longue (4 ans, 5k abonnés, jamais monétisé = meilleur canal acquisition)
- [ ] Pinterest : visuels data, infographies

---

### W9 — Audit SEO complet (7 phases, 50+ audits faits pour 20 €/mois)

> [2088333331729350694](https://x.com/Timseo_/status/2088333331729350694)

```bash
Phase 0 → Audit site/SERP (crawl + analyse top 10)
Phase 1 → Quick wins (indexation, CTR, positions 4-10)
Phase 2 → Cannibalisation (export GSC 90j complet)
Phase 3 → Clusters AEO (groupement orienté réponses)
Phase 4 → Vecteurs sémantiques (entités + lexique + micro-intentions)
Phase 5 → Maillage interne (délégué à Claude)
Phase 6 → Briefs contenu (structure + ton de voix + data proprio)
Phase 7 → Plan d'action 90 jours (priorisé par impact business)
```

**Livrable** : `wiki/audits/audit-<client>-<date>.md` avec toutes les phases documentées.

---

### W10 — Lancement site SEO en 15 min (MVP)

> [2082488568723976344](https://x.com/Timseo_/status/2082488568723976344) ; [2082742743613288874](https://x.com/Timseo_/status/2082742743613288874)

```bash
1. Claude génère v1 HTML complet (pas de CMS)
2. Itérer section par section (JAMAIS page entière d'un coup)
3. Indexer sur Google Search Console
4. Email pro sur Resend (100 emails/jour gratuits)
5. Déployer (Netlify/Vercel/Cloudflare Pages)
```

**Exemples sites full Claude** : `fusionn.co`, `qadence.io`, `seocity.app`

---

## AUTOMATISATIONS (27 configurées)

> « Une automatisation vérifie chaque lundi que les 26 autres tournent encore » [2088292563153551525](https://x.com/Timseo_/status/2088292563153551525)

| # | Automatisation | Fréquence | Stack |
|---|----------------|-----------|-------|
| 1 | Revue de presse SEO quotidienne | Quotidien | Claude + RSS + Obsidian |
| 2 | Audit indexation (404, sitemap, vérif Google) | Hebdo | Claude + GSC API |
| 3 | Relevé citations IA (ChatGPT, Perplexity, Gemini, etc.) | Hebdo | Custom script |
| 4 | Connexion GSC → positions + indexation | Quotidien | Qadence / GSC API |
| 5 | Vérification santé 26 autres scripts | Lundi | Cron + healthcheck |
| 6 | Reddit Cockpit (questions + signaux) | Quotidien | Reddit API + Claude |
| 7 | LinkedIn Journal (posts + engagement) | Quotidien | LinkedIn API |
| 8 | X Reply Cockpit (réponses + veille) | Quotidien | X API |
| 9 | Brèves IA 2×/jour | 2×/jour | RSS + Claude |
| 10 | Newsletter IA hebdo | Hebdo | Substack API |
| 11-27 | ... (autres automatisations techniques) | Variables | Claude + scripts |

**Stack d'automatisation** : `launchd` (macOS cron) + scripts Python/Node + APIs officielles. Pas de n8n / Make / Zapier.

---

## KPIs — Ce qu'on suit vs Ce qu'on ignore

> [2086703171657932977](https://x.com/Timseo_/status/2086703171657932977) ; [2086053157982126505](https://x.com/Timseo_/status/2086053157982126505)

**✅ NOUVEAUX KPIs (business-first) :**
- [ ] Proximité de l'offre (match entre requête et ce qu'on vend)
- [ ] Intention d'achat (Do vs Know)
- [ ] CPC (proxy valeur commerciale)
- [ ] Faisabilité de ranking (difficulté réelle vs autorité)
- [ ] Capacité à récupérer un email (lead magnet intégré)
- [ ] Score RRF (Reciprocal Rank Fusion — métrique retriever interne)

**❌ ANCIENS KPIs (vanité, « d'un autre temps ») :**
- ❌ Trafic brut
- ❌ Volume de recherche
- [ ] Nombre de backlinks
- ❌ Position moyenne (ex: rank moyen 50 mais top 1 sur « agence seo » = OK)

---

## STRUCTURE VAULT OBSIDIAN (référence)

```
vault/
├── AGENTS.md                    # Instructions IA (racine)
├── raw/                         # Sources brutes (lecture seule)
│   ├── gsc-exports/
│   ├── client-calls/
│   ├── reddit-threads/
│   └── competitor-pages/
├── wiki/                        # Domaine agent (wikilinks partout)
│   ├── AGENTS.md                # Copie/référence
│   ├── mots-cles/
│   │   ├── mots-cles-decisionnels.md
│   │   ├── mots-cles-overview.md
│   │   ├── mots-cles-resistants-ia.md
│   │   └── peurs-objections.md
│   ├── architecture/
│   │   ├── cluster-aeo/
│   │   ├── modeles-pseo/
│   │   ├── programmatique-pseo/
│   │   ├── maillage-systeme/
│   │   └── roadmap-pseo/
│   ├── contenu/
│   │   ├── workflow-article.md
│   │   ├── ton-de-voix.md
│   │   ├── redaction-guide.md
│   │   └── page-statistiques.md
│   ├── geo/
│   │   ├── geo-audit.md
│   │   ├── donnees-structurees.md
│   │   └── product-led-seo.md
│   ├── signaux-sociaux/
│   │   ├── reddit-cockpit.md
│   │   ├── x-reply-cockpit.md
│   │   └── linkedin-journal.md
│   ├── veille/
│   │   ├── breves-quotidiennes.md
│   │   └── newsletter-ia.md
│   ├── audits/
│   │   └── audit-<client>-<date>.md
│   ├── cannibalisation/
│   │   └── plan-action-<date>.md
│   └── systeme/
│       ├── 281-faits-memoire.md
│       ├── 66-procedures.md
│       └── 27-automatisations.md
└── .chroma/                     # ChromaDB local (RAG)
```

---

## OUTILS OFFICIELLEMENT RECOMMANDÉS (par Timseo_)

| Outil | Usage | Coût |
|-------|-------|------|
| **Claude Code** | LLM principal, code, analyse, rédaction | 20 €/mois |
| **Obsidian** | Vault, wikilinks, structure Karpathy | Gratuit |
| **ChromaDB** | Vector DB RAG local | Gratuit (self-hosted) |
| **Sentence-Transformers** | Embeddings locaux | Gratuit |
| **Google Keyword Planner** | CPC + volume (seuls indicateurs fiables) | Gratuit (compte Google Ads) |
| **Reddit** | Signaux utilisateurs, vraies questions | Gratuit |
| **Grok + DeepSearch** | Signaux émergents, recherche temps réel | Inclus X Premium |
| **Google Search Console** | Données réelles positions/indexation | Gratuit |
| **Qadence.io** | Agent SEO SaaS (scrape GSC auto) | Freemium |
| **Resend** | Email transactionnel | 100 emails/jour gratuits |
| **Supabase** | Collecte data support client | Gratuit (petits volumes) |
| **Vite + prerender.mjs** | Build + prerender sites statiques | Gratuit |
| **Lighthouse (local)** | Core Web Vitals mobile-first | Gratuit |
| **Schema.org** | Référentiel JSON-LD | Gratuit |
| **launchd** | Cron macOS pour automatisations | Gratuit |

**Outils SEO payants ARRÊTÉS** : Semrush, Ahrefs, Majestic, Screaming Frog, etc. (« data généraliste quasi obsolète »)

---

## PROMPTS CLAUDE CLÉS (à copier dans vault/wiki/)

### Prompt recherche mots-clés
```
Tu es expert SEO. Contexte : [coller data proprio + signaux Reddit + GKP].
Mission : identifier 3-5 mots-clés business + 10 micro-intentions chacun.
Format sortie : tableau markdown avec colonnes [Mot-clé business] [Intention Do/Know] [Requête longue] [Objection] [Format page] [Priorité].
```

### Prompt audit cannibalisation
```
Analyse cet export GSC 90j complet (1M tokens). Isole toutes requêtes 2+ URLs.
Pour chaque conflit : classe (exact/intention/proximité), compare positions/impressions/clics/CTR.
Sortie : plan d'action markdown avec décision [301|Fusion|Séparation|Rien] + justification.
RÈGLE ABSOLUE : si 301, jamais 410. Si 2 pages top 10 → écrire 2 angles distincts.
```

### Prompt maillage interne
```
Voici le crawl complet (ou export GSC) du site. Propose un maillage interne optimal.
Contraintes : ancre naturelle, contexte pertinent, max 3 liens sortants par page, priorité pages business.
Sortie : liste CSV [page_source] [page_cible] [ancre] [contexte_phrase] [priorité].
```

### Prompt score citabilité LLM
```
Lis ce contenu EN ENTIER avec la requête cible : [requête] et type page : [article/landing/faq].
Note 7 scores sur 100 : Surprise, Grounding, Content Effort, Alignement RRF, RAG Structurer, Freshness Guard, Atomic Proofs.
Compte preuves atomiques (triplets [sujet][relation][valeur]) → seuil 2/100 mots.
Vérifie réponse dans 30 mots après chaque H2.
Cite phrases exactes problèmes. Sortie : plan réécriture attaquant 2 scores les plus bas.
```

### Prompt anti-voix-IA
```
Liste les patterns "voix de Claude" à éviter (mots de liaison, structures, tournures).
Puis réécris ce texte en les évitant scrupuleusement.
Style : direct, expert, exemples concrets, pas de fluff, phrases courtes.
```

---

## CHECKLIST RAPIDE DÉPLOIEMENT (pour nouveau projet)

```bash
# 1. Setup système (W0) — 30 min
☐ Vault Obsidian raw/wiki + AGENTS.md
☐ ChromaDB + embeddings
☐ ./kb rebuild OK
☐ 27 automatisations configurées

# 2. Stratégie (W1-W2) — 2-4h
☐ 3-5 mots-clés business identifiés
☐ 10 micro-intentions / mot-clé
☐ Data propriétaire collectée (appels, SAV, avis)
☐ Signaux Reddit/X récupérés
☐ Univers sémantique défini par verticale
☐ 1-15 pages planifiées par requête stratégique
☐ Templates pSEO créés (si applicable)

# 3. Technique (W5) — 1h
☐ Checklist base technique validée (19 points)
☐ JSON-LD déployés (Org/WebSite/Article/FAQ)
☐ Sitemap + robots.txt + 404.html
☐ Lighthouse mobile passé (LCP/INP/CLS verts)

# 4. Contenu (W2-W8) — continu
☐ Pages business produites (cas usage, comparatifs, FAQ, data proprio)
☐ Ton de voix appliqué (anti-patterns IA)
☐ Maillage interne lancé (Claude)
☐ Signaux sociaux activés (LinkedIn/YouTube/Reddit)
☐ Score citabilité LLM ≥ 70/100 sur pages cibles

# 5. Audit & Boucle (W9) — mensuel
☐ Audit 7 phases lancé
☐ Cannibalisation vérifiée
☐ Plan 90j mis à jour
☐ Automatisations santé vérifiées (lundi)
```

---

## RÉFÉRENCES RAPIDES (posts sources les plus cités)

| Thème | Post clé | Date |
|-------|----------|------|
| 10 principes SEO 2026 | [2070580100979114069](https://x.com/Timseo_/status/2070580100979114069) | 26/06/2026 |
| Fin des mots-clés | [2075179658706895230](https://x.com/Timseo_/status/2075179658706895230) | 09/07/2026 |
| Système complet (66 proc, 1528 notes, 281 faits, 27 auto) | [2088292563153551525](https://x.com/Timseo_/status/2088292563153551525) | 14/08/2026 |
| Guide agent SEO 7 phases | [2087568290612949463](https://x.com/Timseo_/status/2087568290612949463) | 12/08/2026 |
| Checklist technique site Claude | [2087203754324242918](https://x.com/Timseo_/status/2087203754324242918) | 11/08/2026 |
| Cas Golfiller (top 1 sans BL achat) | [2094097061012541844](https://x.com/Timseo_/status/2094097061012541844) | 30/08/2026 |
| Score citabilité LLM 7 dims | [2091926256581587093](https://x.com/Timseo_/status/2091926256581587093) | 24/08/2026 |
| Nouveaux KPIs SEO | [2086703171657932977](https://x.com/Timseo_/status/2086703171657932977) | 10/08/2026 |
| Signaux sociaux top 6 | [2083533202065445266](https://x.com/Timseo_/status/2083533202065445266) | 01/08/2026 |
| Lancement site 15 min | [2082488568723976344](https://x.com/Timseo_/status/2082488568723976344) | 29/07/2026 |

---

## USAGE DANS HERMES

```bash
# Charger le skill
# (le skill est auto-disponible une fois placé dans ~/.hermes/skills/timseo-seo/)

# Exemple d'utilisation en conversation :
# "Lance W1 pour mon client [nom] — voici leur data proprio : ..."
# "Fais un audit W9 complet sur monsite.com"
# "Génère le plan maillage W3 pour mon export GSC"
# "Score la citabilité LLM de cette page pour la requête '...'"
```

---

## MAINTENANCE

- **Mise à jour doctrine** : relancer l'analyse @Timseo_ tous les 3-6 mois (nouveaux posts)
- **Versioning** : incrémenter `version` dans frontmatter à chaque modification majeure
- **Fact store** : sauvegarder les décisions clients / résultats d'audit via `fact_store(action='add', category='project')`
- **Partage** : ce skill est personnel — ne pas publier sans accord

---

*Skill créé le 2026-09-01 par Octo pour Teeflo. Basé sur 100+ publications @Timseo_ (juin 2025 → août 2026). Voir rapport complet pour sources exhaustives et nuances.*