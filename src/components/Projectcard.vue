<template>
  <div class="card">
    <h3>{{ title }}</h3>
    <p>{{ description }}</p>

    <div class="links">
      <a :href="github" target="_blank">GitHub</a>

      <!-- lien site seulement si il existe -->
      <a v-if="demo" :href="demo" target="_blank">Voir le site</a>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  title: string
  description: string
  github: string
  demo?: string
}>()
</script>

<style scoped>
.card {
  border: 1px solid #ddd;
  padding: 20px;
  border-radius: 10px;
  width: 300px;
  background: rgba(255, 255, 255, 0.95);
  display: flex;
  flex-direction: column;
  min-height: 250px;
}

h3 {
  color: #1a1464;
  margin-bottom: 10px;
}

p {
  color: #475569;
  flex-grow: 1;
}

.links {
  margin-top: auto;
  display: flex;
  gap: 10px;
}

a {
  text-decoration: none;
  color: #3b82f6;
  font-weight: 600;
  transition: color 0.3s ease;
}

a:hover {
  color: #1d4ed8;
}
</style>