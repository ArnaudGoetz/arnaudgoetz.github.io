# Moteur Narratif Augmenté (Endless Novel) – Prototype

> Génération adaptative de scènes textuelles avec contrôle de cohérence.

![Hero narratif](../../assets/img/projets/narratif/hero_narratif.png)

## Galerie (placeholders)
Prévoir 4 images : console, diagramme d’état, séquence test, mémoire.

## Objectifs
- Génération / mutation de scènes selon état
- Suivi personnages / attributs
- Préparation intégration modèle IA future (module abstrait)

## Stack
C++ (core), Python (outils), JSON/YAML.

## Architecture (extrait)
```
core/
  engine/
    story_state.hpp
    narrative_rules.hpp
  runtime/
    branching.cpp
    interpreter.cpp
  data/
    characters/
    locations/
```

## Défis
| Défi | Approche |
|------|----------|
| Cohérence | Table de symboles + snapshot mémoire |
| Contrôle IA | Filtrage / gabarits textuels |
| Extensibilité | Modules ponctuels (règles -> registre) |

## Roadmap
- [ ] Cache de “souvenirs” pondérés
- [ ] Génération d’illustrations contextuelles
- [ ] Export HTML interactif