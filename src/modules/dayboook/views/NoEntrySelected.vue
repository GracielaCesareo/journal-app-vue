<template>
  <div class="d-flex justify-content-center">
    <h1 clas="align-self-center">Not content selected</h1>

    <FabButton/>
  </div>
</template>

<script>
import { defineAsyncComponent } from 'vue'

export default {
     name: 'NoEntrySelected',
     components:{
    FabButton: defineAsyncComponent(() => import("@/modules/dayboook/components/FabButton")),
}
}
</script>

<style lang="scss" scoped>
    div{
        height: 100%;
    }
</style>