<template>
  <q-card dark flat bordered class="experience-card">
    <q-card-section>
      <h5 class="text-white q-mb-lg">Experience</h5>

      <div v-for="(exp, index) in experiences" :key="index" class="experience-item q-mb-lg">
        <div class="row justify-between q-mb-xs">
          <span class="text-white text-weight-bold">{{ exp.title }}</span>
          <span class="text-grey-5">{{ exp.date }}</span>
        </div>
        <div class="text-primary q-mb-sm">{{ exp.company }}</div>
        <p class="text-grey-5 text-body2">{{ exp.description }}</p>
        
        <div class="q-mt-sm">
          <q-chip
            v-for="tech in exp.technologies"
            :key="tech"
            dense
            color="grey-9"
            text-color="grey-3"
            size="sm"
            class="q-mr-xs"
          >
            {{ tech }}
          </q-chip>
        </div>
      </div>
    </q-card-section>
  </q-card>
</template>

<script setup>
import { ref } from 'vue'

const experiences = ref([
  {
    title: 'Sr. Software Engineer',
    company: 'Northmarq',
    date: '2023 - Present',
    description: 'Lead DevOps Engineer responsible for CI/CD pipelines, infrastructure automation, and cloud management using Azure DevOps and Terraform. Lead projects to bridge consumers with real loan data, improving data accessibility and user experience.',
    technologies: ['C#', 'Vue.js', 'Azure DevOps', 'Terraform', 'Azure'],
  }
])
</script>

<style scoped>
.experience-card {
  background: #1a1a1a;
  border: 1px solid #333;
  height: 100%;
}

.experience-card h5 {
  margin: 0;
}

.experience-item {
  border-left: 2px solid #1976d2;
  padding-left: 16px;
}
</style>
