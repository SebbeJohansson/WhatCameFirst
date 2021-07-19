<i18n> 
{   
  "en": {     
    "title": "What Came First?",
    "about": "The game about trying to figure out what came first."   
  }
} 
</i18n>

<template>
  <div class="index">
    <div class="index__intro">
      <h1 class="index__title">
        {{ $t('title') }}
      </h1>
      <p class="index__about">
        {{ $t('about') }}
      </p>
    </div>
  </div>
</template>

<script lang="ts">
  import { defineComponent, ref, watch } from '@nuxtjs/composition-api';
  import { PrismaClient } from '@prisma/client'
  
  export default defineComponent({
    setup(){
      
      const getThings = async () => {
        try {
          const json = 
          console.log();
        } catch (e) {
        }
      };
    },
    async fetch() {
      const prisma = new PrismaClient()
      this.mountains = await prisma.things.findMany();
      console.log(this.mountains);
    }
  });
</script>

<style>

.index__title{
  font-family: Qahiri,sans-serif;
  font-size: 6rem;
  line-height: 6rem;
  margin: 0;
}
.index__about{
  font-family: 'Montserrat', sans-serif;
  margin: 0;
}


</style>
