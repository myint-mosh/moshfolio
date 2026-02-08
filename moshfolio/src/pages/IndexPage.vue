<template>
  <q-page class="black-bg">
    <div class="container q-pa-lg">
      <div class="row q-col-gutter-lg">
        <!-- Profile Card -->
        <div class="col-12 col-md-4">
          <ProfileCard />
        </div>

        <!-- Experience Card -->
        <div class="col-12 col-md-8">
          <ExperienceCard />
        </div>

        <!-- Info JSON -->
        <div class="col-12">
          <InfoJSON />
        </div>
      </div>
    </div>
  </q-page>
</template>

<script setup>
import ProfileCard from 'components/ProfileCard.vue'
import ExperienceCard from 'components/ExperienceCard.vue'
import InfoJSON from 'components/InfoJSON.vue'
</script>

<style scoped>
.black-bg {
  background-color: #000000;
  min-height: 100vh;
}

.container {
  max-width: 1400px;
  margin: 0 auto;
}
</style>
