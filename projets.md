---
layout: page
title: Projets
description: Réalisations techniques en génération procédurale, simulation, rendu 3D et IA appliquée
permalink: /projets/
---

<div class="project-section">
  <h3>🌳 Génération Procédurale d'Arbres 3D</h3>
  <p><strong>Technologies :</strong> C++, OpenGL, algorithmes récursifs<br>
  <strong>Contexte :</strong> Projet de rendu 3D avancé</p>

  <!-- Placeholder pour image -->
  <div style="background: #f0f0f0; border: 2px dashed #ccc; height: 200px; display: flex; align-items: center; justify-content: center; margin: 1rem 0; border-radius: 6px;">
    <span style="color: #666;">🖼️ Image : Arbre 3D généré procéduralement</span>
  </div>

  <h4>🎯 Description</h4>
  <p>Algorithme paramétrique générant des structures arborescentes complètes avec tronc, ramifications hiérarchiques et courbure contrôlée. Le système permet de créer une grande variété d'arbres réalistes à partir de quelques paramètres simples.</p>

  <h4>⚙️ Paramètres de contrôle</h4>
  <table>
    <tr>
      <th>Paramètre</th>
      <th>Effet</th>
      <th>Plage typique</th>
    </tr>
    <tr>
      <td><code>seed</code></td>
      <td>Reproductibilité des résultats</td>
      <td>0 - 999999</td>
    </tr>
    <tr>
      <td><code>branch_factor</code></td>
      <td>Densité de ramifications par nœud</td>
      <td>2 - 6</td>
    </tr>
    <tr>
      <td><code>depth</code></td>
      <td>Profondeur hiérarchique maximale</td>
      <td>4 - 8</td>
    </tr>
    <tr>
      <td><code>curvature</code></td>
      <td>Courbure moyenne des segments</td>
      <td>0.1 - 0.8</td>
    </tr>
    <tr>
      <td><code>taper</code></td>
      <td>Amincissement progressif des branches</td>
      <td>0.6 - 0.9</td>
    </tr>
  </table>

  <h4>🔄 Pipeline de génération</h4>
  <ol>
    <li><strong>Génération récursive :</strong> Construction de la structure arborescente</li>
    <li><strong>Conversion en maillage :</strong> Transformation en géométrie 3D</li>
    <li><strong>Lissage :</strong> Recalcul des normales pour un rendu réaliste</li>
    <li><strong>Export multi-format :</strong> OBJ, glTF avec niveaux de détail (LOD)</li>
  </ol>

  <h4>💻 Exemple d'algorithme</h4>
  <pre><code class="language-cpp">
Node* grow(Node* parent, int remaining_depth) {
    if (remaining_depth == 0) return parent;
    
    int branch_count = random_range(1, branch_factor);
    for (int i = 0; i &lt; branch_count; ++i) {
        auto* child = new Node(
            calculate_branch_direction(parent, i),
            parent-&gt;radius * taper,
            parent-&gt;length * length_ratio
        );
        parent-&gt;children.push_back(child);
        grow(child, remaining_depth - 1);
    }
    return parent;
}
  </code></pre>

  <h4>🚀 Améliorations futures</h4>
  <ul>
    <li>Génération de feuillage procédural avec billboards et instancing</li>
    <li>Système de LOD automatique basé sur la distance et l'angle de vue</li>
    <li>Générateur paramétré pour différents biomes (tropical, tempéré, boréal)</li>
    <li>Export vers moteurs de jeu (Unity, Unreal Engine)</li>
  </ul>
</div>

<div class="project-section">
  <h3>📖 Moteur Narratif Augmenté (Endless Novel)</h3>
  <p><strong>Technologies :</strong> C++, Python, JSON/YAML, APIs IA<br>
  <strong>Contexte :</strong> Stage BLACKCODE - Prototype de recherche</p>

  <div style="background: #f0f0f0; border: 2px dashed #ccc; height: 200px; display: flex; align-items: center; justify-content: center; margin: 1rem 0; border-radius: 6px;">
    <span style="color: #666;">🖼️ Diagramme : Architecture du moteur narratif</span>
  </div>

  <h4>🎯 Vision</h4>
  <p>Génération adaptative de scènes textuelles avec contrôle rigoureux de cohérence narrative. Le système maintient un état persistant et s'adapte aux choix du lecteur tout en préservant la logique du récit.</p>

  <h4>🏗️ Architecture technique</h4>
  <pre><code>
endless_novel/
├── core/
│   ├── engine/
│   │   ├── story_state.hpp      # État global du récit
│   │   ├── narrative_rules.hpp  # Règles de cohérence
│   │   └── character_manager.hpp
│   ├── runtime/
│   │   ├── branching.cpp        # Gestion des embranchements
│   │   ├── interpreter.cpp      # Exécution des scènes
│   │   └── ai_interface.cpp     # Interface avec IA
│   └── data/
│       ├── characters/          # Définitions personnages
│       ├── locations/           # Environnements
│       └── templates/           # Modèles de scènes
  </code></pre>

  <h4>🧩 Défis techniques résolus</h4>
  <table>
    <tr>
      <th>Défi</th>
      <th>Solution implémentée</th>
    </tr>
    <tr>
      <td><strong>Cohérence narrative</strong></td>
      <td>Table de symboles + système de snapshots mémoire</td>
    </tr>
    <tr>
      <td><strong>Contrôle de l'IA</strong></td>
      <td>Filtrage contextuel et gabarits textuels</td>
    </tr>
    <tr>
      <td><strong>Extensibilité</strong></td>
      <td>Architecture modulaire avec registre de règles</td>
    </tr>
    <tr>
      <td><strong>Performance</strong></td>
      <td>Cache intelligent et génération asynchrone</td>
    </tr>
  </table>

  <h4>🎨 Fonctionnalités principales</h4>
  <ul>
    <li><strong>Génération contextuelle :</strong> Scènes adaptées à l'état du récit</li>
    <li><strong>Mémoire persistante :</strong> Suivi des personnages, lieux et événements</li>
    <li><strong>Validation automatique :</strong> Vérification de cohérence pré-diffusion</li>
    <li><strong>Interface modulaire :</strong> Préparation pour intégration UI future</li>
  </ul>

  <h4>📋 Roadmap de développement</h4>
  <ul>
    <li>Implémentation d'un cache de "souvenirs" pondérés</li>
    <li>Génération d'illustrations contextuelles automatiques</li>
    <li>Export vers format HTML interactif</li>
    <li>Interface graphique utilisateur intuitive</li>
  </ul>
</div>

<div class="project-section">
  <h3>📐 Reconstruction 3D Basée Images</h3>
  <p><strong>Technologies :</strong> Python, OpenCV, algorithmes de vision par ordinateur<br>
  <strong>Contexte :</strong> Projet M1 - Application médicale</p>

  <div style="background: #f0f0f0; border: 2px dashed #ccc; height: 200px; display: flex; align-items: center; justify-content: center; margin: 1rem 0; border-radius: 6px;">
    <span style="color: #666;">🖼️ Pipeline : De l'image 2D au modèle 3D</span>
  </div>

  <h4>🎯 Objectif médical</h4>
  <p>Projet exploratoire visant à reconstruire un modèle 3D anatomique à partir de vues multiples pour assister la détection de position patient en chirurgie percutanée.</p>

  <h4>🔬 Méthodologie technique</h4>
  <ol>
    <li><strong>Prétraitement :</strong> Filtrage et normalisation des images d'entrée</li>
    <li><strong>Détection de caractéristiques :</strong> Points clés et correspondances inter-images</li>
    <li><strong>Triangulation :</strong> Reconstruction 3D par intersection de rayons</li>
    <li><strong>Fusion :</strong> Assemblage du nuage de points en maillage cohérent</li>
    <li><strong>Validation :</strong> Estimation des erreurs de reprojection</li>
  </ol>

  <h4>⚡ Défis rencontrés</h4>
  <ul>
    <li><strong>Calibration caméra :</strong> Précision des paramètres intrinsèques et extrinsèques</li>
    <li><strong>Correspondances robustes :</strong> Gestion des occultations et variations d'éclairage</li>
    <li><strong>Optimisation :</strong> Équilibre entre précision et temps de calcul</li>
    <li><strong>Validation médicale :</strong> Respect des contraintes de précision clinique</li>
  </ul>

  <h4>🔬 Résultats obtenus</h4>
  <ul>
    <li>Pipeline fonctionnel de reconstruction multi-vues</li>
    <li>Précision suffisante pour applications d'aide au positionnement</li>
    <li>Documentation complète du processus et des limitations</li>
  </ul>

  <h4>🚀 Perspectives d'amélioration</h4>
  <ul>
    <li>Calibration avancée multi-caméras temps réel</li>
    <li>Comparaison d'algorithmes alternatifs (SLAM, photogrammétrie)</li>
    <li>Export vers environnements VR/AR (glTF, PLY)</li>
    <li>Intégration avec systèmes de navigation chirurgicale</li>
  </ul>
</div>

<div class="project-section">
  <h3>🧲 Simulation Aimant Bitter - Couplage Thermo-Électrique</h3>
  <p><strong>Technologies :</strong> Gmsh, ParaView, Python, solveurs numériques<br>
  <strong>Contexte :</strong> Projet de simulation numérique avancée</p>

  <div style="background: #f0f0f0; border: 2px dashed #ccc; height: 200px; display: flex; align-items: center; justify-content: center; margin: 1rem 0; border-radius: 6px;">
    <span style="color: #666;">🖼️ Visualisation : Champs thermique et électrique</span>
  </div>

  <h4>🎯 Problématique scientifique</h4>
  <p>Étude de la répartition thermique et des flux de courant dans une structure d'aimant supraconducteur de type Bitter, caractérisée par des géométries complexes et des couplages physiques multiples.</p>

  <h4>🛠️ Chaîne d'outils complète</h4>
  <table>
    <tr>
      <th>Étape</th>
      <th>Outil</th>
      <th>Fonction</th>
    </tr>
    <tr>
      <td><strong>Géométrie</strong></td>
      <td>Gmsh</td>
      <td>Modélisation CAD et maillage adaptatif</td>
    </tr>
    <tr>
      <td><strong>Calcul</strong></td>
      <td>Solveur FEM custom</td>
      <td>Résolution couplée thermo-électrique</td>
    </tr>
    <tr>
      <td><strong>Visualisation</strong></td>
      <td>ParaView</td>
      <td>Rendu scientifique des champs</td>
    </tr>
    <tr>
      <td><strong>Post-traitement</strong></td>
      <td>Python/NumPy</td>
      <td>Analyse statistique et métriques</td>
    </tr>
  </table>

  <h4>🔄 Workflow de simulation</h4>
  <ol>
    <li><strong>Géométrie paramétrée :</strong> Modèle CAD flexible avec paramètres d'entrée</li>
    <li><strong>Maillage adaptatif :</strong> Raffinement local dans les zones critiques</li>
    <li><strong>Résolution itérative :</strong> Couplage des équations de diffusion thermique et électrique</li>
    <li><strong>Convergence :</strong> Critères de stabilité et validation numérique</li>
    <li><strong>Export multi-format :</strong> VTK, HDF5 pour visualisation et archivage</li>
  </ol>

  <h4>📊 Résultats et métriques</h4>
  <ul>
    <li><strong>Cartes thermiques :</strong> Distribution spatiale des températures</li>
    <li><strong>Flux électriques :</strong> Densité de courant et résistivité locale</li>
    <li><strong>Points critiques :</strong> Identification des zones de concentration thermique</li>
    <li><strong>Validation :</strong> Comparaison avec données expérimentales disponibles</li>
  </ul>

  <h4>🔬 Pistes de recherche avancées</h4>
  <ul>
    <li>Couplage thermo-mécanique pour déformation structurelle</li>
    <li>Automatisation de métriques (ΔT max, gradients critiques)</li>
    <li>Optimisation multi-résolution pour calculs haute performance</li>
    <li>Intégration dans pipeline de conception d'aimants</li>
  </ul>
</div>

<div style="background: #e8f4f8; border-left: 4px solid #0366d6; padding: 1.5rem; margin-top: 2rem;">
  <h3 style="margin-top: 0; color: #0366d6;">💡 Philosophy des projets</h3>
  <p style="margin-bottom: 0;">
    Chaque projet reflète une approche méthodique combinant <strong>rigueur technique</strong>, 
    <strong>innovation créative</strong> et <strong>applications concrètes</strong>. 
    L'objectif est toujours de créer des outils robustes, documentés et réutilisables, 
    pouvant servir de base à des développements futurs plus ambitieux.
  </p>
</div>
