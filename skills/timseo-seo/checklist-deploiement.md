# Checklist rapide déploiement — Timseo_ SEO System

> Copie-colle dans ton vault/wiki/ pour suivi projet

## 🚀 Phase 1 — Setup système (W0) — 30 min
- [ ] Vault Obsidian créé : `vault/{raw,wiki}` + `AGENTS.md` à la racine
- [ ] ChromaDB lancé (port 8000) + embeddings `sentence-transformers`
- [ ] `./kb rebuild` fonctionnel (incrémental)
- [ ] 27 automatisations configurées (launchd + scripts)

## 🎯 Phase 2 — Stratégie mots-clés & architecture (W1-W2) — 2-4h
- [ ] 3-5 mots-clés business identifiés (proximité offre + CPC + faisabilité)
- [ ] 10 micro-intentions / mot-clé business (format Do/Know + objection + format page)
- [ ] Data propriétaire collectée : appels clients, tickets SAV, avis, comparaisons
- [ ] Signaux Reddit/X récupérés (vraies questions, objections, vocabulaire)
- [ ] Univers sémantique défini par verticale gagnable
- [ ] 1-15 pages planifiées par requête stratégique (cas usage, comparatifs, FAQ, directories, data proprio)
- [ ] Templates pSEO créés si applicable (1 template = 1 variable = data proprio)

## ⚙️ Phase 3 — Technique base (W5) — 1h
- [ ] Pas de SPA pure : prerender post-build / SSR-SSG / prerender headless
- [ ] Chaque route = HTML propre avec title, meta description, canonical dans le brut
- [ ] `sitemap.xml` auto-généré + `robots.txt` + vrai `404.html` (404 HTTP)
- [ ] Title + meta description uniques + 1 seul H1 + hiérarchie H2/H3
- [ ] Canonical explicite + Open Graph + Twitter Card
- [ ] JSON-LD : Organization+WebSite (home), Article (blog), FAQPage (si visible uniquement)
- [ ] Lazy-load images width/height + font-display: swap
- [ ] Lighthouse MOBILE : LCP/INP/CLS verts

## 📝 Phase 4 — Contenu & signaux (continu)
- [ ] Pages business produites (cas usage, comparatifs, FAQ, data proprio, calculateurs)
- [ ] Ton de voix appliqué (anti-patterns IA : direct, expert, exemples concrets)
- [ ] Maillage interne lancé via Claude (crawl ou export GSC en input)
- [ ] Signaux sociaux activés : LinkedIn/YouTube/Reddit (posts optimisés mots-clés compétitifs)
- [ ] Score citabilité LLM ≥ 70/100 sur pages cibles (7 dimensions + 2 preuves atomiques/100 mots)

## 🔄 Phase 5 — Audit mensuel & boucle (W9) — mensuel
- [ ] Audit 7 phases : site/serp → quick wins → cannibalisation → clusters AEO → vecteurs sémantiques → maillage → briefs → plan 90j
- [ ] Cannibalisation : export GSC 90j complet → classifier conflits → 301 jamais 410
- [ ] Plan 90j mis à jour (priorisé impact business)
- [ ] Vérif santé 27 automatisations (chaque lundi)

## 🛑 Garde-fous (ne jamais faire)
- [ ] ❌ Acheter des backlinks
- [ ] ❌ Automatiser SEO avant d'avoir ranké 1 site
- [ ] ❌ Croire que Claude seul = consultant SEO
- [ ] ❌ Publier article blog sur requête AI Overview 9/10
- [ ] ❌ 410 sur page cannibalisée
- [ ] ❌ Produire pour produire
- [ ] ❌ SPA sans prerender
- [ ] ❌ JSON-LD sans contenu visible correspondant
- [ ] ❌ Suivre trafic/volume/position moyenne/nb BL comme KPIs

## 📊 KPIs à tracker (business-first)
- [ ] Proximité de l'offre
- [ ] Intention d'achat (Do vs Know)
- [ ] CPC
- [ ] Faisabilité ranking
- [ ] Capacité récupération email
- [ ] Score RRF

---
*Basé sur doctrine @Timseo_ (juin 2025 → août 2026). Voir skill complet `timseo-seo` pour workflows détaillés.*