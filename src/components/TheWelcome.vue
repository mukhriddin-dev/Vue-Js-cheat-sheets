<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
import VueDoc1 from "../assets/docs/Vue-Essentials-Cheat-Sheet.pdf";
import VueDoc2 from "../assets/docs/Vue-3-Cheat-Sheet.pdf"
import VueDoc3 from "../assets/docs/Vue-Router-Cheat-Sheet.pdf"
import VueDoc4 from "../assets/docs/Pinia-Cheat-Sheet.pdf"
import VueDoc5 from "../assets/docs/Migration-Guide-Cheat-Sheet.pdf"
import VueDoc6 from "../assets/docs/Nuxtjs-Cheat-Sheet.pdf"
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Vue-3 Essentials cheat sheets  <span id="download">PDF</span> </template>

    <a :href="VueDoc1" target="_blank" rel="noopener">official documentation (DOWNLOAD)</a>
    
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Vue-3 Cheat sheets  <span id="download">PDF</span> </template>

   <a :href="VueDoc2" target="_blank" rel="noopener">official documentation (DOWNLOAD)</a>

    <br />
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Vue-Router cheat sheets <span id="download">PDF</span> </template>

    <a :href="VueDoc3" target="_blank" rel="noopener">official documentation (DOWNLOAD)</a>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
   <EcosystemIcon />
    </template> 
    <template #heading>Pinia cheat sheets <span id="download">PDF</span></template>
    <a :href="VueDoc4" target="_blank" rel="noopener">official documentation (DOWNLOAD)</a>
  </WelcomeItem>

    <WelcomeItem>
      <template #icon>
         <DocumentationIcon />
        <!-- <CommunityIcon /> -->
      </template>
      <template #heading>Migration guide cheat sheet  <span id="download">PDF</span></template>
      <a :href="VueDoc5" target="_blank" rel="noopener">official documentation (DOWNLOAD)</a>
    </WelcomeItem>
     <WelcomeItem>
        <template #icon>
     <EcosystemIcon />
        </template>
        <template #heading>Nuxt.js Cheat sheets   <span id="download">PDF</span></template>
        <a :href="VueDoc6" target="_blank" rel="noopener">official documentation (DOWNLOAD)</a>
      </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Follow me on Github</template>
    <a href="https://github.com/mukhriddin-dev" target="_blank" rel="noopener">@mukhriddin-web</a>.
  </WelcomeItem>
</template>
