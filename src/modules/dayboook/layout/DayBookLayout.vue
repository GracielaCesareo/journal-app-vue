<template>
  <Navbar/>
  
  <div class="d-flex">
    <div class="col-4">
        <EntryList/>
    </div>
    <div class="col">
        <router-view></router-view>
    </div>
  </div>
</template>

<script>

import { defineAsyncComponent } from 'vue'

export default {
    name: 'DayBookLayout',
    components: {
    Navbar: defineAsyncComponent(() => import(/* webpackChunkName: 'navbar' */ "@/modules/dayboook/components/Navbar")),
    EntryList: defineAsyncComponent(() => import(/* webpackChunkName: 'entrylist' */ "@/modules/dayboook/components/EntryList")),
    
}
}
</script>

<style>

</style>