<template>
  <nav class="navbar">
    <div class="nav-container">
      <router-link to="/" class="nav-brand">PO</router-link>
      <div class="nav-links">
        <router-link to="/" class="nav-link">Accueil</router-link>
        <router-link to="/about" class="nav-link">À propos</router-link>
        <router-link to="/portfolio" class="nav-link">Portfolio</router-link>
      </div>
    </div>
  </nav>
</template>

<style scoped>
.navbar {
  background: linear-gradient(135deg, rgba(10, 14, 39, 0.95) 0%, rgba(26, 16, 82, 0.95) 100%);
  backdrop-filter: blur(10px);
  padding: 1rem 0;
  position: sticky;
  top: 0;
  z-index: 100;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
  border-bottom: 1px solid rgba(169, 75, 159, 0.2);
}

.nav-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.nav-brand {
  font-size: 1.8rem;
  font-weight: bold;
  color: #ffffff;
  text-decoration: none;
  background: linear-gradient(135deg, #a94b9f 0%, #7b2d85 100%);
  padding: 0.5rem 1rem;
  border-radius: 8px;
  transition: all 0.3s ease;
}

.nav-brand:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(169, 75, 159, 0.4);
}

.nav-links {
  display: flex;
  gap: 2rem;
}

.nav-link {
  color: #e0e7ff;
  text-decoration: none;
  font-weight: 500;
  font-size: 1.1rem;
  position: relative;
  transition: color 0.3s ease;
}

.nav-link::after {
  content: '';
  position: absolute;
  bottom: -5px;
  left: 0;
  width: 0;
  height: 2px;
  background: linear-gradient(90deg, #a94b9f, #7b2d85);
  transition: width 0.3s ease;
}

.nav-link:hover {
  color: #ffffff;
}

.nav-link:hover::after {
  width: 100%;
}

.nav-link.router-link-active {
  color: #ffffff;
}

.nav-link.router-link-active::after {
  width: 100%;
}

@media (max-width: 768px) {
  .nav-container {
    flex-direction: column;
    gap: 1rem;
  }

  .nav-links {
    gap: 1rem;
  }

  .nav-link {
    font-size: 0.9rem;
  }
}
</style>