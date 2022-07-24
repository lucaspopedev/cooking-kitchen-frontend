<template>
  <div>

    <Sidebar />

   <div class="container mx-auto">
     <Nuxt />
   </div>
  
  </div>
</template>

<script>
import Sidebar from '~/components/system/Sidebar.vue';
export default {
    components: { Sidebar }
}
</script>
