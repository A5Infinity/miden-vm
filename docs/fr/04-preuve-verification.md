# 04 — Produire puis vérifier la preuve

Le crate `prover/` reçoit la trace et construit la preuve STARK avec Plonky3 adapté à Miden.
Le crate `verifier/` contrôle les engagements et requêtes du protocole.
Cette séparation permet à un vérificateur de confirmer l’exécution sans la reproduire.
La taille de preuve croît beaucoup moins vite que le nombre de cycles présenté dans les mesures amont.
Le dépôt expose plusieurs choix de hachage qui influencent coût et récursivité.
BLAKE3 privilégie la vitesse de preuve sur machine classique.
Poseidon2 est plus naturel à arithmétiser pour une vérification dans une autre preuve.
Le choix du hachage est donc une décision d’architecture, pas un simple détail d’implémentation.

Suite : [précompiles et limites de confiance](05-precompiles-limites.md).
