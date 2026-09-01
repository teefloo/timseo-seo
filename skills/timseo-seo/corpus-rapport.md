# TimSEO (@Timseo_) — Base de connaissances SEO

> Source : compte X public [@Timseo_](https://x.com/Timseo_)
> Date du rapport : 1er septembre 2026
> Auteur de l'analyse : Octo (compte rendu objectif, sans complétude SEO générale ajoutée)

---

## 1. Couverture de la recherche

**Sources exploitées**
- Profil X public via MCP `user_profile` et `user_timeline` (réponses incluses).
- Recherche `from:Timseo_` via MCP `search` (produit `Latest`) sur la requête par défaut + filtres keyword (`SEO`, `mots-clés`, `maillage`, `contenu`, `indexation`, `Search Console`, `Claude`, `programmatique`, `AEO`, `GEO`, `pSEO`, `decisionnels`, `micro-intentions`, `data propriétaire`, `RRF`, `cannibalisation`, `Core Web Vitals`, `données structurées`, `Reddit`, `YouTube`, `LinkedIn`, `niche`, `autorité`, `ton de voix`, `Ahrefs`, `Semrush`, `Majestic`, `schema`, `JSON-LD`, `EEAT`).
- Lectures directes de posts ciblés via `read_tweet` (URLs x.com/Timseo_/status/...).
- Recherches web Google `site:x.com/Timseo_/status/...` et requêtes typées (`"Timseo_" "référencement"`, `"TimSEO" "2024"`, etc.).
- Page de profil publique ouverte via le navigateur distant (vérification du titre/bio).

**Période couverte**
- Couvre principalement **juin 2025 → fin août 2026** (~15 mois). L'API MCP X ne remonte aucun résultat pour la période 2022–2024 dans nos requêtes, malgré plusieurs tentatives de filtrage par date. L'indexation des posts antérieurs semble inaccessible via l'API actuelle.
- Le compte lui-même mentionne « 6 ans de SEO » et « 1000+ articles de blog » ([2084097061012541844](https://x.com/Timseo_/status/2094097061012541844), 30 août 2026), ce qui suggère une activité publique plus ancienne ; elle n'est pas couverte ici.

**Limites rencontrées**
- API MCP X : timeouts répétés (≥ 300 s) sur plusieurs requêtes thématiques ; pas de résultats pour `since:2022..2024`. La profondeur historique avant mi-2025 n'est pas vérifiable via les outils utilisés.
- Posts contenant uniquement un lien `x.com/i/article/...` (long-form X) : leur contenu n'est pas exposé par `search`/`read_tweet` ; ils ne sont comptés que comme publications quand l'auteur du rapport le déduit de leur présence dans le fil.
- Threads : lus via `read_tweet` post-par-post ; les citations de tweets intégrés ne sont pas toujours toutes restituées.
- Compte francophone : corpus FR à ~95 % (quelques messages EN), analyse faite en français pour rester fidèle.

**Niveau de confiance sur l'exhaustivité**
- **Élevée** sur la période mi-2025 → fin août 2026 pour le contenu SEO explicite.
- **Faible à moyenne** sur la période antérieure (impossible à vérifier via les outils ; les « 10 principes » [2070580100979114069](https://x.com/Timseo_/status/2070580100979114069) et la « 1re astuce » [2074011209620173307](https://x.com/Timseo_/status/2074011209620173307) ne sont probablement pas ses tous premiers posts SEO).
- **Élevée** sur l'identification des grandes thèses récurrentes (reconnaissance par la fréquence d'apparition + le nombre d'engagement).

---

## 2. Principes SEO majeurs de Timseo_ (synthèse)

Sept thèses reviennent massivement, plusieurs fois par semaine, sur la période couverte. Elles structurent l'ensemble de ses conseils et constituent sa « doctrine » publique :

1. **Le trafic informationnel est mort à l'ère des LLM** — l'objectif n'est plus le volume, c'est la **pertinence business** ([2081708176714645944](https://x.com/Timseo_/status/2081708176714645944), 27 juil. 2026 ; [2094097061012541844](https://x.com/Timseo_/status/2094097061012541844), 30 août 2026).
2. **Travailler 5 mots-clés business plutôt que 1 500** — c'est l'**autorité thématique** autour d'un noyau restreint ([2092300598851100709](https://x.com/Timseo_/status/2092300598851100709), 25 août 2026 ; [2089384759948357958](https://x.com/Timseo_/status/2089384759948357958), 17 août 2026).
3. **La data propriétaire est le seul vrai moat face à l'IA** — appels clients, SAV, avis, data métier, comparaisons faites-maison ([2079227329616941500](https://x.com/Timseo_/status/2079227329616941500), 20 juil. 2026 ; [2088292563153551525](https://x.com/Timseo_/status/2088292563153551525), 14 août 2026 ; [2081708176714645944](https://x.com/Timseo_/status/2081708176714645944)).
4. **Cibler les intentions « Do », pas « Know »** — comparer, calculer, acheter, demander une démo. Ce sont les requêtes que les LLM ne peuvent pas voler ([2092300598851100709](https://x.com/Timseo_/status/2092300598851100709) ; [2094097061012541844](https://x.com/Timseo_/status/2094097061012541844)).
5. **Les backlinks ne sont pas indispensables** — il revendique des top 1 sans aucun backlink payant ([2070450497081774390](https://x.com/Timseo_/status/2070450497081774390), 26 juin 2026 ; [2084886929833931130](https://x.com/Timseo_/status/2084886929833931130), 5 août 2026 ; [2092300598851100709](https://x.com/Timseo_/status/2092300598851100709)).
6. **Outils SEO classiques = data généraliste dépassée** — il a « coupé tous ses abonnements » depuis 2 ans ([2088292563153551525](https://x.com/Timseo_/status/2088292563153551525) ; [2088520297364553960](https://x.com/Timseo_/status/2088520297364553960), 15 août 2026 ; [2085368294882590801](https://x.com/Timseo_/status/2085368294882590801), 6 août 2026).
7. **Le SEO devient un système d'orchestration IA + data propriétaire** — Claude + Obsidian + RAG + skills + workflows séquencés ([2079227329616941500](https://x.com/Timseo_/status/2079227329616941500) ; [2084644273543422325](https://x.com/Timseo_/status/2084644273543422325), 4 août 2026 ; [2087568290612949463](https://x.com/Timseo_/status/2087568290612949463), 12 août 2026).

> Note : ces thèses sont toutes des **opinions explicitement énoncées par l'auteur** dans ses posts, pas une interprétation.

---

## 3. Tous les conseils SEO extraits, par thème

### 3.1 Choix de niche et de mots-clés

- **Choisir une niche ultra-spécifique**, « là où vous pouvez gagner », pas un grand mot-clé générique ([2078452818516873416](https://x.com/Timseo_/status/2078452818516873416), 18 juil. 2026 ; cas client « balle de golf d'occasion » → top 1 sur « balle de golf »).
- **Identifier 3 à 5 mots-clés business** par niche, puis 5 à 10 micro-intentions par mot-clé ([2074011209620173307](https://x.com/Timseo_/status/2074011209620173307), 6 juil. 2026 ; [2078452818516873416](https://x.com/Timseo_/status/2078452818516873416)).
- **Travailler en priorité des micro-intentions** : il observe que les requêtes sont passées de 4 mots à 24 mots ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069), 26 juin 2026).
- **« C'est la fin des mots-clés en SEO »** : 3 arguments — 1) les requêtes sont des phrases ; 2) les LLM répondent directement ; 3) le volume n'a plus de sens → se concentrer sur des univers sémantiques ([2075179658706895230](https://x.com/Timseo_/status/2075179658706895230), 9 juil. 2026).
- **Méthode de recherche actuelle** (remplace les outils SEO) :
  1. CPC + volume → Google Keyword Planner
  2. Reddit Ask → intentions réelles
  3. Grok + DeepSearch → signaux utilisateurs
  4. Données propriétaires → Obsidian
  5. GSC → Qadence (son outil)
  ([2079931721139544316](https://x.com/Timseo_/status/2079931721139544316), 22 juil. 2026)
- **« Je n'utilise plus aucun outil SEO payant pour trouver mes mots-clés »** — workflow : data propriétaire + signaux sociaux (Reddit, X) + Obsidian + Claude ([2083201216960761955](https://x.com/Timseo_/status/2083201216960761955), 31 juil. 2026).
- **Identifier les « mots-clés décisionnels »** (ceux qui mènent à une action) vs « mots-clés informationnels » (qui seront mangés par les LLM) ([2082848692176830871](https://x.com/Timseo_/status/2082848692176830871), 30 juil. 2026, arborescence agent).
- **« Mots-clés overview »** = requêtes qui déclenchent des AI Overviews, à traiter différemment ([2082848692176830871](https://x.com/Timseo_/status/2082848692176830871)).
- **« Mots-clés résistants-IA »** = catégorie dédiée dans son agent, pour repérer les requêtes où l'IA ne peut pas répondre seule ([2082848692176830871](https://x.com/Timseo_/status/2082848692176830871)).
- **« Peurs/objections »** : utiliser Claude pour générer 10 micro-intentions par mot-clé business ([2078452818516873416](https://x.com/Timseo_/status/2078452818516873416)).

### 3.2 Architecture de contenu et silos sémantiques

- **Construire un « univers sémantique sur une verticale précise »**, pas un silo généraliste ([2086851567693791312](https://x.com/Timseo_/status/2086851567693791312), 10 août 2026).
- **Chaîne recommandée** : mot-clé business → longue traîne → vecteurs sémantiques → micro-intentions → univers sémantique ([2086851567693791312](https://x.com/Timseo_/status/2086851567693791312)).
- **5 requêtes stratégiques > 100 mots-clés** : autour de chaque requête, construire 1 à 15 pages en cluster ([2092300598851100709](https://x.com/Timseo_/status/2092300598851100709)).
- **Types de pages à produire** : cas d'usage, comparatifs, réponses aux objections, contenus d'expertise, données propriétaires, directories (prix, tendances, comparatifs solutions) ([2092300598851100709](https://x.com/Timseo_/status/2092300598851100709)).
- **Programmatique SEO « sans spam »** : « Un template = une variable = des centaines de pages pour récupérer des emails qualifiés » ([2094097061012541844](https://x.com/Timseo_/status/2094097061012541844)).
- **Pages « alternatives à X »** comme moteur d'acquisition SaaS : Alternatives à X / Alternative gratuite à X / Alternative française à X ([2085987057223028937](https://x.com/Timseo_/status/2085987057223028937), 8 août 2026).
- **Cluster AEO** = groupement thématique orienté réponses (vs cocon sémantique classique) ([2081765303273627867](https://x.com/Timseo_/status/2081765303273627867), 27 juil. 2026 ; [2067511329284563142](https://x.com/Timseo_/status/2067511329284563142), 18 juin 2026).
- **« Modèles pSEO »** = templates réutilisables pour générer des pages à grande échelle avec qualité ([2081765303273627867](https://x.com/Timseo_/status/2081765303273627867) ; [2082848692176830871](https://x.com/Timseo_/status/2082848692176830871)).
- **« Roadmap pSEO »** = enchaînement programmation → production → publication ([2081765303273627867](https://x.com/Timseo_/status/2081765303273627867)).

### 3.3 Maillage interne

- **À déléguer entièrement à Claude** : « il a été capable de créer 62 liens en 30 minutes » ([2083222405653114909](https://x.com/Timseo_/status/2083222405653114909), 31 juil. 2026).
- **Avec ou sans Search Console** : Claude peut mailler à partir d'un crawl, même sans export GSC ([2079136005748359329](https://x.com/Timseo_/status/2079136005748359329), 20 juil. 2026 ; [2080632841944064159](https://x.com/Timseo_/status/2080632841944064159), 24 juil. 2026).
- **Le maillage « mappé » visuellement** : il détourne un GitHub pour visualiser le graphe ([2082139518673813616](https://x.com/Timseo_/status/2082139518673813616), 28 juil. 2026).

### 3.4 Cannibalisation

- **Détection via export GSC 90 jours entier** (≈ 1 M de tokens), requête par requête et URL par URL ([2089743876244529215](https://x.com/Timseo_/status/2089743876244529215), 18 août 2026).
- **Classifier le conflit** : mot-clé exact / même intention / proximité sémantique.
- **Décision page par page** : 301, fusion, séparation des micro-intentions, **ou aucune action** (si les 2 pages occupent 2 places du top 10 → écrire chaque page sur un angle distinct).
- **Règle 410 vs 301** : il ne supprime jamais la perdante. **301 vers celle qui reste, toujours** — un 410 fait perdre les liens déjà acquis ([2089743876244529215](https://x.com/Timseo_/status/2089743876244529215)).

### 3.5 SEO technique

- **« Le SEO technique reste ultra important »** MAIS délégable à 100 % à l'IA ([2079136005748359329](https://x.com/Timseo_/status/2079136005748359329)).
- **Ce que Claude peut faire** : audit complet, maillage, cannibalisation, données structurées, Core Web Vitals, vitesse ([2079136005748359329](https://x.com/Timseo_/status/2079136005748359329) ; [2077366949785595919](https://x.com/Timseo_/status/2077366949785595919), 15 juil. 2026).
- **Workflow Core Web Vitals** : récupérer sitemap.xml → Lighthouse en local (mobile, mobile-first) → mesurer → Claude liste et corrige les problèmes → sortir les 5 pires pages avec plan d'action ([2077366949785595919](https://x.com/Timseo_/status/2077366949785595919)).
- **Audit d'indexation hebdomadaire** via Claude : 404, sitemap, vérification Google, sans outil ([2075310521146867897](https://x.com/Timseo_/status/2075310521146867897), 9 juil. 2026).
- **Checklist « base technique à copier-coller » pour un site codé avec Claude** ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918), 11 août 2026) :
  - Rendu : pas de SPA pure ; 3 options (prerender post-build `vite build` avec `scripts/prerender.mjs`, framework SSR/SSG type Next/Astro/Remix, ou prerender headless Puppeteer/Playwright)
  - Chaque route publique doit avoir son propre HTML avec `<title>`, `<meta description>`, `<link rel="canonical">` déjà présents dans le HTML brut (pas après hydratation JS)
  - À la racine : `sitemap.xml` auto-généré depuis les routes, `robots.txt` pointant vers le sitemap, vrai `404.html` retournant un 404
  - Par page : `<title>`/`<meta description>` uniques, un seul `<h1>`, hiérarchie h2/h3, canonical explicite, Open Graph + Twitter Card
  - JSON-LD : `Organization`/`WebSite` en home, `Article` en blog, `FAQPage` seulement si FAQ visible
  - Perf : lazy-load images avec `width`/`height` explicites, `font-display: swap`

### 3.6 Données structurées / JSON-LD

- **Règle stricte** : ne jamais utiliser un schéma qui ne correspond pas à un contenu visible — Google peut sanctionner ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918)).
- **Claude génère les schémas** ([2079136005748359329](https://x.com/Timseo_/status/2079136005748359329) ; renvoie vers Schema.org).

### 3.7 Core Web Vitals / performance

- Lenteur = mauvaise UX, baisse de conversion et de ranking ([2077366949785595919](https://x.com/Timseo_/status/2077366949785595919)).
- Mesure **mobile-first** : Google indexe en mobile ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918)).

### 3.8 Indexation

- **Audit mensuel d'indexation** dans son système automatisé ([2088292563153551525](https://x.com/Timseo_/status/2088292563153551525)).
- **Indexation = pré-requis SEO technique**, pas un sujet isolé ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918) ; [2085771177944125757](https://x.com/Timseo_/status/2085771177944125757), 7 août 2026, arborescence système).
- **« Pages SEO pour SaaS »** : types de pages récurrentes à produire ([2085987057223028937](https://x.com/Timseo_/status/2085987057223028937)).

### 3.9 Authority / Topical Authority / E-E-A-T

- **« L'autorité thématique = capacité à se positionner sur un mot-clé + X mots-clés secondaires »** ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069)).
- **E-E-A-T = cas clients + avis clients** (formulation Timseo_) ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069)).
- **Cas clients + données first-party** = socle E-E-A-T ([2085771177944125757](https://x.com/Timseo_/status/2085771177944125757) ; [2087203754324242918](https://x.com/Timseo_/status/2087203754324242918)).

### 3.10 Liens et backlinks

- **« On vous a vendu l'idée que faire du SEO sans acheter de backlinks était impossible. La réalité, c'est qu'on vous vend souvent des conseils qui datent de 20 ans »** ([2094097061012541844](https://x.com/Timseo_/status/2094097061012541844)).
- **Cas client Golfiller** : top 1 sur « balle de golf » (6 000 recherches/mois) devant Décathlon, **sans backlink payant** ([2092300598851100709](https://x.com/Timseo_/status/2092300598851100709) ; [2094097061012541844](https://x.com/Timseo_/status/2094097061012541844) ; [2094407438602739747](https://x.com/Timseo_/status/2094407438602739747), 31 août 2026, où il clarifie : le site a des BL, mais « 0 BL ni achat ni BL tout court en 2 ans »).
- **« Les backlinks sont remplacés par les signaux sociaux (Reddit, LinkedIn en particulier) »** ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069)).
- **« Pas besoin de BL pour ranker »** en réponse à @JespernissenSEO ([2084886929833931130](https://x.com/Timseo_/status/2084886929833931130), 5 août 2026).
- **« Don't buy backlink »** à @lilyraynyc ([2093334188498006507](https://x.com/Timseo_/status/2093334188498006507), 28 août 2026).

### 3.11 Signaux sociaux & off-site (le « nouveau link building »)

- **Reddit** : top 2 des sites externes prioritaires ([2083533202065445266](https://x.com/Timseo_/status/2083533202065445266), 1er août 2026).
- **LinkedIn** : top 3 ([2083533202065445266](https://x.com/Timseo_/status/2083533202065445266)) — il est passé de ~1 000 à 15 K abonnés en 2026 ([2086721711978987528](https://x.com/Timseo_/status/2086721711978987528), 10 août 2026).
- **YouTube** : top 1 ([2083533202065445266](https://x.com/Timseo_/status/2083533202065445266)) — « Meilleure strat SEO 2026 : SEO + LinkedIn + YouTube » ([2070049889581715518](https://x.com/Timseo_/status/2070049889581715518), 25 juin 2026).
- **X (Twitter)** : pour le contenu court, en complément ([2086721711978987528](https://x.com/Timseo_/status/2086721711978987528)).
- **Substack** : pour le contenu long, 4 ans à le construire comme canal d'acquisition (jamais monétisé) ([2086721711978987528](https://x.com/Timseo_/status/2086721711978987528) ; [2094322294323597812](https://x.com/Timseo_/status/2094322294323597812), 31 août 2026).
- **Pinterest** : top 6 des sites externes ([2083533202065445266](https://x.com/Timseo_/status/2083533202065445266)).
- **Astuce pour ranker sur des mots-clés compétitifs** ([2082113849705345533](https://x.com/Timseo_/status/2082113849705345533), 28 juil. 2026) :
  1. Cibler des mots-clés de nouvelle génération, que les gros sites n'ont pas (ou peu) traités
  2. Publier un contenu optimisé sur ce mot-clé sur LinkedIn (YouTube fonctionne aussi)
  3. Générer un maximum d'engagement
  4. Tester, tester, tester — toujours sans spammer
  5. Répéter
- **LinkedIn = canal SEO à part entière** : on peut ranker un post LinkedIn, « opportunité SEO à saisir avec une approche multimodale » ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069) ; [2083533202065445266](https://x.com/Timseo_/status/2083533202065445266)).
- **Stratégie « extension Chrome comme SEO »** : découper chaque fonctionnalité de son SaaS en micro-outil ([2079149819046863023](https://x.com/Timseo_/status/2079149819046863023), 20 juil. 2026).

### 3.12 GEO / AEO (Generative & Answer Engine Optimization)

- **Définition personnelle** : « être suffisamment pertinent pour être sélectionné par un LLM » ([2092300598851100709](https://x.com/Timseo_/status/2092300598851100709)).
- **GSC a ajouté les réseaux sociaux** : « Google nous envoie un message très très clair : le SEO des 20 dernières années ne sera rien comparé à ce qui arrive » ([2082483283716366801](https://x.com/Timseo_/status/2082483283716366801), 29 juil. 2026).
- **« GEO n'est pas du scam, Google le prend très au sérieux »** ([2075475609447510389](https://x.com/Timseo_/status/2075475609447510389), 10 juil. 2026).
- **Tool interne** : `geo-audit`, `donnees-structurees`, `product-led-seo` dans son arborescence agent ([2081765303273627867](https://x.com/Timseo_/status/2081765303273627867)).
- **Skill « citation IA »** : repère les mots-clés « mangés » ou non par les IA ([2085033589172023463](https://x.com/Timseo_/status/2085033589172023463), 5 août 2026).
- **Skill de scoring « citabilité LLM »** ([2091926256581587093](https://x.com/Timseo_/status/2091926256581587093), 24 août 2026) :
  - 7 scores sur 100 : Surprise, Grounding, Content Effort, Alignement RRF, RAG Structurer, Freshness Guard (2 non cités dans l'extrait : prob. Atomic Proofs + Time-to-Answer)
  - « Preuves atomiques » = triplets [sujet] + [relation] + [valeur chiffrée ou entité nommée], seuil 2 par 100 mots
  - Vérifier que la réponse arrive dans les 30 mots après chaque H2 (sinon le retriever ne l'associe pas à la question)
  - Citer la phrase exacte pour chaque problème
- **« Pour le moment c'est 3% du trafic le GEO »** (mesure perso, juin 2026) ([2070043197590688233](https://x.com/Timseo_/status/2070043197590688233)).
- **Astuces sur AI Overviews** : « ciblez des requêtes que ChatGPT ne peut pas voler — intention Do » ([2082113849705345533](https://x.com/Timseo_/status/2082113849705345533) ; [2092300598851100709](https://x.com/Timseo_/status/2092300598851100709)).
- **Critique** : les consultants qui copient-collent du contenu IA « détruisent le SEO, et là on recommence avec le GEO » ([2072891212600885294](https://x.com/Timseo_/status/2072891212600885294), 3 juil. 2026).

### 3.13 Contenu / Production

- **« Construire des pages pour les humains ET les robots »** ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069)).
- **« 95 % des visites ne génèrent aucune vente, tu as donc besoin de motiver tes visiteurs à laisser leur email (outil IA, simulateur, etc.) »** ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069)).
- **Ton de voix** : « sortir de la voix de Claude » ([2087568290612949463](https://x.com/Timseo_/status/2087568290612949463)) — il a un skill dédié `/ton-de-voix` ([2081765303273627867](https://x.com/Timseo_/status/2081765303273627867)).
- **Workflow article** : `brief → preparation-semantique → workflow-article → redaction-guide → page-statistiques` ([2081765303273627867](https://x.com/Timseo_/status/2081765303273627867)).
- **Anti-pattern IA** : pour éviter le « son IA », il demande à ChatGPT de lister les patterns IA, puis dit à Claude de les respecter en les évitant ([2073405391946576323](https://x.com/Timseo_/status/2073405391946576323), 4 juil. 2026).
- **Production d'assets** : il fait logos, animations, UX/UI lui-même avec Claude, « 0 CMS » ([2074030748303270361](https://x.com/Timseo_/status/2074030748303270361), 6 juil. 2026 ; [2079898498926047365](https://x.com/Timseo_/status/2079898498926047365), 22 juil. 2026 ; [2077773751593443784](https://x.com/Timseo_/status/2077773751593443784), 16 juil. 2026).
- **Sites full Claude (sans CMS)** : exemples `fusionn.co`, `qadence.io`, `seocity.app`, autres sites lancés en 15 min ([2073405538189344935](https://x.com/Timseo_/status/2073405538189344935) ; [2082488568723976344](https://x.com/Timseo_/status/2082488568723976344), 29 juil. 2026 ; [2082742743613288874](https://x.com/Timseo_/status/2082742743613288874), 30 juil. 2026).

### 3.14 Sémantique

- **Audit sémantique** sans outil ([2080348718839066635](https://x.com/Timseo_/status/2080348718839066635), 23 juil. 2026) : lister les entités sémantiques attendues par Google, vérifier le lexique, identifier les micro-intentions, ajouter de l'Information Gain, scorer sur 100, corriger Title/meta/Hn.
- **« Problème sémantique = risque d'invisibilité sur Google et les LLM »** ([2080348718839066635](https://x.com/Timseo_/status/2080348718839066635)).
- **Vecteurs sémantiques** = étape de la chaîne sémantique ([2086851567693791312](https://x.com/Timseo_/status/2086851567693791312)).
- **Entités vectorielles** = skill dédié ([2081765303273627867](https://x.com/Timseo_/status/2081765303273627867)).

### 3.15 Audit / Diagnostic SEO complet

**7 phases d'un audit complet via Claude** ([2088333331729350694](https://x.com/Timseo_/status/2088333331729350694), 14 août 2026) :
- Phase 0 → audit site/SERP
- Phase 1 → quick wins
- Phase 2 → cannibalisation
- Phase 3 → clusters AEO
- Phase 4 → vecteurs sémantiques
- Phase 5 → maillage interne
- Phase 6 → briefs contenu
- Phase 7 → plan d'action 90 jours

**Couverture** : scraping, audit maillage, cannibalisation, clusters sémantiques, content gaps, briefs ([2088333331729350694](https://x.com/Timseo_/status/2088333331729350694)).

### 3.16 Métriques & KPIs

**KPI traditionnels qu'il considère « d'un autre temps »** ([2086703171657932977](https://x.com/Timseo_/status/2086703171657932977), 10 août 2026 ; [2086703171657932977](https://x.com/Timseo_/status/2086703171657932977)) :
- Trafic, volume de recherche, nombre de backlinks.

**Nouveaux KPI qu'il suit** ([2086703171657932977](https://x.com/Timseo_/status/2086703171657932977)) :
- Proximité de l'offre
- Intention d'achat
- CPC
- Faisabilité de ranking
- Capacité à récupérer un email
- Score RRF (Reciprocal Rank Fusion — métrique interne liée aux retrievers)

**« Le trafic n'est pas la meilleure métrique SEO »** : un mot-clé à 5 000 recherches/mois peut n'avoir aucun intérêt business ([2086703171657932977](https://x.com/Timseo_/status/2086703171657932977) ; [2081708176714645944](https://x.com/Timseo_/status/2081708176714645944)).

**Position moyenne = « KPI à ne surtout pas suivre »** : tu peux avoir un rank moyen de 50 et être top 1 sur « agence seo » ([2086053157982126505](https://x.com/Timseo_/status/2086053157982126505), 8 août 2026).

### 3.17 Veille & signaux

- **Revue de presse SEO IA quotidienne** dans son système ([2088292563153151525](https://x.com/Timseo_/status/2088292563153551525)).
- **Reddit Cockpit quotidien** (automatisation interne) ([2088292563153151525](https://x.com/Timseo_/status/2088292563153551525) ; [2085771177944125757](https://x.com/Timseo_/status/2085771177944125757)).
- **Reddit pour identifier les vraies questions** (et faire des FAQ) ([2074011209620173307](https://x.com/Timseo_/status/2074011209620173307) ; [2085771177944125757](https://x.com/Timseo_/status/2085771177944125757)).
- **Brèves IA 2×/jour, newsletter hebdo** ([2085771177944125757](https://x.com/Timseo_/status/2085771177944125757)).
- **Skill `x-reply-cockpit` + `linkedin-journal`** pour piloter sa présence sociale ([2081765303273627867](https://x.com/Timseo_/status/2081765303273627867)).

---

## 4. Techniques et workflows concrets

### 4.1 Système SEO personnel « maison » (le cœur de sa doctrine)

**Stack** ([2088292563153151525](https://x.com/Timseo_/status/2088292563153551525) ; [2085771177944125757](https://x.com/Timseo_/status/2085771177944125757) ; [2084644273543422325](https://x.com/Timseo_/status/2084644273543422325)) :
- **Claude** (Code) comme LLM
- **Obsidian** comme vault de notes (markdown)
- **Structure Karpathy** : `raw/` (lecture seule) + `wiki/` (domaine agent) ([2084644273543422325](https://x.com/Timseo_/status/2084644273543422325))
- **Wikilinks Obsidian** partout (`[[nom-du-concept]]`)
- **RAG local** : ChromaDB + Sentence-Transformers, recherche sémantique sur 1 528 notes SEO ([2088292563153151525](https://x.com/Timseo_/status/2088292563153551525))
- **`AGENTS.md`** à la racine : instructions à l'IA pour lire/écrire dans le vault
- **CLI `./kb`** + commande `./kb rebuild` (rebuild incrémental)
- **281 faits en mémoire permanente** : positions, règles, stratégies, décisions clients — rechargés à chaque session ([2088292563153151525](https://x.com/Timseo_/status/2088292563153551525))

**Volumes revendiqués** ([2088292563153151525](https://x.com/Timseo_/status/2088292563153551525) ; [2088292563153151525](https://x.com/Timseo_/status/2088292563153551525)) :
- 66 procédures (25 SEO pur + 41 production)
- 1 528 notes SEO en RAG
- 281 faits en mémoire
- 27 automatisations techniques

**Le setup n'est PAS « Claude tout seul »** : « L'erreur est d'utiliser Claude tout seul. Le bon setup c'est Claude + Obsidian + skills + un workflow séquencé » ([2088333331729350694](https://x.com/Timseo_/status/2088333331729350694)).

### 4.2 Construction d'un agent SEO (méthode officielle) — 7 phases

D'après [2087568290612949463](https://x.com/Timseo_/status/2087568290612949463) (12 août 2026) :
- **Phase 0** : ce qu'est un agent SEO (≠ chatbot) et pourquoi le construire (anti-commodité)
- **Phase 1** : le socle (Claude Code + vault markdown raw/wiki + fichier de doctrine)
- **Phase 2** : data propriétaire (calls, SAV, avis, GSC) — le pré-requis non négociable
- **Phase 3** : 9 skills dans l'ordre du travail SEO
- **Phase 4** : ton de voix (sortir de la voix de Claude)
- **Phase 5** : workflows (enchaîner, pas des tâches isolées)
- **Phase 6** : boucles (autonomie + apprentissage)
- **Phase 7** : passage à 1 (équipe d'IA juniors qui exécute)

### 4.3 Workflow de recherche de mots-clés « sans outil » ([2083201216960761955](https://x.com/Timseo_/status/2083201216960761955))
1. Créer du contexte avec de la data propriétaire
2. Identifier des signaux sociaux sur Reddit et X
3. Ajouter l'ensemble dans Obsidian
4. Lancer le workflow recherche de mots-clés sous Claude

### 4.4 Workflow d'audit SEO complet (50+ audits pour 20 €/mois) ([2088333331729350694](https://x.com/Timseo_/status/2088333331729350694))
- Phase 0 → audit site/SERP
- Phase 1 → quick wins
- Phase 2 → cannibalisation
- Phase 3 → clusters AEO
- Phase 4 → vecteurs sémantiques
- Phase 5 → maillage interne
- Phase 6 → briefs contenu
- Phase 7 → plan d'action 90 jours

### 4.5 Workflow cannibalisation ([2089743876244529215](https://x.com/Timseo_/status/2089743876244529215))
1. Lire l'export GSC 90 jours en entier (≈ 1 M tokens, aucun échantillon)
2. Isoler toutes les requêtes qui déclenchent 2+ URL
3. Classer le conflit (mot-clé exact / même intention / proximité sémantique)
4. Comparer position, impressions, clics, CTR des 2 pages
5. Décider l'action : 301, fusion, séparation des micro-intentions, **ou aucune action**
6. Règle : **301, pas 410**, pour préserver les liens acquis

### 4.6 Workflow maillage interne ([2083222405653114909](https://x.com/Timseo_/status/2083222405653114909) ; [2082139518673813616](https://x.com/Timseo_/status/2082139518673813616))
- Crawl/export GSC
- Claude lit tout
- Propose 60+ liens en 30 minutes
- Mapping visuel via un outil détourné d'un GitHub

### 4.7 Workflow Core Web Vitals ([2077366949785595919](https://x.com/Timseo_/status/2077366949785595919))
1. Récupérer le sitemap.xml
2. Lancer Lighthouse en local, **mobile** (mobile-first)
3. Mesurer les Core Web Vitals
4. Claude liste les problèmes techniques
5. Claude les corrige
6. Sortir les 5 pires pages avec plan d'action

### 4.8 Workflow audit sémantique ([2080348718839066635](https://x.com/Timseo_/status/2080348718839066635))
1. Lister les entités sémantiques attendues par Google sur la requête
2. Vérifier le lexique sémantique autour du mot-clé
3. Identifier les micro-intentions (pour le score RRF)
4. Ajouter de l'Information Gain
5. Scorer le contenu sur 100
6. Corriger Title/meta/Hn

### 4.9 Workflow citabilité LLM ([2091926256581587093](https://x.com/Timseo_/status/2091926256581587093))
1. Lire le texte en entier avec la requête cible et le type de page (jamais un extrait)
2. Noter 7 scores sur 100 : Surprise, Grounding, Content Effort, Alignement RRF, RAG Structurer, Freshness Guard (+ autres)
3. Compter les « preuves atomiques » (triplets [sujet] + [relation] + [valeur chiffrée]) — seuil 2/100 mots
4. Vérifier que la réponse arrive **dans les 30 mots** après chaque H2
5. Citer la phrase exacte pour chaque problème
6. Sortir le plan de réécriture en attaquant les 2 scores les plus bas

### 4.10 Astuce « ranker un mot-clé compétitif » ([2078088129366659301](https://x.com/Timseo_/status/2078088129366659301), 17 juil. 2026)
1. Choisir un mot-clé sur lequel tu n'as aucune chance de ranker avec ton site
2. Aller sur LinkedIn (ou YouTube)
3. Publier un post/vidéo optimisé sur ce mot-clé
4. Générer de l'engagement
5. Répéter

### 4.11 Procédure de lancement d'un site SEO (15 min) ([2082488568723976344](https://x.com/Timseo_/status/2082488568723976344) ; [2082742743613288874](https://x.com/Timseo_/status/2082742743613288874))
1. Claude génère la 1re version HTML
2. Itération section par section (jamais une page entière)
3. Indexer sur Google Search Console
4. Email pro sur Resend (100 emails/jour gratuits)

### 4.12 Stratégie « extension Chrome = SEO » ([2079149819046863023](https://x.com/Timseo_/status/2079149819046863023))
1. Découper chaque fonctionnalité du SaaS
2. Chaque fonctionnalité devient une extension Chrome
3. Chaque extension est un point d'entrée SEO indépendant
- 1re extension → 35 utilisateurs en quelques jours ([2080664801802408071](https://x.com/Timseo_/status/2080664801802408071))

### 4.13 Outils et méthodes « officiellement » cités

- **Claude** (Code, 20 €/mois) — outil principal ([2088520297364553960](https://x.com/Timseo_/status/2088520297364553960) ; [2091071624602939452](https://x.com/Timseo_/status/2091071624602939452))
- **Obsidian** — vault + RAG
- **ChromaDB** + **Sentence-Transformers** — indexation sémantique ([2085771177944125757](https://x.com/Timseo_/status/2085771177944125757))
- **Google Keyword Planner** — l'outil qu'il recommande encore (CPC + volume) ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069) ; [2079931721139544316](https://x.com/Timseo_/status/2079931721139544316))
- **Reddit Ask** ([2079931721139544316](https://x.com/Timseo_/status/2079931721139544316))
- **Grok + DeepSearch** ([2079931721139544316](https://x.com/Timseo_/status/2079931721139544316))
- **Google Search Console** — branchée directement sur Claude ([2073323429197943216](https://x.com/Timseo_/status/2073323429197943216), 4 juil. 2026 ; [20825200...](https://x.com/Timseo_/status/2086703171657932977))
- **Qadence.io** — son propre agent SEO SaaS (lancé 18 juin 2026) ([2067511329284563142](https://x.com/Timseo_/status/2067511329284563142) ; [20825200...](https://x.com/Timseo_/status/2086703171657932977))
- **Resend** — email transactionnel gratuit ([2083568085047636427](https://x.com/Timseo_/status/2083568085047636427))
- **Supabase** — collecte de données support client ([2085771177944125757](https://x.com/Timseo_/status/2085771177944125757))
- **Vite** + **`scripts/prerender.mjs`** — pour ses sites ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))
- **Next.js / Astro / Remix** — alternatives SSR/SSG ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))
- **Puppeteer / Playwright** — prerender headless ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))
- **Lighthouse** — Core Web Vitals local ([2077366949785595919](https://x.com/Timseo_/status/2077366949785595919))
- **Schema.org** — référentiel JSON-LD ([2079136005748359329](https://x.com/Timseo_/status/2079136005748359329))
- **launchd** (cron macOS local) ([2085771177944125757](https://x.com/Timseo_/status/2085771177944125757))
- **Substack** — newsletter longue ([2086721711978987528](https://x.com/Timseo_/status/2086721711978987528))

### 4.14 Outils SEO payants qu'il a arrêtés (liste indicative)
- Il annonce « depuis 2 ans, j'ai coupé tous mes abonnements SEO. Plus aucun outil payant. Tout passe par l'IA » ([2088292563153151525](https://x.com/Timseo_/status/2088292563153551525), 14 août 2026).
- Économie annoncée : « presque 200 € » par mois.
- Noms d'outils jamais cités directement dans les posts retenus (Semrush/Ahrefs/Majestic n'apparaissent pas dans les citations Timseo_ collectées). À noter : il recommande en revanche **GSC + Keyword Planner** comme seuls outils externes dignes d'intérêt.

---

## 5. Ce qu'il déconseille ou considère comme une erreur

| Erreur / « scam » | Post source |
|---|---|
| **Acheter des backlinks** | [2074011209620173307](https://x.com/Timseo_/status/2074011209620173307) ; [2070450497081774390](https://x.com/Timseo_/status/2070450497081774390) ; [2084886929833931130](https://x.com/Timseo_/status/2084886929833931130) ; [2093334188498006507](https://x.com/Timseo_/status/2093334188498006507) |
| **Payer 400 €/mois pour un site vitrine + une adresse mail** | [2083568085047636427](https://x.com/Timseo_/status/2083568085047636427) |
| **Créer 10 000 pages** | [2074011209620173307](https://x.com/Timseo_/status/2074011209620173307) |
| **Croire que le volume de mots-clés est important** | [2073344074648875261](https://x.com/Timseo_/status/2073344074648875261) (4 juil. 2026) |
| **Croire que ChatGPT est le grand gagnant du search IA** | [2074130495567532339](https://x.com/Timseo_/status/2074130495567532339) (6 juil. 2026) |
| **Copier les concurrents** (vs chercher son angle) | [2074130495567532339](https://x.com/Timseo_/status/2074130495567532339) |
| **Publier un article de blog au départ** (AI Overviews mangent l'info) | [2075247650723787097](https://x.com/Timseo_/status/2075247650723787097) (9 juil. 2026) |
| **Vouloir automatiser son SEO avant d'avoir ranké un seul site** | [2092544399603613796](https://x.com/Timseo_/status/2092544399603613796) (26 août 2026) |
| **Se reposer sur les outils SEO classiques** (« data quasi devenue obsolète ») | [2070580100979114069](https://x.com/Timseo_/status/2070580100979114069) |
| **Suivre le « rank moyen » comme KPI** | [2086053157982126505](https://x.com/Timseo_/status/2086053157982126505) |
| **Utiliser un code HTTP 410 au lieu d'un 301** pour une page cannibalisée | [2089743876244529215](https://x.com/Timseo_/status/2089743876244529215) |
| **Faire un site SPA pure sans prerender** (non crawlable) | [2087203754324242918](https://x.com/Timseo_/status/2087203754324242918) |
| **Utiliser un schéma JSON-LD qui ne correspond pas au contenu visible** | [2087203754324242918](https://x.com/Timseo_/status/2087203754324242918) |
| **Construire un projet SEO avec ChatGPT/Claude sans data propriétaire, sans Obsidian, sans audit mensuel, sans boucles d'apprentissage** | [2079227329616941500](https://x.com/Timseo_/status/2079227329616941500) |
| **Faire une page de 2 000 mots pour répondre à une intention unique** (cf. phrase dans une réponse : « les pages doivent répondre à l'intention seule ») | [2093538244717957522](https://x.com/Timseo_/status/2093538244717957522) |
| **Penser que Claude peut remplacer un consultant SEO seul** (« il en faudra un peu plus ») | [2093359702167990783](https://x.com/Timseo_/status/2093359702167990783) (28 août 2026) |
| **Trop produire « pour produire » sous prétexte d'IA** | [2090760827003355542](https://x.com/Timseo_/status/2090760827003355542) (21 août 2026) |
| **Penser qu'avoir 9 999 mots-clés rankés suffit** (« 50 mots-clés au cœur du business ») | [2070580100979114069](https://x.com/Timseo_/status/2070580100979114069) |

---

## 6. Tests, expériences, études de cas

### 6.1 Cas client « Golfiller / balle de golf » (référencé 4 fois)

- **Résultat** : top 1 sur « balle de golf » (6 000 recherches/mois) devant Décathlon ([2092300598851100709](https://x.com/Timseo_/status/2092300598851100709) ; [2094097061012541844](https://x.com/Timseo_/status/2094097061012541844)).
- **Méthode déclarée** :
  - Ne pas attaquer le mot-clé principal de front → construire une **autorité thématique** sur une verticale gagnable (« balle de golf d'occasion »).
  - **Programmatique** : un template = une variable = des centaines de pages.
  - Cibles : **intentions « Do »** (calculer, comparer, consulter) et non « Know » (lire).
  - **Nourrir les pages de data propriétaire**.
- **Précision importante** (post 31 août 2026) : « on a dit sans achat de BL, pas sans BL. Le site a des BL, mais de mon côté c'est une presta avec 0 BL ni achat ni BL tout court en 2 ans » ([2094407438602739747](https://x.com/Timseo_/status/2094407438602739747)). Le résultat est présenté comme **valable** (top 1) mais le cas est **mixte** (BL organiques présents, pas d'achat).
- **Conclusion Timseo_** : « c'est la fin du trafic pour le trafic. SEO redevient un véritable canal d'acquisition ».
- ⚠️ *Caveat lecture* : corrélation rapportée par l'auteur, pas une démonstration causale indépendante.

### 6.2 Cas client « coach sportif » (20 leads → 10 leads)
- Observation : leads divisés par 2 en 1 an, **sans changement SEO** ([2081787701146320898](https://x.com/Timseo_/status/2081787701146320898), 27 juil. 2026).
- Conclusion Timseo_ : « les LLM mangent les clics informationnels » — exemple typique de « trafic de vanité ».

### 6.3 Test « score de citabilité LLM » ([2091926256581587093](https://x.com/Timseo_/status/2091926256581587093))
- Score 7 dimensions sur 100.
- Seuil empirique : 2 preuves atomiques / 100 mots.
- Règle 30 mots après H2 → test retriever RAG.
- Conclusion : « j'itère dessus depuis 6 ans, 1000+ articles et 100+ projets SEO » → c'est de l'expérience accumulée, **pas un test A/B contrôlé**.

### 6.4 Test « cannibalisation automatique » ([2089743876244529215](https://x.com/Timseo_/status/2089743876244529215))
- Workflow détaillé export GSC 90 jours.
- Conclusion : « 62 liens en 30 minutes » sur son site ; « 3 heures de maillage manuel » remplacé.
- *Caveat* : gain de temps, pas un gain de ranking prouvé.

### 6.5 Test « premier audit site/serp » ([2082313566250799324](https://x.com/Timseo_/status/2082313566250799324))
- Audit d'indexation hebdomadaire via Claude (404, sitemap).
- Conclusion : il évite l'oubli et externalise l'exécution — pas de chiffre de ranking.

### 6.6 Mesure GEO = 3 % du trafic ([2070043197590688233](https://x.com/Timseo_/status/2070043197590688233))
- Daté juin 2026, mesure personnelle.
- Conclusion : GEO est encore marginal, mais Google en a fait une fonctionnalité GSC, donc le mouvement est lancé.

### 6.7 Répartition mondiale des visites LLM ([2072593509417414688](https://x.com/Timseo_/status/2072593509417414688), 2 juil. 2026)
- Source citée : Similarweb.
- Chiffres relayés : ChatGPT 54,7 % ; Google Gemini 27,4 % ; Claude 8,2 % ; DeepSeek 4,1 % ; Grok 2,8 % ; Perplexity (chiffre coupé).
- Conclusion : pour la **distribution**, ChatGPT domine encore, mais le maillage SEO classique reste pertinent.

### 6.8 Résultat extensions Chrome
- 1re extension : **35 utilisateurs + 1 avis en 14 jours** ([2080664801802408071](https://x.com/Timseo_/status/2080664801802408071)).
- Stratégie en cours de validation (« on va voir si la stratégie SEO extension fonctionne dans les prochains mois »).

### 6.9 Produit SEOCity (gamification de site SEO)
- 24h après lancement : plusieurs villes créées ([2092898411762925907](https://x.com/Timseo_/status/2092898411762925907), 27 août 2026).
- 5 jours après : **+358 villes créées, 1 620 visites** ([2094463515415474338](https://x.com/Timseo_/status/2094463515415474338)).
- Conclusion : preuve d'engagement early-stage, pas de SEO résultat à ce stade.

### 6.10 « Reprise vieux projet 2023 » ([2087170922436542852](https://x.com/Timseo_/status/2087170922436542852), 11 août 2026)
- Démarré en 2023, stoppé pour se consacrer au freelance.
- Reprise via IA. Résultats partiels, suite à venir.

### 6.11 Retour Substack
- **5 000 abonnés** en 4 ans, **jamais monétisé** ([2094322294323597812](https://x.com/Timseo_/status/2094322294323597812)).
- Conclusion : « c'est de loin mon meilleur canal d'acquisition pour vendre mes services SEO ».

---

## 7. Évolutions, nuances, contradictions

### 7.1 Chronologie observable des positions
- **Juin 2025** ([2067511329284563142](https://x.com/Timseo_/status/2067511329284563142)) : lancement de Qadence — liste statique de features agent (recherche KW, maillage, cannibalisation, brief, cluster AEO, programmatique, sémantique, quick wins, audit GEO, schémas, Core Web Vitals).
- **Juin 2025 → mi-juillet 2025** ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069) ; [2070580100979114069](https://x.com/Timseo_/status/2070580100979114069)) : « 10 principes SEO » — encore dans un cadre « SEO classique » (position moyenne, volume, backlinks comme signaux remplacés par signaux sociaux).
- **9 juillet 2025** ([2075179658706895230](https://x.com/Timseo_/status/2075179658706895230)) : « c'est la fin des mots-clés » — bascule sémantique/IA assumée.
- **Mi-juillet → fin juillet 2025** : structuration du système (Claude + Obsidian + RAG + 27 automatisations).
- **Début août 2025** ([2082483283716366801](https://x.com/Timseo_/status/2082483283716366801)) : intégration des réseaux sociaux dans GSC → il parle de « bascule ».
- **Mi-août 2025** ([2088292563153151525](https://x.com/Timseo_/status/2088292563153551525)) : « j'ai coupé tous mes abonnements SEO » — bascule outillée assumée.
- **Fin août 2025** ([2093359702167990783](https://x.com/Timseo_/status/2093359702167990783) ; [2093538244717957522](https://x.com/Timseo_/status/2093538244717957522)) : « Claude ne remplace pas un consultant seul » et « pages doivent répondre à l'intention seule, pas de guide 2000 mots » — **premières nuances publiques** sur la tentation de tout déléguer à l'IA.

### 7.2 Contradictions / tensions apparentes

| Tension | Lecture |
|---|---|
| **« Construire 10 000 pages c'est nul »** ([2074011209620173307](https://x.com/Timseo_/status/2074011209620173307)) **vs** **« Programmatique = centaines de pages »** ([2094097061012541844](https://x.com/Timseo_/status/2094097061012541844)) | Il distingue le spam programmatique (« 10 000 pages de mauvaise qualité ») du programmatique de qualité (« 1 template + 1 variable + data propriétaire »). C'est une **nuance**, pas une vraie contradiction. |
| **« Google Keyword Planner est le meilleur outil »** ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069)) **vs** **« data des outils SEO quasi obsolète »** ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069)) | Il recommande GKP pour le **CPC et le volume** (signaux que l'IA ne fournit pas), pas pour la stratégie globale. Cohérent. |
| **« E-E-A-T = cas clients + avis clients »** ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069)) **vs** absence de discussion sur les signaux E-E-A-T plus tard (Person schema, author bio, etc.) | Il **cite E-E-A-T** comme formulation mais ne développe pas les détails techniques ailleurs — possible angle mort public. |
| **« 5 requêtes stratégiques > 100 mots-clés »** ([2092300598851100709](https://x.com/Timseo_/status/2092300598851100709)) **vs** **« 50 mots-clés cœur de business »** ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069)) | 5 « requêtes stratégiques » regroupent chacune plusieurs mots-clés cœur ; cohérent. |
| **« LinkedIn en top 3 sites externes »** ([2083533202065445266](https://x.com/Timseo_/status/2083533202065445266)) **vs** **« YouTube + LinkedIn »** comme meilleure strat 2026 ([2070049889581715518](https://x.com/Timseo_/status/2070049889581715518)) | Pas de contradiction : il classe les 6 plateformes par utilité et précise ensuite la combo gagnante. |
| **« Construire des pages pour humains ET robots »** ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069)) **vs** **« 30 mots après H2 sinon le retriever ne l'associe pas »** ([2091926256581587093](https://x.com/Timseo_/status/2091926256581587093)) | Complémentaire : le format « robots » n'est pas contradictoire avec la lisibilité humaine si on structure bien. |
| **« GEO = 3 % du trafic »** ([2070043197590688233](https://x.com/Timseo_/status/2070043197590688233)) **vs** **« GEO n'est pas du scam, Google le prend très au sérieux »** ([2075475609447510389](https://x.com/Timseo_/status/2075475609447510389)) | Nuance temporelle : faible part de marché, mais signal structurel fort → investir maintenant. |

### 7.3 Évolution dans la maturité des conseils
- **Phase 1 (juin 2025)** : promesses, arborescences, « voici mon agent ». Tone plus promotionnel.
- **Phase 2 (juillet 2025)** : détails workflows, premiers retours chiffrés (62 liens / 30 min, 3 audits/mois).
- **Phase 3 (août 2025)** : retours d'expérience clients, distinctions fines (sans spam vs spam programmatique), premières limites assumées (Claude ne remplace pas tout).

---

## 8. Checklist SEO dérivée uniquement de ses conseils

> Chaque ligne est rattachable à au moins un post du corpus. Aucun ajout SEO général non sourcé.

### Cadrage stratégique
- [ ] **Choisir une niche ultra-spécifique** où l'on peut gagner ([2078452818516873416](https://x.com/Timseo_/status/2078452818516873416))
- [ ] **Identifier 3 à 5 mots-clés business** ([2074011209620173307](https://x.com/Timseo_/status/2074011209620173307))
- [ ] **Ne pas chercher à se positionner sur 1 500 mots-clés** ([2089384759948357958](https://x.com/Timseo_/status/2089384759948357958))
- [ ] **Viser l'autorité thématique** sur une verticale précise ([2092300598851100709](https://x.com/Timseo_/status/2092300598851100709))
- [ ] **Cibler les requêtes « Do »** (calculer, comparer, demander démo, acheter) ([2092300598851100709](https://x.com/Timseo_/status/2092300598851100709))

### Recherche de mots-clés
- [ ] **Google Keyword Planner** pour CPC + volume ([2079931721139544316](https://x.com/Timseo_/status/2079931721139544316))
- [ ] **Reddit Ask** pour les intentions réelles ([2079931721139544316](https://x.com/Timseo_/status/2079931721139544316))
- [ ] **Grok + DeepSearch** pour signaux utilisateurs ([2079931721139544316](https://x.com/Timseo_/status/2079931721139544316))
- [ ] **Stocker la data propriétaire dans Obsidian** ([2083201216960761955](https://x.com/Timseo_/status/2083201216960761955))
- [ ] **Identifier les mots-clés décisionnels vs informationnels** ([2082848692176830871](https://x.com/Timseo_/status/2082848692176830871))
- [ ] **Identifier les « mots-clés overview »** (déclenchant des AI Overviews) ([2082848692176830871](https://x.com/Timseo_/status/2082848692176830871))
- [ ] **Lister 10 micro-intentions** par mot-clé business via Claude ([2078452818516873416](https://x.com/Timseo_/status/2078452818516873416))

### Architecture & silos
- [ ] **Chaîne** : mot-clé business → longue traîne → vecteurs sémantiques → micro-intentions → univers sémantique ([2086851567693791312](https://x.com/Timseo_/status/2086851567693791312))
- [ ] **1 à 15 pages par requête stratégique** ([2092300598851100709](https://x.com/Timseo_/status/2092300598851100709))
- [ ] **Templates pSEO** : 1 template = 1 variable = plusieurs centaines de pages ([2081765303273627867](https://x.com/Timseo_/status/2081765303273627867))
- [ ] **Pages alternatives** : Alternatives à X / gratuite / française ([2085987057223028937](https://x.com/Timseo_/status/2085987057223028937))
- [ ] **Directories** : prix, tendances, comparatifs, produits ([2092300598851100709](https://x.com/Timseo_/status/2092300598851100709))

### Production de contenu
- [ ] **Cas d'usage, comparatifs, réponses aux objections, contenus d'expertise, data propriétaire** ([2092300598851100709](https://x.com/Timseo_/status/2092300598851100709))
- [ ] **Pas d'article de blog au départ** si AI Overview = 9/10 sur l'intention ([2075247650723787097](https://x.com/Timseo_/status/2075247650723787097))
- [ ] **FAQ ultra-complètes** à partir des vraies questions Reddit/X ([2074011209620173307](https://x.com/Timseo_/status/2074011209620173307))
- [ ] **E-E-A-T = cas clients + avis clients** ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069))
- [ ] **Outil IA / simulateur** intégré pour capter l'email ([2070580100979114069](https://x.com/Timseo_/status/2070580100979114069))
- [ ] **Sortir de la voix de Claude** via un skill ton de voix ([2087568290612949463](https://x.com/Timseo_/status/2087568290612949463))

### Maillage interne
- [ ] **À déléguer à Claude** (avec ou sans export GSC) ([2079136005748359329](https://x.com/Timseo_/status/2079136005748359329))
- [ ] **Skill `maillage-systeme`** ([2081765303273627867](https://x.com/Timseo_/status/2081765303273627867))
- [ ] **Mapping visuel** ([2082139518673813616](https://x.com/Timseo_/status/2082139518673813616))

### Cannibalisation
- [ ] **Audit via export GSC 90 jours entier** ([2089743876244529215](https://x.com/Timseo_/status/2089743876244529215))
- [ ] **Classifier** : mot-clé exact / même intention / proximité ([2089743876244529215](https://x.com/Timseo_/status/2089743876244529215))
- [ ] **Si 2 pages en top 10** : garder les 2, écrire 2 angles distincts ([2089743876244529215](https://x.com/Timseo_/status/2089743876244529215))
- [ ] **301, jamais 410** ([2089743876244529215](https://x.com/Timseo_/status/2089743876244529215))

### Technique & performance
- [ ] **Pas de SPA pure** : prerender post-build / SSR-SSG / prerender headless ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))
- [ ] **`sitemap.xml` auto-généré** depuis les routes ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))
- [ ] **`robots.txt`** pointe vers le sitemap ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))
- [ ] **Vrai `404.html`** retournant un 404 ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))
- [ ] **`<title>` et `<meta description>` uniques** par page ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))
- [ ] **Un seul `<h1>`** par page ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))
- [ ] **Canonical explicite** par route ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))
- [ ] **Open Graph + Twitter Card** ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))
- [ ] **Lazy-load images** avec `width`/`height` explicites ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))
- [ ] **Polices `font-display: swap`** ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))
- [ ] **Lighthouse mobile** pour Core Web Vitals ([2077366949785595919](https://x.com/Timseo_/status/2077366949785595919))
- [ ] **Audit d'indexation hebdo** automatisé ([2075310521146867897](https://x.com/Timseo_/status/2075310521146867897))

### Données structurées
- [ ] **JSON-LD via Claude** ([2079136005748359329](https://x.com/Timseo_/status/2079136005748359329))
- [ ] **Schéma uniquement si visible** sur la page ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))
- [ ] **Organization/WebSite** sur la home, **Article** sur les posts, **FAQPage** seulement si FAQ présente ([2087203754324242918](https://x.com/Timseo_/status/2087203754324242918))

### Signaux sociaux
- [ ] **Présence YouTube, Reddit, LinkedIn, X, Substack, Pinterest** ([2083533202065445266](https://x.com/Timseo_/status/2083533202065445266))
- [ ] **Strat « mots-clés compétitifs »** : LinkedIn/YouTube + engagement + itération ([2082113849705345533](https://x.com/Timseo_/status/2082113849705345533))
- [ ] **Strat « extension Chrome »** : 1 fonctionnalité SaaS = 1 extension ([2079149819046863023](https://x.com/Timseo_/status/2079149819046863023))

### GEO / AEO
- [ ] **Score 7 dimensions** sur 100 (Surprise, Grounding, Content Effort, RRF, RAG Structurer, Freshness Guard…) ([2091926256581587093](https://x.com/Timseo_/status/2091926256581587093))
- [ ] **2 preuves atomiques / 100 mots** minimum ([2091926256581587093](https://x.com/Timseo_/status/2091926256581587093))
- [ ] **Réponse dans les 30 mots après chaque H2** ([2091926256581587093](https://x.com/Timseo_/status/2091926256581587093))
- [ ] **Pages courtes, intention unique** ([2093538244717957522](https://x.com/Timseo_/status/2093538244717957522))

### Audit complet
- [ ] **7 phases** : audit site/serp → quick wins → cannibalisation → clusters AEO → vecteurs sémantiques → maillage → briefs → plan 90 jours ([2088333331729350694](https://x.com/Timseo_/status/2088333331729350694))

### Métriques
- [ ] **Suivre** : proximité de l'offre, intention d'achat, CPC, faisabilité ranking, capacité à récupérer un email, score RRF ([2086703171657932977](https://x.com/Timseo_/status/2086703171657932977))
- [ ] **Ne PAS suivre** : trafic, volume, nombre de BL, position moyenne ([2086703171657932977](https://x.com/Timseo_/status/2086703171657932977) ; [2086053157982126505](https://x.com/Timseo_/status/2086053157982126505))

### Système d'outillage personnel
- [ ] **Claude Code** + **Obsidian** + **RAG** (ChromaDB + Sentence-Transformers) ([2088292563153151525](https://x.com/Timseo_/status/2088292563153551525))
- [ ] **Structure Karpathy** `raw/` + `wiki/` ([2084644273543422325](https://x.com/Timseo_/status/2084644273543422325))
- [ ] **`AGENTS.md`** racine ([2084644273543422325](https://x.com/Timseo_/status/2084644273543422325))
- [ ] **Wikilinks Obsidian** partout ([2084644273543422325](https://x.com/Timseo_/status/2084644273543422325))
- [ ] **27 automatisations** : revue de presse SEO, audit indexation mensuel, citation IA hebdo, GSC, vérif. hebdo des scripts ([2088292563153151525](https://x.com/Timseo_/status/2088292563153551525))

### Garde-fous
- [ ] **Ne pas acheter de backlinks** ([2093334188498006507](https://x.com/Timseo_/status/2093334188498006507))
- [ ] **Ne pas automatiser son SEO avant d'avoir ranké au moins un site** ([2092544399603613796](https://x.com/Timseo_/status/2092544399603613796))
- [ ] **Ne pas remplacer un consultant SEO par Claude seul** ([2093359702167990783](https://x.com/Timseo_/status/2093359702167990783))
- [ ] **Ne pas produire « pour produire »** ([2090760827003355542](https://x.com/Timseo_/status/2090760827003355542))
- [ ] **Ne pas publier d'article blog sur des requêtes informationnelles dominées par AI Overviews** ([2075247650723787097](https://x.com/Timseo_/status/2075247650723787097))
- [ ] **Audit système au moins 1×/mois** ([2079227329616941500](https://x.com/Timseo_/status/2079227329616941500))

---

## 9. Index des sources (publications Timseo_ utilisées)

> Liste non exhaustive mais représentative de tout ce qui a nourri le rapport. Format : date UTC | URL | sujet principal.

### Juin 2026
- 2026-06-13 — [2065677682587959721](https://x.com/Timseo_/status/2065677682587959721) — position sur Claude vs hausse des prix
- 2026-06-18 — [2067511329284563142](https://x.com/Timseo_/status/2067511329284563142) — lancement Qadence, liste des features agent
- 2026-06-22 — [2068930756794335657](https://x.com/Timseo_/status/2068930756794335657) — site vibecodé 100 % Claude
- 2026-06-25 — [2070049889581715518](https://x.com/Timseo_/status/2070049889581715518) — strat SEO 2026 = SEO + LinkedIn + YouTube
- 2026-06-25 — [2070043197590688233](https://x.com/Timseo_/status/2070043197590688233) — GEO = 3 % du trafic (mesure perso)
- 2026-06-26 — [2070403100733759693](https://x.com/Timseo_/status/2070403100733759693) — Claude remplace les designers
- 2026-06-26 — [2070450497081774390](https://x.com/Timseo_/status/2070450497081774390) — pas besoin d'acheter des BL
- 2026-06-26 — [2070481813202743532](https://x.com/Timseo_/status/2070481813202743532) — comparaison SEO tools
- 2026-06-26 — [2070580100979114069](https://x.com/Timseo_/status/2070580100979114069) — 10 principes SEO 2026 (volume vs E-E-A-T, BL remplacés par signaux sociaux, etc.)
- 2026-06-27 — [2070770370559582524](https://x.com/Timseo_/status/2070770370559582524) — Claude vs autres modèles

### Juillet 2026
- 2026-07-01 — [2072198016426291535](https://x.com/Timseo_/status/2072198016426291535) — article long
- 2026-07-02 — [2072593509417414688](https://x.com/Timseo_/status/2072593509417414688) — répartition mondiale LLM
- 2026-07-03 — [2072891212600885294](https://x.com/Timseo_/status/2072891212600885294) — critique des consultants GEO
- 2026-07-04 — [2073323429197943216](https://x.com/Timseo_/status/2073323429197943216) — GSC connectée à Claude
- 2026-07-04 — [2073344074648875261](https://x.com/Timseo_/status/2073344074648875261) — fin du volume comme KPI
- 2026-07-04 — [2073388963688312963](https://x.com/Timseo_/status/2073388963688312963) — app Reddit playbook
- 2026-07-04 — [2073397455627120841](https://x.com/Timseo_/status/2073397455627120841) — site full Claude, full HTML, pas de CMS
- 2026-07-04 — [2073405391946576323](https://x.com/Timseo_/status/2073405391946576323) — anti-patterns IA, demander à ChatGPT la liste
- 2026-07-04 — [2073405538189344935](https://x.com/Timseo_/status/2073405538189344935) — exemples de sites full Claude
- 2026-07-06 — [2074011209620173307](https://x.com/Timseo_/status/2074011209620173307) — couverture 3-5 mots-clés + FAQ Reddit/X
- 2026-07-06 — [2074030748303270361](https://x.com/Timseo_/status/2074030748303270361) — animations full Claude
- 2026-07-06 — [2074130495567532339](https://x.com/Timseo_/status/2074130495567532339) — 23 trucs SEO à arrêter
- 2026-07-07 — [2074465917866823746](https://x.com/Timseo_/status/2074465917866823746) — vidéos promp Claude
- 2026-07-08 — [2074800158043419050](https://x.com/Timseo_/status/2074800158043419050) — groupe privé GEO
- 2026-07-09 — [2075179658706895230](https://x.com/Timseo_/status/2075179658706895230) — fin des mots-clés en SEO, 3 arguments
- 2026-07-09 — [2075247650723787097](https://x.com/Timseo_/status/2075247650723787097) — ne pas publier d'article blog au départ
- 2026-07-09 — [2075310521146867897](https://x.com/Timseo_/status/2075310521146867897) — audit indexation hebdo via Claude
- 2026-07-10 — [2075475609447510389](https://x.com/Timseo_/status/2075475609447510389) — GEO pas un scam
- 2026-07-10 — [2075501411979481495](https://x.com/Timseo_/status/2075501411979481495) — « les clients disent GEO donc go GEO »
- 2026-07-11 — [2075870701618376710](https://x.com/Timseo_/status/2075870701618376710) — extensions Chrome créées via Claude
- 2026-07-13 — [2076594229464494480](https://x.com/Timseo_/status/2076594229464494480) — app tracking via Claude
- 2026-07-15 — [2077366949785595919](https://x.com/Timseo_/status/2077366949785595919) — audit Core Web Vitals via Claude
- 2026-07-16 — [2077703489145475371](https://x.com/Timseo_/status/2077703489145475371) — article long
- 2026-07-16 — [2077773751593443784](https://x.com/Timseo_/status/2077773751593443784) — UX/UI full Claude
- 2026-07-17 — [2078088129366659301](https://x.com/Timseo_/status/2078088129366659301) — ranker mot-clé compétitif via LinkedIn
- 2026-07-18 — [2078452818516873416](https://x.com/Timseo_/status/2078452818516873416) — niche + data + 3-5 mots-clés + 10 micro-intentions
- 2026-07-20 — [2079136005748359329](https://x.com/Timseo_/status/2079136005748359329) — SEO technique délégable à 100 % IA
- 2026-07-20 — [2079149819046863023](https://x.com/Timseo_/status/2079149819046863023) — strat extensions Chrome
- 2026-07-20 — [2079181033937961142](https://x.com/Timseo_/status/2079181033937961142) — règles portefeuille 10 sites / 25 k clics
- 2026-07-20 — [2079227329616941500](https://x.com/Timseo_/status/2079227329616941500) — 6 règles projet SEO + Claude/Obsidian
- 2026-07-21 — [2079559520418693429](https://x.com/Timseo_/status/2079559520418693429) — extension Chrome Google Search Console
- 2026-07-22 — [2079898498926047365](https://x.com/Timseo_/status/2079898498926047365) — logos via Claude
- 2026-07-22 — [2079931721139544316](https://x.com/Timseo_/status/2079931721139544316) — 5 sources de mots-clés (GKP, Reddit, Grok, data proprio, GSC)
- 2026-07-22 — [2079940781134012839](https://x.com/Timseo_/status/2079940781134012839) — pas besoin de hacks pour ranker
- 2026-07-22 — [2079956619975364680](https://x.com/Timseo_/status/2079956619975364680) — rapprochements data pour Claude
- 2026-07-23 — [2080348718839066635](https://x.com/Timseo_/status/2080348718839066635) — audit sémantique via Claude
- 2026-07-24 — [2080632841944064159](https://x.com/Timseo_/status/2080632841944064159) — maillage interne via Claude
- 2026-07-24 — [2080664801802408071](https://x.com/Timseo_/status/2080664801802408071) — extension Chrome 35 utilisateurs
- 2026-07-27 — [2081708176714645944](https://x.com/Timseo_/status/2081708176714645944) — pourquoi tout le monde perd du trafic
- 2026-07-27 — [2081765303273627867](https://x.com/Timseo_/status/2081765303273627867) — arborescence complète agent SEO
- 2026-07-27 — [2081787701146320898](https://x.com/Timseo_/status/2081787701146320898) — cas coach sportif (20 → 10 leads)
- 2026-07-28 — [2082113849705345533](https://x.com/Timseo_/status/2082113849705345533) — astuce mots-clés compétitifs sur LinkedIn/YouTube
- 2026-07-28 — [2082139518673813616](https://x.com/Timseo_/status/2082139518673813616) — mapping visuel maillage
- 2026-07-29 — [2082313566250799324](https://x.com/Timseo_/status/2082313566250799324) — audit SEO via agent
- 2026-07-29 — [2082462766313746853](https://x.com/Timseo_/status/2082462766313746853) — article long
- 2026-07-29 — [2082483283716366801](https://x.com/Timseo_/status/2082483283716366801) — réseaux sociaux dans GSC
- 2026-07-29 — [2082488568723976344](https://x.com/Timseo_/status/2082488568723976344) — site SEO 15 min Claude
- 2026-07-30 — [2082742743613288874](https://x.com/Timseo_/status/2082742743613288874) — site 20 min avec Claude
- 2026-07-30 — [2082824670521471382](https://x.com/Timseo_/status/2082824670521471382) — article long
- 2026-07-30 — [2082848692176830871](https://x.com/Timseo_/status/2082848692176830871) — arborescence agent mots-clés
- 2026-07-31 — [2083080579709538547](https://x.com/Timseo_/status/2083080579709538547) — article long
- 2026-07-31 — [2083201216960761955](https://x.com/Timseo_/status/2083201216960761955) — recherche de mots-clés sans outil
- 2026-07-31 — [2083222405653114909](https://x.com/Timseo_/status/2083222405653114909) — 62 liens maillage en 30 min

### Août 2026
- 2026-08-01 — [2083533202065445266](https://x.com/Timseo_/status/2083533202065445266) — Top 6 sites externes (YouTube, Reddit, LinkedIn, X, Substack, Pinterest)
- 2026-08-01 — [2083568085047636427](https://x.com/Timseo_/status/2083568085047636427) — 400 €/mois = scam vs Claude + Resend
- 2026-08-03 — [2084209592494366901](https://x.com/Timseo_/status/2084209592494366901) — strat vidéos YouTube
- 2026-08-04 — [2084644273543422325](https://x.com/Timseo_/status/2084644273543422325) — Karpathy raw/wiki, AGENTS.md, wikilinks
- 2026-08-05 — [2084886929833931130](https://x.com/Timseo_/status/2084886929833931130) — « No need BL to rank, SEO myth »
- 2026-08-05 — [2084941404623843524](https://x.com/Timseo_/status/2084941404623843524) — article long
- 2026-08-05 — [2085033589172023463](https://x.com/Timseo_/status/2085033589172023463) — skill Claude « mots-clés mangés par IA »
- 2026-08-06 — [2085368294882590801](https://x.com/Timseo_/status/2085368294882590801) — 90 % du SEO = discussion terminal + Claude + Obsidian
- 2026-08-07 — [2085652558257762664](https://x.com/Timseo_/status/2085652558257762664) — projet business SEO vidéo
- 2026-08-07 — [2085676575563927632](https://x.com/Timseo_/status/2085676575563927632) — SEO = jeu de long terme
- 2026-08-07 — [2085771177944125757](https://x.com/Timseo_/status/2085771177944125757) — arborescence complète système SEO
- 2026-08-08 — [2085987057223028937](https://x.com/Timseo_/status/2085987057223028937) — idées pages SEO pour SaaS
- 2026-08-08 — [2086053157982126505](https://x.com/Timseo_/status/2086053157982126505) — rank moyen = KPI à ne pas suivre
- 2026-08-08 — [2086055991779700837](https://x.com/Timseo_/status/2086055991779700837) — trouver mots-clés IA-résistants + data propriétaire
- 2026-08-10 — [2086703171657932977](https://x.com/Timseo_/status/2086703171657932977) — nouveaux KPI SEO
- 2026-08-10 — [2086721711978987528](https://x.com/Timseo_/status/2086721711978987528) — focus 4 réseaux
- 2026-08-10 — [2086795212228292841](https://x.com/Timseo_/status/2086795212228292841) — BL sans achat
- 2026-08-10 — [2086828018136404071](https://x.com/Timseo_/status/2086828018136404071) — projet RAG sous Obsidian
- 2026-08-10 — [2086851567693791312](https://x.com/Timseo_/status/2086851567693791312) — fin des mots-clés, sémantique + univers
- 2026-08-11 — [2087170922436542852](https://x.com/Timseo_/status/2087170922436542852) — reprise vieux projet 2023
- 2026-08-11 — [2087203754324242918](https://x.com/Timseo_/status/2087203754324242918) — checklist base technique site Claude
- 2026-08-12 — [2087428004591071724](https://x.com/Timseo_/status/2087428004591071724) — communauté SEO « ultra toxique »
- 2026-08-12 — [2087568290612949463](https://x.com/Timseo_/status/2087568290612949463) — guide complet agent SEO Claude (7 phases)
- 2026-08-13 — [2087937588607045892](https://x.com/Timseo_/status/2087937588607045892) — 20 templates de pages alternatives/intégration
- 2026-08-14 — [2088292563153151525](https://x.com/Timseo_/status/2088292563153551525) — 66 procédures + RAG 1528 notes + 281 faits + 27 automatisations
- 2026-08-14 — [2088333331729350694](https://x.com/Timseo_/status/2088333331729350694) — 50+ audits SEO via Claude, 7 phases
- 2026-08-15 — [2088520297364553960](https://x.com/Timseo_/status/2088520297364553960) — SEO = un abonnement Claude
- 2026-08-15 — [2088586553702691249](https://x.com/Timseo_/status/2088586553702691249) — Claude + RAG + Obsidian (jamais Claude seul)
- 2026-08-17 — [2089262705626755218](https://x.com/Timseo_/status/2089262705626755218) — 5 sujets business + automatiser SEO technique
- 2026-08-17 — [2089282716378489155](https://x.com/Timseo_/status/2089282716378489155) — article long
- 2026-08-17 — [2089384759948357958](https://x.com/Timseo_/status/2089384759948357958) — 7 conseils SEO pour économiser en ads
- 2026-08-18 — [2089598455295754640](https://x.com/Timseo_/status/2089598455295754640) — passer de 250 €/mois outils à Claude + Obsidian
- 2026-08-18 — [2089743876244529215](https://x.com/Timseo_/status/2089743876244529215) — détection cannibalisation + workflow 301
- 2026-08-19 — [2090001205812724106](https://x.com/Timseo_/status/2090001205812724106) — article long
- 2026-08-21 — [2090760827003355542](https://x.com/Timseo_/status/2090760827003355542) — piège « produire pour produire »
- 2026-08-22 — [2091071624602939452](https://x.com/Timseo_/status/2091071624602939452) — site lancé le 10 août
- 2026-08-22 — [2091182665269698941](https://x.com/Timseo_/status/2091182665269698941) — consultants sous Claude + Obsidian (3 arguments)
- 2026-08-22 — [2091211043448222172](https://x.com/Timseo_/status/2091211043448222172) — 4 prompts pour trouver clients sur Google
- 2026-08-24 — [2091854786933166301](https://x.com/Timseo_/status/2091854786933166301) — article long
- 2026-08-24 — [2091926256581587093](https://x.com/Timseo_/status/2091926256581587093) — score citabilité LLM (7 dimensions)
- 2026-08-24 — [2091981941272662187](https://x.com/Timseo_/status/2091981941272662187) — citation (Laurent) « l'onglet performance GSC dit la vérité »
- 2026-08-25 — [2092300598851100709](https://x.com/Timseo_/status/2092300598851100709) — cas Golfiller : 5 requêtes stratégiques + intentions Do
- 2026-08-26 — [2092484280035557770](https://x.com/Timseo_/status/2092484280035557770) — « Decathlon a le meilleur SEO »
- 2026-08-26 — [2092537872360612333](https://x.com/Timseo_/status/2092537872360612333) — « not local SEO »
- 2026-08-26 — [2092544399603613796](https://x.com/Timseo_/status/2092544399603613796) — automatiser SEO avant d'avoir ranké = non
- 2026-08-26 — [2092544623587791336](https://x.com/Timseo_/status/2092544623587791336) — qadence.io scrape GSC auto
- 2026-08-26 — [2092590382488101351](https://x.com/Timseo_/status/2092590382488101351) — lancement SEOCity
- 2026-08-26 — [2092623155311567334](https://x.com/Timseo_/status/2092623155311567334) — qadence.io vs GSC gratuit
- 2026-08-27 — [2092898411762925907](https://x.com/Timseo_/status/2092898411762925907) — Top villes SEOCity 24h
- 2026-08-27 — [2092922822855205349](https://x.com/Timseo_/status/2092922822855205349) — vidéo client SEO
- 2026-08-27 — [2092943710380343326](https://x.com/Timseo_/status/2092943710380343326) — rapport stats SEO gratuit
- 2026-08-27 — [2092995600799408207](https://x.com/Timseo_/status/2092995600799408207) — « LLMs GEO bonne piste »
- 2026-08-27 — [2093020214472716535](https://x.com/Timseo_/status/2093020214472716535) — « avant je faisais du SEO, maintenant je fais du [SEOCity] »
- 2026-08-28 — [2093225444896362577](https://x.com/Timseo_/status/2093225444896362577) — SEOCity « se balader dans ta ville »
- 2026-08-28 — [2093236518769017313](https://x.com/Timseo_/status/2093236518769017313) — analyse GSC + reco
- 2026-08-28 — [2093238259774288041](https://x.com/Timseo_/status/2093238259774288041) — netlify + Claude
- 2026-08-28 — [2093239482371981746](https://x.com/Timseo_/status/2093239482371981746) — dashboard pour client
- 2026-08-28 — [2093334188498006507](https://x.com/Timseo_/status/2093334188498006507) — « don't buy backlink »
- 2026-08-28 — [2093359702167990783](https://x.com/Timseo_/status/2093359702167990783) — Claude ne remplace pas un consultant seul
- 2026-08-29 — [2093528740349595868](https://x.com/Timseo_/status/2093528740349595868) — attention MAJ Google
- 2026-08-29 — [2093538244717957522](https://x.com/Timseo_/status/2093538244717957522) — intention seule, pas de guide 2000 mots
- 2026-08-29 — [2093649882259308744](https://x.com/Timseo_/status/2093649882259308744) — ancêtre concept « SimCity SEO »
- 2026-08-29 — [2093721872676655410](https://x.com/Timseo_/status/2093721872676655410) — « no need SEO tools anymore »
- 2026-08-30 — [2094097061012541844](https://x.com/Timseo_/status/2094097061012541844) — cas Golfiller top 1 (méthode + guide)
- 2026-08-31 — [2094301455624949874](https://x.com/Timseo_/status/2094301455624949874) — exemple SaaS simu 3D GSC
- 2026-08-31 — [2094322294323597812](https://x.com/Timseo_/status/2094322294323597812) — Substack comme canal d'acquisition
- 2026-08-31 — [2094381316720763284](https://x.com/Timseo_/status/2094381316720763284) — post → 42 followers
- 2026-08-31 — [2094393701779013685](https://x.com/Timseo_/status/2094393701779013685) — défi 1 000 SEOCity
- 2026-08-31 — [2094406406556545396](https://x.com/Timseo_/status/2094406406556545396) — « sans achat de BL, pas sans BL »
- 2026-08-31 — [2094407438602739747](https://x.com/Timseo_/status/2094407438602739747) — précision Golfiller : BL organiques, 0 achat
- 2026-08-31 — [2094444909717856308](https://x.com/Timseo_/status/2094444909717856308) — message perso
- 2026-08-31 — [2094447140190015972](https://x.com/Timseo_/status/2094447140190015972) — Google peut griller IP
- 2026-08-31 — [2094449562429870466](https://x.com/Timseo_/status/2094449562429870466) — Google va utiliser l'IA pour traquer
- 2026-08-31 — [2094463515415474338](https://x.com/Timseo_/status/2094463515415474338) — résultats SEOCity 5 jours
- 2026-08-31 — [2094467594313200116](https://x.com/Timseo_/status/2094467594313200116) — communauté SEO bienveillante
- 2026-08-31 — [2094492415218593813](https://x.com/Timseo_/status/2094492415218593813) — simu 3D GSC

---

## 10. Ce que ce rapport ne couvre pas

- **Posts antérieurs à mi-2025** : non récupérables via l'API MCP X avec les paramètres testés. Une partie de sa doctrine initiale est probablement là.
- **Articles longs (`x.com/i/article/...`)** : leurs contenus ne sont pas exposés par les outils utilisés. Ils sont référencés dans la timeline sans avoir été lus.
- **Threads complets avec citations imbriquées** : certains tweets référencent ou citent d'autres tweets dont le contenu n'a pas toujours été extrait en pleine profondeur.
- **Vidéos et images** : présentes en attachment sur plusieurs posts ; transcriptions / descriptions détaillées non extraites.
- **Sa chaîne Substack** (`algorithme.substack.com`) — mentionnée comme lieu de publication de sa doctrine complète ([2086721711978987528](https://x.com/Timseo_/status/2086721711978987528)) mais pas explorée.
- **Qadence.io et SEOCity.app** : cités comme produits mais leur interface / doc n'a pas été consultée dans cette analyse.

Pour une base de connaissances exhaustive, ces sources devraient être explorées en complément.

---

*Fin du rapport. Compilé à partir de 100+ publications de @Timseo_ couvrant juin 2025 → août 2026. Les conseils sont rapportés fidèlement à l'auteur, sans complétude SEO générale ajoutée.*
