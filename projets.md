---
layout: page
title: Projets
description: Réalisations techniques en génération procédurale, simulation, rendu 3D et IA appliquée
permalink: /projets/
---

<div class="intro-note" style="background-color: #f6f8fa; border-left: 4px solid #0366d6; padding: 15px 20px; margin-bottom: 40px; border-radius: 4px;">
  <p style="margin: 0; line-height: 1.6;">
    <strong>Note :</strong> Les projets présentés ci-dessous constituent une sélection représentative de mon parcours 
    de <strong>Master</strong>, mais ne reflètent pas l'intégralité de mes réalisations. 
    Ils ont été choisis pour illustrer la <strong>diversité des compétences</strong> acquises et la 
    <strong>pluralité de ma formation</strong>.
  </p>
</div>

<div class="project-section">
  <h3>Génération d'Arbre Procédurale en 3D - Bucket Sort - Exploration d'Espace</h3>
  
  <h4>Contexte et Objectifs</h4>
  <p>
    Les modèles 3D d'arbres sont particulièrement lourds dans les jeux vidéo et les simulations. 
    Ce projet propose une solution pour concilier réalisme visuel et performance, en générant des arbres 
    personnalisables et reproductibles en temps réel.
  </p>
  
  <h4>Contraintes Techniques</h4>
  <ul>
    <li><strong>Performance temps réel</strong> : Méthodes d'exécution rapides adaptées aux applications interactives</li>
    <li><strong>Génération procédurale</strong> : Chaque arbre est unique selon les paramètres fournis</li>
    <li><strong>Topologie correcte</strong> : Maillages manifold garantissant une géométrie valide</li>
  </ul>
  
  <h4>Pipeline de Génération</h4>
  <ol>
    <li><strong>Génération de nuage de points</strong> : Utilisation de la super-formule pour créer l'enveloppe de la couronne</li>
    <li><strong>Structure accélératrice</strong> : Implémentation d'un tri par paquet (Bucket Sort) pour optimiser les calculs</li>
    <li><strong>Algorithme de colonisation d'espace</strong> : Croissance organique des branches vers les points attracteurs</li>
    <li><strong>Conversion en maillage manifold</strong> : Transformation du squelette en géométrie 3D valide</li>
    <li><strong>Rendu optimisé</strong> : Affichage performant du résultat final</li>
  </ol>
  
  <h4>Méthode : Space Colonization Algorithm</h4>
  <p>
    L'algorithme repose sur une approche de colonisation d'espace inspirée par la croissance naturelle des arbres. 
    Les branches se développent en direction de points attracteurs distribués dans la couronne, créant une structure 
    organique et réaliste.
  </p>
  <p>
    <em>Basé sur les travaux de Ratul et al. (2019) : "Applicability of space colonization algorithm for real time tree generation", 
    International Conference on Computer and Information Technology (ICCIT).</em>
  </p>
  
  <h4>Rapport Technique Complet</h4>
  <div class="pdf-viewer-container" style="margin: 20px 0; border: 1px solid #ddd; border-radius: 4px; overflow: hidden;">
    <iframe 
      src="/assets/rapports/arbre_procedural.pdf" 
      width="100%" 
      height="600px" 
      style="border: none;"
      title="Rapport - Génération d'Arbre Procédurale">
    </iframe>
    <p style="text-align: center; padding: 10px; background-color: #f5f5f5; margin: 0;">
      <a href="/assets/rapports/arbre_procedural.pdf" download style="text-decoration: none; color: #0366d6; font-weight: bold;">
        📄 Télécharger le rapport PDF
      </a>
    </p>
  </div>
  
  <h4>Technologies</h4>
  <p>
    <span class="tech-tag">C++</span>
    <span class="tech-tag">OpenGL</span>
    <span class="tech-tag">Génération Procédurale</span>
    <span class="tech-tag">Géométrie Algorithmique</span>
    <span class="tech-tag">Optimisation Spatiale</span>
  </p>
</div>

<div class="project-section">
  <h3>Reconstruction 3D Basée Image pour la Détection de Position du Patient en Chirurgie Percutanée</h3>
  <p><em>Projet de recherche M1 supervisé</em></p>
  
  <h4>Contexte Médical</h4>
  <p>
    La cryoablation percutanée utilise une aiguille pour geler les tumeurs de manière minimalement invasive. 
    En chirurgie assistée par ordinateur, le guidage précis de l'aiguille le long d'un trajet planifié est essentiel 
    pour garantir l'efficacité du traitement. Cela nécessite une localisation précise du patient et une recalibration 
    du modèle 3D en temps réel.
  </p>
  
  <h4>Innovation et Objectifs</h4>
  <p>
    Ce projet vise à optimiser le processus de détection et recalibration en réduisant les coûts d'équipement et 
    l'encombrement spatial. L'approche proposée utilise un smartphone ou une webcam pour la détection et la 
    recalibration, en remplacement des systèmes de tracking coûteux traditionnels.
  </p>
  <p>
    <strong>Objectif principal :</strong> Reconstruire la forme 3D de la peau du patient à partir d'images 2D 
    (photos ou vidéos) pour permettre la recalibration du modèle numérique avec la surface réelle.
  </p>
  
  <h4>Méthodologie de Recherche</h4>
  <p><strong>Phase 1 : État de l'art</strong></p>
  <ul>
    <li>Revue complète de la littérature sur les méthodes de reconstruction 3D basée image</li>
    <li>Analyse des technologies existantes dans le domaine</li>
    <li>Synthèse comparative des différentes approches</li>
  </ul>
  
  <p><strong>Phase 2 : Implémentation technique</strong></p>
  <ul>
    <li><strong>DepthAnything</strong> : Transformation des images 2D en cartes de profondeur (depth maps)</li>
    <li><strong>Open3D</strong> : Génération de nuages de points à partir des cartes de profondeur</li>
    <li><strong>Pipeline complet</strong> : Photo/Vidéo → Depth Map → Point Cloud → Reconstruction de surface</li>
  </ul>
  
  <h4>Rapport de Recherche Complet</h4>
  <div class="pdf-viewer-container" style="margin: 20px 0; border: 1px solid #ddd; border-radius: 4px; overflow: hidden;">
    <iframe 
      src="/assets/rapports/TER_2025_compressed.pdf" 
      width="100%" 
      height="600px" 
      style="border: none;"
      title="Rapport - Reconstruction 3D pour Chirurgie Percutanée">
    </iframe>
    <p style="text-align: center; padding: 10px; background-color: #f5f5f5; margin: 0;">
      <a href="/assets/rapports/TER_2025_compressed.pdf" download style="text-decoration: none; color: #0366d6; font-weight: bold;">
        📄 Télécharger le rapport de recherche PDF
      </a>
    </p>
  </div>
  
  <h4>Technologies</h4>
  <p>
    <span class="tech-tag">Python</span>
    <span class="tech-tag">DepthAnything</span>
    <span class="tech-tag">Open3D</span>
    <span class="tech-tag">Computer Vision</span>
    <span class="tech-tag">Deep Learning</span>
    <span class="tech-tag">Point Cloud Processing</span>
    <span class="tech-tag">Chirurgie Assistée</span>
  </p>
</div>

<div class="project-section">
  <h3>Simulation Thermique et Électrique d'un Aimant Bitter</h3>
  <p><em>Projet M1 : Calcul Scientifique Haute Performance</em></p>
  
  <h4>Contexte et Objectifs</h4>
  <p>
    Simulation du couplage thermo-électrique d'un aimant Bitter utilisé pour générer des champs magnétiques intenses 
    en laboratoire. Le projet implémente une chaîne complète de calcul scientifique : du maillage 3D à la visualisation 
    avancée des résultats, en passant par le calcul parallèle haute performance.
  </p>
  
  <h4>Pipeline Scientifique</h4>
  <ol>
    <li><strong>Pré-traitement (Gmsh)</strong> : Modélisation géométrique et génération de maillage 3D adaptatif</li>
    <li><strong>Calcul HPC (Feel++)</strong> : Simulation parallèle sur cluster Gaya avec résolution des équations couplées (potentiel électrique + thermique)</li>
    <li><strong>Post-traitement (ParaView)</strong> : Visualisation avancée avec filtres d'extraction, champs vectoriels et iso-surfaces thermiques</li>
  </ol>
  
  <h4>Résultats</h4>
  <p>
    Distribution thermique de <strong>298K à 374K</strong> permettant l'identification des zones critiques nécessitant 
    un refroidissement optimisé. Analyse des patterns de circulation du courant électrique dans la structure.
  </p>
  
  <h4>Rapport de Projet Complet</h4>
  <div class="pdf-viewer-container" style="margin: 20px 0; border: 1px solid #ddd; border-radius: 4px; overflow: hidden;">
    <iframe 
      src="/assets/rapports/prePost.pdf" 
      width="100%" 
      height="600px" 
      style="border: none;"
      title="Rapport - Simulation Aimant Bitter">
    </iframe>
    <p style="text-align: center; padding: 10px; background-color: #f5f5f5; margin: 0;">
      <a href="/assets/rapports/prePost.pdf" download style="text-decoration: none; color: #0366d6; font-weight: bold;">
        📄 Télécharger le rapport de projet PDF
      </a>
    </p>
  </div>
  
  <h4>Technologies</h4>
  <p>
    <span class="tech-tag">Gmsh</span>
    <span class="tech-tag">Feel++</span>
    <span class="tech-tag">ParaView</span>
    <span class="tech-tag">MPI</span>
    <span class="tech-tag">HPC</span>
    <span class="tech-tag">SLURM</span>
    <span class="tech-tag">Calcul Scientifique</span>
  </p>
</div>

<div class="project-section">
  <h3>Détection de Fissures par l'Algorithme du Germe</h3>
  <p><em>Projet : Fondements et Algorithmes de l'Imagerie Numérique</em></p>
  
  <h4>Contexte et Objectifs</h4>
  <p>
    Implémentation d'une variante de l'algorithme du germe pour détecter automatiquement des fissures 
    dans des images en niveaux de gris. Le projet développe une méthode robuste d'identification et de 
    cartographie des fissures sur diverses surfaces.
  </p>
  
  <div class="image-gallery" style="display: flex; gap: 20px; margin: 20px 0; align-items: center;">
    <div style="flex: 1;">
      <img src="/assets/projects/detection-fissures/src.png" alt="Image source avec fissures" 
           style="width: 100%; border: 1px solid #ddd; border-radius: 4px;">
      <p style="text-align: center; margin-top: 10px; font-style: italic; color: #666;">
        Image source contenant les fissures à détecter
      </p>
    </div>
    <div style="flex: 1;">
      <img src="/assets/projects/detection-fissures/res.png" alt="Carte de détection des fissures" 
           style="width: 100%; border: 1px solid #ddd; border-radius: 4px;">
      <p style="text-align: center; margin-top: 10px; font-style: italic; color: #666;">
        Carte de détection : pixels blancs = fissures détectées
      </p>
    </div>
  </div>
  
  <h4>Méthodes Implémentées</h4>
  <ul>
    <li><strong>Seuillage adaptatif</strong> : Seuil dynamique s'ajustant selon la propagation et la circularité</li>
    <li><strong>Propagation par couches</strong> : Expansion isotrope évitant les biais directionnels</li>
    <li><strong>Critère de circularité</strong> : Filtrage géométrique (2R/D) pour distinguer fissures et régions compactes</li>
    <li><strong>Germes multiples</strong> : Détection automatisée de plusieurs fissures disjointes</li>
    <li><strong>Analyse topologique</strong> : Construction du graphe des composantes quasi-connexes</li>
  </ul>
  
  <h4>Pipeline de Traitement</h4>
  <ol>
    <li><strong>Initialisation</strong> : Sélection des germes et calcul de seuil automatique</li>
    <li><strong>Propagation</strong> : Extension aux 8-voisins avec contraintes de taille</li>
    <li><strong>Validation</strong> : Filtrage basé sur la circularité et rejet des fausses détections</li>
    <li><strong>Fusion</strong> : Agrégation des résultats et génération de la carte finale</li>
  </ol>
  
  <h4>Technologies</h4>
  <p>
    <span class="tech-tag">C</span>
    <span class="tech-tag">Traitement d'Images</span>
    <span class="tech-tag">Algorithmes de Croissance</span>
    <span class="tech-tag">Géométrie Discrète</span>
    <span class="tech-tag">Analyse Topologique</span>
    <span class="tech-tag">Seuillage Adaptatif</span>
    <span class="tech-tag">Vision par Ordinateur</span>
  </p>
</div>

<style>
.project-section {
  margin-bottom: 50px;
  padding-bottom: 30px;
  border-bottom: 2px solid #e1e4e8;
}

.project-section:last-child {
  border-bottom: none;
}

.project-section h3 {
  color: #2c3e50;
  margin-bottom: 20px;
  font-size: 1.5em;
}

.project-section h4 {
  color: #34495e;
  margin-top: 25px;
  margin-bottom: 15px;
  font-size: 1.2em;
}

.project-section ul, .project-section ol {
  margin-left: 20px;
  line-height: 1.8;
}

.project-section li {
  margin-bottom: 10px;
}

.tech-tag {
  display: inline-block;
  background-color: #e1f5fe;
  color: #01579b;
  padding: 5px 12px;
  margin: 5px 5px 5px 0;
  border-radius: 3px;
  font-size: 0.9em;
  font-weight: 500;
}

.pdf-viewer-container {
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}
</style>


