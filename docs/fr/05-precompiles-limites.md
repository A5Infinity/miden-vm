# 05 — Précompiles, périmètre et limites

Les précompiles permettent de différer des calculs coûteux vers l’hôte.
La VM authentifie une racine différée, puis une preuve agrégée peut solder les exécutions compatibles.
Les crates `precompiles-*` séparent registre, AIR, production et vérification de ces preuves.
Cette optimisation élargit aussi le modèle de confiance à documenter autour de l’hôte et des données externes.
Le support récursif complet est encore présenté comme une fonctionnalité planifiée dans le README amont.
Le projet est explicitement alpha, non audité et sujet à des changements incompatibles.
Ce parcours est une lecture documentaire des dossiers `core/`, `processor/`, `air/`, `prover/` et `verifier/`.
Aucune installation, compilation ou exécution nouvelle n’a été effectuée ; la suite `tests/` reste la référence pour vérifier le comportement.
