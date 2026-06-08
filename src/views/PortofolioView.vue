<template>
  <section class="portfolio-section">
    <div class="container">
      <h1 class="main-title">Mon Portfolio</h1>
      <p class="subtitle">Découvrez mes projets et mes réalisations</p>
      
      <div class="grid">
        <ProjectCard
          v-for="project in projects"
          :key="project.title"
          :title="project.title"
          :description="project.description"
          :github="project.github"
          :demo="project.demo"
        />
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
import ProjectCard from '../components/Projectcard.vue'

const projects = [
  {
    title: "Projet Angular",
    description: "Application CRM permettant de gérer une liste de contacts avec la possibilité de les consulter, d'en ajouter, et les marquer comme favoris.",
    github: "https://github.com/paulineogrine-cloud/CRM.git",
    demo: "https://crm-project-ogrine-p.vercel.app/"
  },
  {
    title: "Projet Deep Learning",
    description: "Un classifieur intelligent basé sur l'apprentissage profond pour identifier automatiquement la présence de chats dans des images.",
    github: "https://github.com/paulineogrine-cloud/DL-Application.git"
    // pas de site → pas de demo
  },

  {
    title: "Projet Docker",
    description: "Application de vote en temps réel : une architecture Docker multi-services (Flask, Node.js, Java, PostgreSQL, Redis) permettant aux utilisateurs de voter pour leur école préférée avec synchronisation live des résultats.",
    github: "https://github.com/paulineogrine-cloud/Application-de-vote.git"
    // pas de site → pas de demo
  },
  {
    title: "Projet ETNAIR",
    description: "Plateforme ETNAIR avec API, frontend et infrastructure de déploiement pour gérer des fonctionnalités complètes autour d'un service web moderne de location de biens immobiliers.",
    github: "git@github.com:paulineogrine-cloud/ETNA_AIR.git",
    demo: "https://unread-stroller-barricade.ngrok-free.dev/home"
  }
]

</script>

<style scoped>
.portfolio-section {
  min-height: 100vh;
  background: linear-gradient(135deg, #0a0e27 0%, #1a1052 35%, #2d1b5e 65%, #16213e 100%);
  padding: 5rem 1rem;
  position: relative;
  overflow: hidden;
}

/* Effets de lumière animée */
.portfolio-section::before {
  content: '';
  position: absolute;
  top: -20%;
  right: -10%;
  width: 600px;
  height: 600px;
  background: radial-gradient(circle, rgba(169, 75, 159, 0.15) 0%, transparent 70%);
  border-radius: 50%;
  animation: float 15s ease-in-out infinite;
}

.portfolio-section::after {
  content: '';
  position: absolute;
  bottom: -20%;
  left: -10%;
  width: 600px;
  height: 600px;
  background: radial-gradient(circle, rgba(74, 26, 107, 0.1) 0%, transparent 70%);
  border-radius: 50%;
  animation: float 20s ease-in-out infinite reverse;
}

@keyframes float {
  0%, 100% { transform: translateY(0px); }
  50% { transform: translateY(30px); }
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  position: relative;
  z-index: 1;
}

.main-title {
  font-size: 3.5rem;
  font-weight: bold;
  text-align: center;
  margin-bottom: 1rem;
  color: #ffffff;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
  position: relative;
  display: inline-block;
  width: 100%;
}

.main-title::after {
  content: '';
  position: absolute;
  bottom: -15px;
  left: 50%;
  transform: translateX(-50%);
  width: 120px;
  height: 4px;
  background: linear-gradient(90deg, #4a1a6b, #a94b9f);
  border-radius: 2px;
  box-shadow: 0 2px 8px rgba(169, 75, 159, 0.3);
}

.subtitle {
  text-align: center;
  font-size: 1.25rem;
  color: #e0e7ff;
  margin-bottom: 4rem;
  margin-top: 2rem;
  font-weight: 400;
}

.grid {
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
  justify-content: center;
  margin-top: 3rem;
}

@media (max-width: 768px) {
  .main-title {
    font-size: 2.5rem;
  }
  
  .subtitle {
    font-size: 1rem;
  }
  
  .portfolio-section {
    padding: 3rem 1rem;
  }
  
  .grid {
    gap: 1.5rem;
  }
}
</style>