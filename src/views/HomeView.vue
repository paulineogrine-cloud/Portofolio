<template>
  <section class="hero">
    <div class="overlay">
      <h1>Pauline Ogriné</h1>
      <h2>Ingénieure Optique • Computer Vision • Future Data Engineer</h2>
      <p>Ingénieure diplômée en optique, je me spécialise aujourd'hui en Data Engineering. 
        Je conçois et développe des pipelines de données robustes ainsi que des outils d'automatisation 
        pour la collecte, le traitement, le stockage et l'analyse de données. 
        Mon parcours en traitement d'images me permet d'aborder des problématiques mêlant qualité des données et intelligence artificielle.</p>

      <div class="buttons">
        <router-link to="/portfolio" class="btn">Voir mon travail</router-link>
      </div>
    </div>
  </section>
</template>

<style scoped>
.hero {
  height: 80vh;
  background: linear-gradient(135deg, #0a0e27 0%, #1a1052 35%, #2d1b5e 65%, #16213e 100%);
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  text-align: center;
  position: relative;
  overflow: hidden;
}

/* Effet de lumière tournant */
.hero::before {
  content: '';
  position: absolute;
  top: -50%;
  right: -50%;
  width: 200%;
  height: 200%;
  background: radial-gradient(circle, rgba(255,255,255,0.08) 0%, transparent 70%);
  animation: rotate 20s linear infinite;
}

@keyframes rotate {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

.overlay {
  max-width: 700px;
  position: relative;
  z-index: 1;
}

h1 {
  font-size: 3rem;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
}

h2 {
  margin: 10px 0;
  font-weight: 400;
  text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
}

p {
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.15);
}

.buttons {
  margin-top: 20px;
}

.btn {
  background: white;
  color: #4a1a6b;
  padding: 12px 28px;
  border-radius: 8px;
  margin: 5px;
  text-decoration: none;
  font-weight: 600;
  transition: all 0.3s ease;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
}

.btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.3);
  background: linear-gradient(135deg, #ffffff 0%, #f0e6ff 100%);
}

.btn.secondary {
  background: transparent;
  border: 2px solid white;
  color: white;
}

.btn.secondary:hover {
  background: rgba(255, 255, 255, 0.1);
}

.cards {
  display: flex;
  justify-content: center;
  gap: 20px;
  padding: 40px;
}

.card {
  width: 250px;
  padding: 20px;
  border-radius: 15px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}
</style>