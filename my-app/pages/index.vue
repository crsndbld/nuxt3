<script setup lang="ts">

const { data, pending } = useFetch("/api/top");


console.log('data.api: ', data?.value?.api); 

</script>
<template>
  <div class="relative w-[200px] h-[200px] ">
    {{ data?.api }}
  </div>
</template>