<script setup lang="ts">

</script>

<script setup>
const links = [
  { href: "https://www.cdc.gov/physicalactivity/basics/pa-health/index.htm", text: "Physical activity and health" },
  { href: "http://www.heart.org/HEARTORG/HealthyLiving/PhysicalActivity/FitnessBasics/FlexibilityExercise-Stretching_UCM_464002_Article.jsp#.WpB8zIPwaUl", text: "Stretching exercises" },
  { href: "http://www.heart.org/HEARTORG/HealthyLiving/PhysicalActivity/FitnessBasics/Strengthand-Resistance-Training-Exercise_UCM_462357_Article.jsp#.WpCPxIPwaUl", text: "Strengthtraining" },
  { href: "https://www.health.harvard.edu/exercise-and-fitness/interval-training-for-a-strongerheart", text: "Cardiovascular training" },
  { href: "https://www.self.com/gallery/power-yoga-workout", text: "Yoga workout" }
]
</script>
<template>
  <div>
    <h2>Additional resources</h2>
    <ul>
      <li v-for="link in links" :key="link.href">
        <a :href="link.href" target="_blank" rel="noopener noreferrer">{{ link.text }}</a>
      </li>
    </ul>
  </div>
</template>

<style scoped>

</style>