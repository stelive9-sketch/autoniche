# NEW PROJECT - PROJECT BIBLE

> **VERSION :** v0.2.0 (2026-04-02)
> **STATUS :** Phase de cadrage validée. Projet "AutoNiche" lancé.
> **STACK :** Next.js (React), TailwindCSS, Node.js (scripts), OpenAI API.
> **DEPLOY :** Vercel (Hébergement statique).
> **OBJECTIF :** Générer de l'argent de manière 100% passive via création massive de contenu SEO orienté affiliation.

---

## 1. Vision du projet

- **Probleme adresse** : La création manuelle de sites de niche pour l'affiliation est trop lente et non scalable.
- **Utilisateur cible** : Le propriétaire du système (USER), souhaitant un revenu passif.
- **Proposition de valeur** : Générer, à partir d'un seul mot-clé, un site web complet ultra-optimisé SEO, rempli de contenu pertinent et intégrant des liens d'affiliation.
- **Resultat attendu** : Un moteur de génération (CLI/Node.js) + Un template de site statique Next.js prêt à être déployé de manière illimitée.

---

## 2. Perimetre

### In scope

- Script Node.js pour orchestrer l'API OpenAI (Génération de cocons sémantiques, articles, métadonnées).
- Template de front-end Next.js (App Router, SSG, ultra-rapide, score Lighthouse 100).
- Intégration automatique de balises SEO et données structurées.
- Emplacements publicitaires/affiliation gérés via fichier de configuration unique.

### Out of scope

- E-commerce direct ou gestion de paiements (exclusivement monétisation externe).
- Back-office UI (la configuration se fait via variables d'environnement et fichiers JSON locaux).
- Inscription utilisateurs (outil strictement interne/personnel).

---

## 3. Architecture cible

| Domaine | Decision actuelle |
|---|---|
| Frontend | Next.js (React), TailwindCSS, Markdown/MDX |
| Backend | Scripts Node.js locaux (pas de serveur backend live) |
| Base de donnees | Fichiers JSON et MDX locaux (aucune BDD distante nécessaire) |
| Integrations externes | OpenAI API (gpt-4-turbo ou gpt-3.5-turbo pour les volumes) |
| IA / automatisation | Prompts chaînés pour génération de contenu sans hallucination |
| Infra / deploy | Déploiement Vercel via Github Actions ou Git push automatisé |

---

## 4. Donnees et integrations

- **Entites principales** : Configuration du site (Thème, Affiliation ID), Articles (Titre, Slug, Contenu, Meta).
- **Sources de donnees** : API OpenAI pour la création textuelle.
- **APIs / services externes** : API OpenAI, Vercel CLI.
- **Secrets / credentials** : `OPENAI_API_KEY`, tokens d'affiliation (Amazon Partenaires, etc.).

---

## 5. Contraintes

- **Business** : Zéro coût d'infrastructure (Vercel Free tier, API OpenAI contrôlée par limites).
- **Technique** : Les sites doivent être statiques pour une performance maximale et la sécurité.
- **Securite / legal** : Ajout automatique des mentions légales (RGPD) et avertissements d'affiliation.
- **Performance / cout** : Génération d'un site complet pour un coût minimal.

---

## 6. Regles critiques

- Aucune hypothese du projet precedent ne doit etre reutilisee sans validation explicite.
- Toute decision structurelle validee doit etre documentee ici avant ou juste apres implementation.
- Toute dependance externe doit etre identifiee avant de devenir un prerequis du projet.
- **Règle absolue** : La qualité du contenu SEO prime. Les prompts Markdown doivent interdire le "bla-bla" IA et imposer un ton expert.

---

## 7. Hypotheses a valider

- Sélectionner la première niche d'affiliation à cibler pour valider le MVP.
- Vérifier les limites de rate-limit de l'API OpenAI pour une génération massive simultanée.

---

## 8. Definition of done initiale

- Le problème, la cible et la proposition de valeur sont définis. (FAIT)
- Le MVP est délimité avec des critères de succès clairs. (FAIT)
- La stack et les contraintes critiques sont documentées. (FAIT)
- La roadmap des prochaines phases est cohérente avec ces décisions. (FAIT)

---

## 9. Etat actuel

- Vision produit AutoNiche actée.
- Validation des phases de cadrage terminée.
- Prêt pour la Phase 1 : Conception des schémas de données et de l'architecture précise du générateur Markdown.
