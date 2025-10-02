# Génération Procédurale d’Arbres 3D

![Hero arbre](../../assets/img/projets/procedural/hero_tree.png)

## Galerie (placeholders)
Wireframe, LOD, texture bake, export.

## Description
Algorithme paramétrique générant des structures arborescentes (tronc, ramifications hiérarchiques, courbure contrôlée).

## Paramètres clés
| Paramètre | Effet |
|-----------|------|
| seed | Reproductibilité |
| branch_factor | Densité de ramifications |
| depth | Profondeur hiérarchique max |
| curvature | Courbure moyenne segments |
| taper | Amincissement progressif |

## Pipeline
1. Génération récursive (structure)
2. Conversion → maillage
3. Lissage & recalcul normales
4. Export (OBJ / glTF) + LOD

## Exemple (pseudo-code)
```cpp
Node* grow(Node* n, int depth) {
  if (depth == 0) return n;
  int count = random_range(1, branch_factor);
  for (int i = 0; i < count; ++i) {
    auto* child = new Node(curve_direction(n, i));
    n->children.push_back(child);
    grow(child, depth - 1);
  }
  return n;
}
```

## Améliorations
- [ ] Feuillage procédural (billboards / instancing)
- [ ] LOD auto (distance / angle)
- [ ] Générateur paramétré pour biomes