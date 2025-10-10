---
layout: default
title: Accueil
---

<div style="text-align: center; margin-bottom: 3rem;">
  <h1 style="font-size: 3rem; margin-bottom: 1rem; color: #24292e;">Bienvenue</h1>
  <p style="font-size: 1.3rem; color: #586069; max-width: 600px; margin: 0 auto;">
    Je m'appelle <strong>Arnaud Goetz</strong>.<br>
    Voici mon Portfolio où je présente mon <strong>parcours scolaire</strong>, 
    mes <strong>expériences professionnelles</strong> et mes <strong>projets</strong>.
  </p>
</div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(350px, 1fr)); gap: 2.5rem; margin: 4rem 0; padding: 0 1rem;">
  
  <div style="border: 1px solid #e1e4e8; border-radius: 12px; padding: 2.5rem; background: linear-gradient(135deg, #f8f9fa 0%, #ffffff 100%); text-align: center; box-shadow: 0 4px 6px rgba(0,0,0,0.05); transition: transform 0.3s ease, box-shadow 0.3s ease;" onmouseover="this.style.transform='translateY(-5px)'; this.style.boxShadow='0 8px 25px rgba(0,0,0,0.15)'" onmouseout="this.style.transform='translateY(0)'; this.style.boxShadow='0 4px 6px rgba(0,0,0,0.05)'">
    <h2 style="margin-top: 0; color: #0366d6; font-size: 1.75rem; font-weight: 700;">Parcours Scolaire</h2>
    <a href="/parcours" style="display: inline-block; background: linear-gradient(135deg, #0366d6, #0256c7); color: white; padding: 1rem 2rem; text-decoration: none; border-radius: 8px; font-weight: 600; font-size: 1.05rem; transition: all 0.2s ease; box-shadow: 0 2px 4px rgba(3,102,214,0.2);" onmouseover="this.style.background='linear-gradient(135deg, #0256c7, #024bb3)'; this.style.transform='translateY(-1px)'" onmouseout="this.style.background='linear-gradient(135deg, #0366d6, #0256c7)'; this.style.transform='translateY(0)'">
      Découvrir mon parcours
    </a>
  </div>

  <div style="border: 1px solid #e1e4e8; border-radius: 12px; padding: 2.5rem; background: linear-gradient(135deg, #f8f9fa 0%, #ffffff 100%); text-align: center; box-shadow: 0 4px 6px rgba(0,0,0,0.05); transition: transform 0.3s ease, box-shadow 0.3s ease;" onmouseover="this.style.transform='translateY(-5px)'; this.style.boxShadow='0 8px 25px rgba(0,0,0,0.15)'" onmouseout="this.style.transform='translateY(0)'; this.style.boxShadow='0 4px 6px rgba(0,0,0,0.05)'">
    <h2 style="margin-top: 0; color: #0366d6; font-size: 1.75rem; font-weight: 700;">Expériences professionnelles</h2>
    <a href="/experiences" style="display: inline-block; background: linear-gradient(135deg, #0366d6, #0256c7); color: white; padding: 1rem 2rem; text-decoration: none; border-radius: 8px; font-weight: 600; font-size: 1.05rem; transition: all 0.2s ease; box-shadow: 0 2px 4px rgba(3,102,214,0.2);" onmouseover="this.style.background='linear-gradient(135deg, #0256c7, #024bb3)'; this.style.transform='translateY(-1px)'" onmouseout="this.style.background='linear-gradient(135deg, #0366d6, #0256c7)'; this.style.transform='translateY(0)'">
      Explorer mes expériences
    </a>
  </div>

  <div style="border: 1px solid #e1e4e8; border-radius: 12px; padding: 2.5rem; background: linear-gradient(135deg, #f8f9fa 0%, #ffffff 100%); text-align: center; box-shadow: 0 4px 6px rgba(0,0,0,0.05); transition: transform 0.3s ease, box-shadow 0.3s ease;" onmouseover="this.style.transform='translateY(-5px)'; this.style.boxShadow='0 8px 25px rgba(0,0,0,0.15)'" onmouseout="this.style.transform='translateY(0)'; this.style.boxShadow='0 4px 6px rgba(0,0,0,0.05)'">
    <h2 style="margin-top: 0; color: #0366d6; font-size: 1.75rem; font-weight: 700;">Projets</h2>
    <a href="/projets" style="display: inline-block; background: linear-gradient(135deg, #0366d6, #0256c7); color: white; padding: 1rem 2rem; text-decoration: none; border-radius: 8px; font-weight: 600; font-size: 1.05rem; transition: all 0.2s ease; box-shadow: 0 2px 4px rgba(3,102,214,0.2);" onmouseover="this.style.background='linear-gradient(135deg, #0256c7, #024bb3)'; this.style.transform='translateY(-1px)'" onmouseout="this.style.background='linear-gradient(135deg, #0366d6, #0256c7)'; this.style.transform='translateY(0)'">
      Découvrir mes projets
    </a>
  </div>
  
</div>

<div style="margin-top: 4rem; padding: 3rem; background: linear-gradient(135deg, #f6f8fa 0%, #ffffff 100%); border-radius: 16px; border: 1px solid #e1e4e8; box-shadow: 0 4px 6px rgba(0,0,0,0.05);">
  <div style="display: grid; grid-template-columns: 200px 1fr; gap: 3rem; align-items: center;">
    
    <!-- Photo de profil -->
    <div style="text-align: center;">
      <div class="profile-photo" style="width: 180px; height: 180px; border: 3px solid #0366d6; border-radius: 50%; margin: 0 auto; box-shadow: 0 4px 8px rgba(3,102,214,0.2); overflow: hidden; position: relative; background:#fff;">
     <img src="/assets/images/profile/pp.jpg" 
       alt="Photo de profil d'Arnaud Goetz" 
       style="width: 100%; height: 100%; object-fit: cover; object-position: 50% 50%; display:block;" loading="lazy">
      </div>
      <p style="margin-top: 1rem; font-size: 0.9rem; color: #586069; font-style: italic;">
        Arnaud Goetz
      </p>
    </div>
    
    <!-- Texte de présentation -->
    <div>
      <h2 style="margin: 0 0 1.5rem 0; color: #24292e; font-size: 2rem; font-weight: 700;">À propos de moi</h2>
      <div style="color:#6a737d; font-style:italic; font-size:1rem; background:#f8f9fa; border:1px dashed #d0d7de; padding:1rem 1.25rem; border-radius:8px;">
        <p style="margin: 0 0 1rem 0;">
               J’aime donner vie à des idées grâce au code et à la 3D. Ce qui me motive, c’est de <strong>comprendre un problème complexe</strong> et de le transformer en une <strong>solution claire et efficace</strong> — qu’il s’agisse d’un algorithme optimisé, d’une scène 3D fidèle ou d’une interaction fluide.
        </p>
        <p style="margin: 0 0 1rem 0;">
                Le <strong>travail en équipe</strong> compte beaucoup pour moi : j’apprends en partageant, en confrontant les approches et en construisant ensemble des projets concrets. Mon parcours en informatique et visualisation 3D m’a rendu curieux, adaptable et persévérant face aux défis techniques.
        </p>
        <p style="margin: 0;">
            Je cherche un environnement où <strong>la technologie sert la créativité</strong> — un lieu où je peux continuer à progresser tout en apportant une véritable valeur aux projets.
        </p>
      </div>
    </div>
    
  </div>
  
  <!-- Version responsive pour mobile -->
  <style>
    @media (max-width: 768px) {
      .about-section {
        grid-template-columns: 1fr !important;
        gap: 2rem !important;
        text-align: center;
      }
      
      .about-section .photo-section {
        order: -1;
      }
    }
  </style>
  
  <script>
    // Ajouter les classes responsive
    document.addEventListener('DOMContentLoaded', function() {
      const aboutGrid = document.querySelector('div[style*="grid-template-columns: 200px 1fr"]');
      if (aboutGrid) {
        aboutGrid.classList.add('about-section');
        aboutGrid.children[0].classList.add('photo-section');
      }
    });
  </script>
</div>

