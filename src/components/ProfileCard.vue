<template>
  <q-card dark flat bordered class="profile-card">
    <q-card-section class="text-center">
      <q-avatar size="200px" class="q-mb-md">
        <img src="https://via.placeholder.com/200" alt="Profile" />
      </q-avatar>

      <div class="description text-white">
        <h5 class="q-mb-sm">Myint Myat Aung</h5>
        <p class="text-grey-5">
          Hi, I'm Myint. I like improving engineers' happiness by building tools and automating processes. I also love reading news and gaming.
        </p>
      </div>
    </q-card-section>
  </q-card>
</template>

<script setup>
//
</script>

<style scoped>
.profile-card {
  background: #1a1a1a;
  border: 1px solid #333;
}

.social-links {
  display: flex;
  justify-content: center;
  gap: 8px;
}

.description h5 {
  margin: 0;
  color: white;
}
</style>
