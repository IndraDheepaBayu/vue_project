<script setup>
import WelcomeItem from './WelcomeItem.vue'
import HIcon from './icons/IconHTTML.vue'
import CIcon from './icons/IconCSS.vue'
import FIcon from './icons/IconFigma.vue'
import JIcon from './icons/IconJS.vue'
import BIcon from './icons/IconB.vue'
import LIcon from './icons/IconLaravel.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <HIcon />
    </template>
    <div class="div">
      <div class="flex">
        <h3>HTML</h3>
        <h3>85%</h3>
      </div>
      <div class="skills_bar">
        <span class="skills_percetage skills_html"></span>
      </div>
    </div>  
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CIcon />
    </template>
    <div class="div">
      <div class="flex">
        <h3>CSS</h3>
        <h3>85%</h3>
      </div>
      <div class="skills_bar">
        <span class="skills_percetage skills_css"></span>
      </div>
    </div>  
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <FIcon />
    </template>
    <div class="div">
      <div class="flex">
        <h3>FIGMA</h3>
        <h3>80%</h3>
      </div>
      <div class="skills_bar">
        <span class="skills_percetage skills_figma"></span>
      </div>
    </div>   
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <JIcon />
    </template>
    <div class="div">
      <div class="flex">
        <h3>JAVA SCRIPT</h3>
        <h3>70%</h3>
      </div>
      <div class="skills_bar">
        <span class="skills_percetage skills_js"></span>
      </div>
    </div>  
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <BIcon />
    </template>
    <div class="div">
      <div class="flex">
        <h3>BOOSTRAP</h3>
        <h3>70%</h3>
      </div>
      <div class="skills_bar">
        <span class="skills_percetage skills_b"></span>
      </div>
    </div>  
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <LIcon />
    </template>
    <div class="div">
      <div class="flex">
        <h3>LARAVEL</h3>
        <h3>70%</h3>
      </div>
      <div class="skills_bar">
        <span class="skills_percetage skills_l"></span>
      </div>
    </div>  
  </WelcomeItem>

</template>

<style>
.div{
  height: 85px;
}

.flex{
  display: flex;
  justify-content: space-between;
}

h3{
  font-size: 1.2rem;
  font-weight: 500;
  margin-bottom: 0.4rem;
  color: var(--color-heading);
}

.skills_bar,
.skills_percetage{
  margin-top: 5px;
  height: 5px;
  border-radius: .25rem;
}

.skills_bar{
  background-color: #fff;
}

.skills_percetage{
  display: block;
  background-color: hsla(160, 100%, 37%, 1);
}

.skills_html{
  width: 85%;
}
.skills_css{
  width: 85%;
}
.skills_figma{
  width: 80%;
}

.skills_js, .skills_b, .skills_l{
  width: 70%;
}

</style>