---
name: ikigai-business-ia
description: Génère des idées de business IA à partir de l'Ikigai de l'utilisateur (aime / sait faire / besoin du monde / payé pour), en QCM une question à la fois, vérifie le marché sur le web, note et passe la short-list en Blue Ocean. À utiliser quand l'utilisateur cherche une idée de business IA, de SaaS IA, de side project rentable ou dit « trouve-moi une idée de business », « mon ikigai », « quoi lancer avec l'IA ».
---

# Ikigai business IA

Objectif : faire émerger 8 à 10 idées de business IA ancrées dans l'Ikigai de l'utilisateur, puis en approfondir 3, notées et confrontées au marché réel.

## Règles transverses

- **Annonce** : au démarrage, dire en une phrase que le skill s'applique et ce qu'il va produire. Ne pas démarrer en silence.
- **QCM une question à la fois** : chaque question est un QCM (outil de questions si disponible, sinon liste numérotée) avec toujours une option « Autre ». La réponse oriente la question suivante. Jamais de questionnaire en bloc.
- **Portes de validation** : chaque phase se termine par une synthèse courte que l'utilisateur valide avant de passer à la suivante.
- **Persistance** : tenir à jour `ikigai-progress.md` (phase courante, réponses, idées, scores, sources). À chaque démarrage, chercher ce fichier et proposer de reprendre.
- **Honnêteté** : signaler sans détour une idée qui rate un cercle. Ne pas gonfler les scores. Les faits de marché viennent de sources citées, jamais de mémoire.
- Langue : français.

## Phase 0 — Cadrage

1. Lire la mémoire / le profil de l'utilisateur et pré-remplir ce qui est déjà connu (métier, stack, projets passés, centres d'intérêt). Présenter ce pré-remplissage pour validation : l'utilisateur corrige, rien n'est considéré comme acquis.
2. QCM : quel cadrage pour « business IA » ?
   - **A. Produit IA** : l'IA est la valeur vendue (SaaS, agent, outil).
   - **B. Business opéré par agents** : n'importe quel secteur, monté et exploité seul avec des agents.
3. Consigner le cadrage dans le fichier de progression.

## Phase 1 — Les 4 cercles (QCM itératifs)

Un cercle à la fois, 2 à 4 questions par cercle, en partant du pré-remplissage :

1. **Ce que j'aime** : sujets, problèmes qui passionnent, ce sur quoi on travaillerait gratuitement.
2. **Ce que je sais faire** : compétences, expertise métier, accès privilégié (réseau, données, secteur).
3. **Ce dont le monde a besoin** : problèmes observés, frustrations vécues, populations mal servies.
4. **Ce pour quoi on peut être payé** : qui a un budget, quels modèles (abonnement, service, commission).

Porte : synthèse des 4 cercles + des 4 intersections (passion, mission, vocation, profession). Validation.

## Phase 2 — Génération (8 à 10 idées)

- Chaque idée doit partir d'au moins un élément concret de chaque cercle, cité.
- Format par idée : nom, une phrase de proposition de valeur, cible, rôle de l'IA (cadrage A) ou rôle des agents dans l'exploitation (cadrage B), éléments Ikigai mobilisés.
- Varier les modèles (B2B / B2C, produit / service) pour éviter 10 variantes d'une même idée.

Porte : l'utilisateur choisit 3 idées par QCM à choix multiples (le skill peut recommander, l'utilisateur tranche).

## Phase 3 — Vérification marché (recherche web)

Pour chacune des 3 idées :
- demande : signaux de besoin (recherches, communautés, appels d'offres) ;
- concurrence : acteurs existants, prix constatés ;
- disposition à payer : prix pratiqués sur des offres comparables.

Toujours citer les sources. Signaler explicitement quand le signal est faible ou introuvable.

## Phase 4 — Notation

Trois critères notés de 1 à 5 (quatre en cadrage B), avec une justification d'une ligne chacun :

| Critère | Question |
|---|---|
| Couverture des 4 cercles | Score par cercle ; un cercle à 1 ou 2 = drapeau rouge nommé (passion sans marché, métier sans plaisir, etc.) |
| Signal marché vérifié | La phase 3 montre-t-elle une demande réelle et solvable ? |
| Défendabilité | Qu'est-ce qui empêche un concurrent ou un LLM généraliste de faire pareil demain ? |
| Faisabilité solo + agents (cadrage B uniquement) | Quelles tâches d'exploitation restent humaines (relation client, logistique, réglementaire, présence physique) ? Une tâche humaine récurrente et non déléguable = score ≤ 2 |

Pas de moyenne qui masque un zéro : une idée avec un critère à 1 est signalée quel que soit son total.

## Phase 5 — Blue Ocean

Pour chaque idée de la short-list : grille ERRC (Éliminer, Réduire, Renforcer, Créer) face aux concurrents trouvés en phase 3, et courbe de valeur résumée en une phrase.

## Phase 6 — Livrable

Produire un document (type Docs si disponible, sinon Markdown) :
1. Ikigai de l'utilisateur (4 cercles + intersections)
2. Les 8 à 10 idées générées (une ligne chacune)
3. Les 3 idées approfondies : marché sourcé, scores, grille ERRC
4. Recommandation argumentée et risques principaux
5. Prochaines étapes concrètes pour valider l'idée retenue (interviews, landing page, prévente)
6. Sources

Mettre à jour le fichier de progression en « terminé ».
