<template>
  <section class="about-section">
    <div class="container">

      <!-- Timeline -->
      <div class="timeline-card">
        <h2 class="section-title">Parcours Professionnel</h2>
        
        <div class="timeline">
          <!-- 2026 Mars - Present -->
          <div class="timeline-item">
            <div class="timeline-marker">
              <div class="timeline-dot current"></div>
            </div>
            <div class="timeline-content">
              <div class="timeline-date">Mars 2026 - Présent</div>
              <h3 class="timeline-title">Formation developpeur d'application</h3>
              <ul class="timeline-list">
                <li><strong>Environnement UNIX/Linux :</strong> Scripts d'installation et configuration d'environnements
                 de travail (packages, alias, automatisation)</li>
                <li><strong>Developpement Full Stack :</strong> Développement d'une applicatrion web complète
                 (API, backend, front-end, gestion d'une base de données SQL)</li>
              </ul>
            </div>
          </div>

          <!-- 2026 Jan-Fev - Deep Learning -->
          <div class="timeline-item">
            <div class="timeline-marker">
              <div class="timeline-dot project"></div>
            </div>
            <div class="timeline-content">
              <div class="timeline-date">Janvier - Février 2026</div>
              <h3 class="timeline-title">Projets Deep Learning & Computer Vision</h3>
              <ul class="timeline-list">
                <li>Détection d'objets (YOLO)</li>
                <li>Segmentation d'images (Architecture U-net)</li>
                <li>Détection de visages (DeepFace)</li>
                <li>Implémentation de transfert de style neuronal</li>
              </ul>
            </div>
          </div>

          <!-- 2024-2025 - Imagine Optic -->
          <div class="timeline-item">
            <div class="timeline-marker">
              <div class="timeline-dot work"></div>
            </div>
            <div class="timeline-content">
              <div class="timeline-date">Janvier 2024 - Août 2025</div>
              <h3 class="timeline-title">Ingénieure Support et Application</h3>
              <p class="timeline-company">Imagine Optic, Paris/Boston</p>
              <ul class="timeline-list">
                <li>Support technique en avant et après-vente pour instruments d'imagerie</li>
                <li>Mise en place de bancs de démonstration (métrologie, optique adaptative, microscopie) chez nos 
                  client ainsi que participation à des salons professionnels
                </li>
            
              </ul>
            </div>
          </div>

          <!-- 2020-2023 - Piseo -->
          <div class="timeline-item">
            <div class="timeline-marker">
              <div class="timeline-dot work"></div>
            </div>
            <div class="timeline-content">
              <div class="timeline-date">2020 - 2023</div>
              <h3 class="timeline-title">Ingénieure Optique</h3>
              <p class="timeline-company">Piseo, Lyon</p>
              <ul class="timeline-list">
                <li>Intégration et industrialisation de systèmes optiques et d'imagerie </li>
                <li>Traitement de données et automatisation et pilotage de caméras
                  avec Python incluant le traitement d'image</li>
              </ul>
            </div>
          </div>

          <!-- 2020 - Diplôme -->
          <div class="timeline-item">
            <div class="timeline-marker">
              <div class="timeline-dot graduation"></div>
            </div>
            <div class="timeline-content">
              <div class="timeline-date">2020</div>
              <h3 class="timeline-title">🎓 Diplôme d'Ingénieure</h3>
              <p class="timeline-company">Institut d'Optique Graduate School </p>
            </div>
          </div>
        </div>
      </div>


      <!-- Compétences -->
      <div class="skills-card">
  <h2 class="section-title">Compétences</h2>
  <div class="skills-grid">
    <div>
      <h3 class="category-title">Langages</h3>
      <div class="tags">
        <span class="tag tag-blue">Python</span>
        <span class="tag tag-blue">JavaScript</span>
        <span class="tag tag-blue">Bash</span>
        <span class="tag tag-blue">Matlab</span>
      </div>
    </div>
    <div>
      <h3 class="category-title">Frontend</h3>
      <div class="tags">
        <span class="tag tag-green">Vue.js</span>
        <span class="tag tag-green">React</span>
        <span class="tag tag-green">Angular</span>
      </div>
    </div>
    <div>
      <h3 class="category-title">Backend & APIs</h3>
      <div class="tags">
        <span class="tag tag-orange">FastAPI</span>
        <span class="tag tag-orange">REST APIs</span>
        <span class="tag tag-orange">Python</span>
      </div>
    </div>
    <div>
      <h3 class="category-title">Base de données</h3>
      <div class="tags">
        <span class="tag tag-red">PostgreSQL</span>
        <span class="tag tag-red">SQLite</span>
        <span class="tag tag-red">pgAdmin</span>
      </div>
    </div>
    <div>
      <h3 class="category-title">Machine Learning</h3>
      <div class="tags">
        <span class="tag tag-purple">TensorFlow</span>
        <span class="tag tag-purple">Keras</span>
        <span class="tag tag-purple">ImageJ</span>
      </div>
    </div>
    <div>
      <h3 class="category-title">DevOps & Outils</h3>
      <div class="tags">
        <span class="tag tag-gray">Docker</span>
        <span class="tag tag-gray">Linux</span>
      </div>
    </div>
  </div>
</div>

      <!-- Certifications -->
      <div class="certification-card">
        <h2 class="cert-title">Certification Deep Learning</h2>
        <p class="cert-subtitle">Coursera Spécialisation Deep Learning</p>
        <p class="cert-author">Par Andrew Ng</p>
        <p class="cert-author"> Janvier - février 2026</p>
        <p class="cert-subtitle">
        RNN • CNN </p>
      </div>

      <!-- Certification Développeur d'Application -->
      <div class="certification-card">
        <h2 class="cert-title">Certification Développeur d'Application</h2>
        <p class="cert-subtitle">Formation Développement Full Stack</p>
        <p class="cert-author"> 09 Mars au 19 juin 2026</p>

        <a href="/attestation-deep-learning.pdf" download class="cert-download-btn">
          📄 Télécharger l'attestation
        </a>

      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'About'
}
</script>

<style scoped>
.about-section {
  min-height: 100vh;
  background: linear-gradient(135deg, #0a0e27 0%, #1a1052 35%, #2d1b5e 65%, #16213e 100%);
  padding: 5rem 1rem;
}

.container {
  max-width: 56rem;
  margin: 0 auto;
}




/* Timeline Card */
.timeline-card {
  background: white;
  border-radius: 1.5rem;
  box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
  padding: 3rem;
  margin-bottom: 2rem;
}

.timeline {
  position: relative;
  padding-left: 2rem;
}

.timeline::before {
  content: '';
  position: absolute;
  left: 0.5rem;
  top: 0;
  bottom: 0;
  width: 2px;
  background: linear-gradient(180deg, #3b82f6 0%, #8b5cf6 100%);
}

.timeline-item {
  position: relative;
  margin-bottom: 3rem;
  padding-left: 2rem;
}

.timeline-item:last-child {
  margin-bottom: 0;
}

.timeline-marker {
  position: absolute;
  left: -1.5rem;
  top: 0;
}

.timeline-dot {
  width: 1rem;
  height: 1rem;
  border-radius: 50%;
  border: 3px solid white;
  box-shadow: 0 0 0 2px #3b82f6;
}

.timeline-dot.graduation {
  background: linear-gradient(135deg, #fbbf24 0%, #f59e0b 100%);
  box-shadow: 0 0 0 3px white, 0 0 0 5px #fbbf24;
}

.timeline-dot.work {
  background: linear-gradient(135deg, #3b82f6 0%, #2563eb 100%);
  box-shadow: 0 0 0 3px white, 0 0 0 5px #3b82f6;
}

.timeline-dot.project {
  background: linear-gradient(135deg, #a855f7 0%, #9333ea 100%);
  box-shadow: 0 0 0 3px white, 0 0 0 5px #a855f7;
}

.timeline-dot.current {
  background: linear-gradient(135deg, #10b981 0%, #059669 100%);
  box-shadow: 0 0 0 3px white, 0 0 0 5px #10b981;
  animation: pulse 2s infinite;
}

@keyframes pulse {
  0%, 100% {
    box-shadow: 0 0 0 3px white, 0 0 0 5px #10b981;
  }
  50% {
    box-shadow: 0 0 0 3px white, 0 0 0 8px #10b981;
  }
}

.timeline-content {
  background: #f8fafc;
  border-radius: 1rem;
  padding: 1.5rem;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.timeline-content:hover {
  transform: translateX(5px);
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
}

.timeline-date {
  font-size: 0.875rem;
  font-weight: 600;
  color: #2563eb;
  margin-bottom: 0.5rem;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

.timeline-title {
  font-size: 1.25rem;
  font-weight: bold;
  color: #0f172a;
  margin-bottom: 0.5rem;
}

.timeline-company {
  color: #64748b;
  font-weight: 500;
  margin-bottom: 1rem;
}

.timeline-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.timeline-list li {
  position: relative;
  padding-left: 1.5rem;
  margin-bottom: 0.5rem;
  color: #475569;
  line-height: 1.6;
}

.timeline-list li::before {
  content: '→';
  position: absolute;
  left: 0;
  color: #3b82f6;
  font-weight: bold;
}
/* Skills Card */
.skills-card {
  background: white;
  border-radius: 1.5rem;
  box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
  padding: 3rem;
  margin-bottom: 2rem;
}

.section-title {
  font-size: 1.875rem;
  font-weight: bold;
  color: #0f172a;
  margin-bottom: 2rem;
  text-align: center;
}

.skills-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;
}

@media (min-width: 768px) {
  .skills-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}

.category-title {
  font-size: 0.875rem;
  font-weight: 600;
  color: #64748b;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  margin-bottom: 1rem;
}

.tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.tag {
  padding: 0.5rem 1rem;
  border-radius: 0.5rem;
  font-size: 0.875rem;
  font-weight: 500;
  color: white;
  box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
}

.tag-blue {
  background: linear-gradient(135deg, #3b82f6 0%, #2563eb 100%);
}

.tag-dark {
  background: linear-gradient(135deg, #475569 0%, #334155 100%);
}

.tag-green {
  background: linear-gradient(135deg, #10b981 0%, #059669 100%);
}

.tag-orange {
  background: linear-gradient(135deg, #f97316 0%, #ea580c 100%);
}

.tag-red {
  background: linear-gradient(135deg, #ef4444 0%, #dc2626 100%);
}

.tag-purple {
  background: linear-gradient(135deg, #a855f7 0%, #9333ea 100%);
}

.tag-gray {
  background: linear-gradient(135deg, #6b7280 0%, #4b5563 100%);
}

/* Certification Card */
.certification-card {
  background: rgba(255, 255, 255, 0.95);
  border-radius: 1.5rem;
  box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.3), 0 10px 10px -5px rgba(0, 0, 0, 0.2);
  padding: 3rem;
  margin-bottom: 2rem;
  text-align: center;
  border: 2px solid rgba(139, 92, 246, 0.3);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.certification-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 25px 35px -5px rgba(0, 0, 0, 0.4);
  border-color: rgba(139, 92, 246, 0.5);
}


.cert-title {
  font-size: 1.5rem;
  font-weight: bold;
  margin-bottom: 0.75rem;
  color: #1e293b;
}

.cert-subtitle {
  color: #475569;
  font-size: 1.125rem;
  margin-bottom: 0.5rem;
}

.cert-details {
  text-align: left;
  margin-top: 10px;
  color: #64748b;
  font-size: 0.95rem;
  line-height: 1.6;
}

.cert-author {
  color: #64748b;
  font-size: 0.875rem;
  margin-top: 0.5rem;
}

.cert-download-btn {
  display: inline-block;
  margin-top: 1.5rem;
  padding: 0.75rem 1.5rem;
  background: linear-gradient(135deg, #8b5cf6 0%, #6366f1 100%);
  color: white;
  border-radius: 0.5rem;
  font-weight: 600;
  text-decoration: none;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
}

.cert-download-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 10px 15px -3px rgba(139, 92, 246, 0.5);
  background: linear-gradient(135deg, #7c3aed 0%, #4f46e5 100%);
}

/* Responsive */
@media (min-width: 768px) {
  .skills-card,
  .timeline-card {
    padding: 3rem;
  }
}

@media (max-width: 767px) {
  .main-title {
    font-size: 2rem;
  }
  
  .skills-card,
  .certification-card,
  .timeline-card {
    padding: 2rem;
  }
  
  .timeline {
    padding-left: 1.5rem;
  }
  
  .timeline-item {
    padding-left: 1.5rem;
  }
}
</style>
