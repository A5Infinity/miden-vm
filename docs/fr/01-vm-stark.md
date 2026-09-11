# 01 — Une machine virtuelle conçue pour les STARK

Miden VM exécute des programmes tout en produisant une trace destinée à être prouvée.
Le dépôt sépare clairement les types communs (`core/`), l’exécution (`processor/`) et les contraintes (`air/`).
Cette séparation rend visible la frontière entre sémantique de la VM et validité cryptographique.
Le prouveur transforme ensuite la trace en preuve STARK dans `prover/`.
Le vérificateur de `verifier/` contrôle cette preuve sans rejouer tout le programme.
Les STARK évitent une cérémonie de configuration de confiance.
Le README amont avertit toutefois que le projet reste en phase alpha et non audité.
Ce parcours décrit donc l’architecture observée, sans conclure à une aptitude en production.

Suite : [la trace d’exécution](02-trace-execution.md).
