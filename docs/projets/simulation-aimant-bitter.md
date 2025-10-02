# Simulation Aimant Bitter (Thermique & Électrique)

![Hero Bitter](../../assets/img/projets/simulation/hero_bitter.png)

## Galerie (placeholders)
Maillage, carte thermique, flux courant, gradient zones.

## Objectif
Étudier la répartition thermique + flux de courant dans une structure de type Bitter.

## Outils
| Étape | Outil |
|-------|-------|
| Maillage | Gmsh |
| Résolution | Solveur expérimental / externe |
| Visualisation | ParaView |
| Post-traitement | Scripts Python |

## Étapes
1. Géométrie paramétrée
2. Raffinement local
3. Résolution itérative
4. Export VTK → Visualisation

## Pistes
- Couplage thermo-mécanique
- Script auto métriques (ΔT max)
- Optimisation multi-résolution