# 03 — Les contraintes AIR

Le dossier `air/` décrit les identités polynomiales attendues de toute trace valide.
Ces contraintes relient l’état courant au suivant et imposent la sémantique des instructions.
Elles couvrent notamment pile, mémoire, décodeur et opérations cryptographiques.
Une trace produite par le processeur n’est acceptable que si ces relations sont satisfaites.
L’AIR constitue donc le contrat mathématique entre l’exécuteur et le vérificateur.
Cette frontière aide l’audit : une instruction doit être cohérente côté exécution et côté contraintes.
Les composants `lifted-air` et `constraint-compiler` prolongent cette représentation symbolique.
Une divergence entre sémantique et AIR serait une surface de risque critique.

Suite : [prouver et vérifier](04-preuve-verification.md).
