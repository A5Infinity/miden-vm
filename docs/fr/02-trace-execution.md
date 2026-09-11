# 02 — De l’exécution à la trace

Le processeur de `processor/` exécute les instructions et construit les colonnes de trace.
Chaque ligne encode un état successif de la machine virtuelle.
Les contextes isolés séparent mémoire racine et mémoires utilisateur.
Les procédures et appels noyau structurent les transitions entre ces contextes.
Les entrées non déterministes permettent au prouveur de fournir secrets et conseils d’exécution.
Elles ne deviennent pas des faits gratuits : les contraintes doivent encore valider leurs effets.
La trace constitue ainsi le témoin algébrique remis au système de preuve.
Cette articulation explique pourquoi exécuter et prouver restent deux responsabilités distinctes.

Suite : [les contraintes AIR](03-contraintes-air.md).
