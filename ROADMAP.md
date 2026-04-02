# New Project - Roadmap

> Last updated: 2026-04-02
> **VERSION ACTUELLE :** v0.2.0 (AutoNiche - Générateur Affiliation SEO)

---

## Phase 0 - Cadrage `TERMINE`

- [x] Definir le nom du projet. (AutoNiche)
- [x] Definir le probleme a resoudre. (Lenteur création sites de niche)
- [x] Definir l'utilisateur cible. (USER / Solopreneur)
- [x] Definir la proposition de valeur. (Générer des revenus passifs via SEO automatisé)
- [x] Delimiter le MVP. (Générateur Node + Template Next.js statique)
- [x] Lister les contraintes business, techniques et legales.
- [x] Choisir une stack initiale. (Next.js, Tailwind, Node.js, OpenAI API)
- [x] Fixer les criteres de succes. (Cadrage complet, prêt à concevoir l'architecture)

---

## Phase 1 - Conception `EN COURS`

- [ ] Formaliser l'architecture cible du script de génération et du template front.
- [ ] Definir le schema des donnees principales (Configuration globale, Schema Article).
- [ ] Definir les integrations externes necessaires (OpenAI, formats de prompt).
- [ ] Prioriser le backlog initial (Script Node vs Template Next).

---

## Phase 2 - Build MVP `A VENIR`

- [ ] Mettre en place le socle technique (Init Next.js, Init dossier scripts).
- [ ] Implementer le parcours principal (Génération structure -> Génération articles -> Build).
- [ ] Ajouter l'observabilite et les garde-fous minimum (Gestion des erreurs API).
- [ ] Valider les flux critiques de bout en bout sur une niche test.

---

## Phase 3 - Tests & Lancement `A VENIR`

- [ ] Tester les cas nominaux et les cas d'echec critiques (Prompt injection, timeouts).
- [ ] Corriger les blocages de production (Performance Lighthouse, indexation).
- [ ] Preparer la mise en ligne ou le pilote (Déploiement Vercel automatisé).
- [ ] Collecter les premiers retours (Trafic organique, premiers clics affiliés).

---

## Decisions verrouillees

- Le projet est un générateur de sites statiques (SSG) pour l'affiliation.
- La monétisation est strictement externe (pas de paiement géré en interne).
- L'outil est strictement backend (CLI) sans IHM pour la génération.
