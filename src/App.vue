<script setup>
 import { defineAsyncComponent } from 'vue'; // Importation de la fonction de Vue permettant de charger des composants de manière asynchrone
//Import Components Asynchronously
const NavBar = defineAsyncComponent(()=>import('@/components/NavBar.vue'));
const HeroSection = defineAsyncComponent(()=>import('@/components/HeroSection.vue'));
const LatestProjSection = defineAsyncComponent(()=>import('@/components/LatestProjSection.vue'));
const ExperienceAndSkills = defineAsyncComponent(()=>import('@/components/ExperienceAndSkills.vue'));
const AboutSection = defineAsyncComponent(()=>import('@/components/AboutSection.vue'));
const ContactSection = defineAsyncComponent(()=>import('@/components/ContactSection.vue'));
const Footer = defineAsyncComponent(()=>import('@/components/Footer.vue'));
const BackToTop = defineAsyncComponent(()=>import('@/components/BackToTop.vue'));
import loadingSpinner from './components/loadingSpinner.vue';
</script>

<style>

*{
  scrollbar-width: thin;
  scrollbar-color: #111827 #f1f1f1;
}
</style>

<template>
  <div class="bg-[#111827] min-h-screen">
     <Suspense>
      <template #default>
         <div>
            <NavBar />
            <HeroSection />
            <ExperienceAndSkills />
            <LatestProjSection />
            <AboutSection />
            <ContactSection />
            <Footer />
            <BackToTop />
      </div>
    </template>
    <template #fallback>
      <div class="flex justify-center items-center min-h-screen">
          <loadingSpinner />
      </div>
    </template>
  </Suspense>
  </div>
</template>
