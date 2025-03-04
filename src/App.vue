<template>
  <div>
    <div
      class="bg-gradient-to-b from-black to-red-500 from-45% p-10 min-h-screen min-w-screen"
    >
      <NavigationMenu>
        <NavigationMenuList>
          <!-- <NavigationMenuItem>
            <Button v-if="mode == 'light'" @click="mode = 'dark'">
              Dark
            </Button>
            <Button v-else @click="mode = 'light'"> Light </Button>
          </NavigationMenuItem> -->
          <NavigationMenuItem>
            <NavigationMenuLink :class="navigationMenuTriggerStyle()" href="/"
              >Home</NavigationMenuLink
            >
          </NavigationMenuItem>
          <NavigationMenuItem>
            <NavigationMenuLink
              :class="navigationMenuTriggerStyle()"
              href="/about"
              >About</NavigationMenuLink
            >
          </NavigationMenuItem>
          <NavigationMenuItem>
            <NavigationMenuLink
              :class="navigationMenuTriggerStyle()"
              href="/contact"
              >Contact</NavigationMenuLink
            >
          </NavigationMenuItem>
          <NavigationMenuItem>
            <NavigationMenuLink
              :class="navigationMenuTriggerStyle()"
              href="/projects"
              >Projects</NavigationMenuLink
            >
          </NavigationMenuItem>
        </NavigationMenuList>
      </NavigationMenu>

      <div class="mt-20">
        <!-- two columns -->
        <div class="flex justify-center">
          <div class="w-1/2">
            <h1 class="text-6xl font-bold text-white">Hi I'm Viktoria</h1>
            <p class="text-2xl text-white mt-5">
              Software Engineer and Web Developer
            </p>
            <p class="text-white mt-5">
              I'm passionate about creating beautiful and functional websites
              and applications.
            </p>
          </div>
          <div class="w-1/2">
            <!-- <img src="@/assets/hero.svg" alt="Welcome to Reka" class="w-full" /> -->
          </div>
        </div>
      </div>
    </div>
    <!-- My skills -->
    <div
      class="bg-gradient-to-t from-black to-red-500 from-65% p-10 min-h-screen min-w-screen"
    >
      <div class="flex justify-center">
        <div class="w-1/2">
          <h1 class="text-6xl font-bold text-white">My Skills</h1>
          <p class="text-2xl text-white mt-5">
            I have experience with the following technologies:
          </p>
          <ul
            class="text-white mt-5 list-disc list-inside text-lg font-semibold space-y-2"
          >
            <li>HTML5</li>
            <li>CSS3</li>
            <li>JavaScript</li>
            <li>Vue.js</li>
            <li>React</li>
            <li>Node.js</li>
            <li>Express.js</li>
            <li>PostgreSQL</li>
            <li>MySQL</li>
            <li>MongoDB</li>
            <li>Git</li>
            <li>GitHub</li>
            <li>GitLab</li>
            <li>Heroku</li>
            <li>Netlify</li>
            <li>Vercel</li>
            <li>VS Code</li>
            <li>WebStorm</li>
            <li>Photoshop</li>
            <li>Illustrator</li>
            <li>Figma</li>
            <li>Adobe XD</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
import { Button } from "@/components/ui/button";
import {
  NavigationMenu,
  NavigationMenuItem,
  NavigationMenuLink,
  NavigationMenuList,
  navigationMenuTriggerStyle,
} from "@/components/ui/navigation-menu";

import { useColorMode } from "@vueuse/core";
import { onMounted } from "vue";

const mode = useColorMode();

onMounted(() => {});
</script>
