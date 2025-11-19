<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <div>
    <SiteHeader />
    <main class="container">
      <section class="content">
        <HomeView />
      </section>
      <aside class="sidebar">
        <SidebarResources />
      </aside>
    </main>
    <SiteFooter />
  </div>
</template>
<script setup>
import SiteHeader from './components/SiteHeader.vue'
import SidebarResources from './components/SidebarResources.vue'
import HomeView from './views/HomeView.vue'
import SiteFooter from './components/SiteFooter.vue'
</script>
<style>
/* Minimal, temporary layout just for Exercise 1 */
* { box-sizing: border-box; }
body { margin: 0; font-family: system-ui, Arial, Helvetica, sans-serif; }
.container { display: grid; grid-template-columns: 1fr 320px; gap: 2rem; width: min(1100px,
92vw); margin: 2rem auto; }
@media (max-width: 900px) { .container { grid-template-columns: 1fr; } .sidebar { order: -1; } }
header img { height: 56px; }
header { padding: 1rem; border-bottom: 1px solid #d6e3f3; }
h1,h2,h3,p { margin: 0 0 .6rem; }
footer { padding: 1rem; text-align: center; border-top: 1px solid #d6e3f3; color: #244; }
a { color: #2a5b9e; }
</style>
