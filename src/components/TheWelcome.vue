<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Personal Profile</template>
    <p>Hello</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Education</template>
    <h4>2020-2023</h4>
    <a href="http://portal.smktarunabhakti.net/login/index.php" target="_blank">SMK TARUNA BHAKTI</a>
    <h4>
      Web Developer
    </h4>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Experience</template>
    <ul>
      <li>Scholl Agenda Guru</li>
      <li>Food Delivery Design</li>
    </ul>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Language</template>
    <ul>
      <li>English</li>
      <li>Bahasa Indonesia</li>
    </ul>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Contact</template>
    <h4>
      (+62) 819-9779-0540
    </h4>
    <h4>
      indradheepa00@gmail.com
    </h4>
    <h4>
      <a href="https://github.com/IndraDheepaBayu" target="_blank">Indra GitHub</a>
    </h4>
  </WelcomeItem>
</template>