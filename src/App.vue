<template>
  <p>줄임말과 원래말을 입력하세요</p>
  <input type="text" v-bind:value="abbr" />
  <input type="text" v-model="normal" />
  <hr/>
  <abbr v-bind:title="normal">{{abbr}}</abbr>
</template>
<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup

</script>
<script>
import {ref} from 'vue';

export default {
  setup(){
    const abbr = ref('DOPT')
    const normal = ref('Dong Project Team')
    return {
      abbr,
      normal,
    }
  }
}
</script>
<style scoped>
</style>
