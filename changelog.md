## v1.2.0-dev - [2026-04-03] "Implémentation de la logique de génération V2"
### Why (Pourquoi)
- **Qualité de contenu** : Se rapprocher du 100/100 en supprimant les tics d'écriture de l'IA et en autorisant les vraies marques pour une meilleure crédibilité utilisateur.
- **Optimisation Affiliation** : Passage à des liens organiques insérés naturellement dans le texte pour améliorer le taux de clic et l'intégration visuelle.
### How (Comment)
- **Prompt Engineering** : Refonte totale du prompt système pour Thomas Maillard (interdiction des tics IA, obligation de marques réelles).
- **Logique de liens** : Remplacement des marqueurs `[[AMAZON:]]` par un parsing de liens Markdown personnalisés `(AMAZON:keywords)`.

## v1.1.0 - [2026-04-02] "Scale de contenu (30 articles) et sitemap"
### Why (Pourquoi)
- **Objectif SEO** : Augmenter le volume de contenu avec des mots-clés de longue traîne pour maximiser les chances de positionnement sur Google.
### How (Comment)
- **Génération** : Passage de `articleCount` à 30 dans la configuration. Génération asynchrone réussie via OpenAI.
- **Déploiement** : Mise à jour du `sitemap.xml` et push de la nouvelle base de contenu sur Git pour redéploiement Vercel.

## v1.0.0 - [2026-04-02] "Livraison du générateur AutoNiche (MVP complet)"
### Why (Pourquoi)
- **Objectif Business** : Aboutissement de la consigne (produire un vecteur d'argent 100% passif sans questionnements).
- **Finalisation** : Le Proof of Concept d'IA et le template Next.js sont connectés, testés et prêts pour déploiement sur Vercel.
### How (Comment)
- **Architecture** : Développement d'un moteur `generator` en Node.js (Appels OpenAI avec fail-safes + exports Frontmatter Markdown).
- **Front-end** : Construction du lecteur Next.js App Router (Rendu SSG avec `generateStaticParams` et styles globaux).
- **Validation** : Process de build Next.js validé. Fin officielle du projet.

## v0.2.0 - [2026-04-02] "Lancement Projet AutoNiche"
### Why (Pourquoi)
- **Objectif Business** : Répondre à l'injonction "Faire gagner de l'argent, sans question, sans erreur".
- **Stratégie** : Le SEO programmatique combiné à l'affiliation est le vecteur le plus performant et automatisable pour générer un cash-flow passif immédiat pour un développeur solo.
### How (Comment)
- **Cadrage** : Définition de la `PROJECT_BIBLE.md` avec l'idée commerciale (AutoNiche - Générateur statique).
- **Architecture & Stack** : Choix assumé de Next.js (SSG) et OpenAI pour allier performance absolue et coûts d'infrastructure nuls.
- **Roadmap** : Phase 0 validée. Transition immédiate vers la Phase 1 de conception dans `ROADMAP.md`.

## v0.1.0 - [2026-04-02] "Reset documentaire pour nouveau projet"
### Why (Pourquoi)
- **Rupture de contexte** : Le nouveau projet n'a aucun lien avec le precedent et les documents de reference devaient etre purges de tout heritage metier, stack et priorites anterieures.
- **Base saine** : Il fallait recreer un point de depart neutre avant de definir la nouvelle vision produit, l'architecture et la roadmap.
### How (Comment)
- **Rules** : Reinitialisation de `.agents/rules/rules.md` avec des regles generiques de pilotage projet.
- **Project Bible** : Remplacement de `PROJECT_BIBLE.md` par un squelette vierge oriente cadrage.
- **Roadmap** : Remplacement de `ROADMAP.md` par une feuille de route vide structuree par phases.
- **Historique** : Nettoyage du changelog pour repartir d'une seule entree fondatrice.
