<template>
  <q-card dark flat bordered class="info-json-card">
    <q-card-section>
      <pre class="json-display">{{ formattedInfo }}</pre>
    </q-card-section>
  </q-card>
</template>

<script setup>
import { computed } from 'vue'

const info = {
  name: 'Myint Myat Aung',
  title: 'Sr. Software Engineer',
  location: 'Minneapolis, MN',
  email: 'myintmyatag23@outlook.com',
  skills: ['JavaScript', 'Vue.js', 'C#', 'YAML', 'Azure'],
  languages: ['English', 'Burmese'],
  education: {
    degree: 'Bachelor of Science in Computer Science',
    university: 'St Cloud State University',
    year: '2023',
  },
  interests: ['Coding', 'Coffee', 'Dota 2', 'Counter Strike', 'Food'],
}

const formattedInfo = computed(() => {
  return JSON.stringify(info, null, 2)
})
</script>

<style scoped>
.info-json-card {
  background: #1a1a1a;
  border: 1px solid #333;
}

.json-display {
  color: #a9b7c6;
  font-family: 'Courier New', monospace;
  font-size: 14px;
  margin: 0;
  overflow-x: auto;
}

.json-display::selection {
  background: #214283;
}
</style>
