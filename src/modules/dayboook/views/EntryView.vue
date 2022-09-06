<template>
  <div class="entry-title d-flex justify-contentbetween p-2">
    <div>
      <span class="text-success fs-e fw-bold">15</span>
      <span class="text-success fs-e fw-bold">Julio</span>
      <span class="text-success fs-e fw-bold">2022, jueves</span>
    </div>

    <div>
      <button class="btn btn-danger mx-2">
        Delete
        <i class="fa fa-trash-alt"></i>
      </button>
      <button class="btn btn-primary">
        Upload picture
        <i class="fa fa-upload"></i>
      </button>
    </div>
  </div>

  <hr>

  <div class="d-flex flex-column px-3 h-75">
    <textarea placeholder="What happend today?"></textarea>
    </div>

    <FabButton
      :icon="fa-sharp"
    />

    <img src="https://s3-us-west-2.amazonaws.com/melingoimages/Images/69813.jpg" alt="entry-picture" class="img-thumbnail">
</template>

<script>
import { defineAsyncComponent } from 'vue'
export default {
  name: 'EntryView',
  components: {
    FabButton: defineAsyncComponent(() => import('@/modules/dayboook/components/FabButton') )
  }
}
</script>

<style lang="scss" scoped>
  textarea{
    font-size: 20px;
    border: none;
    height: 100%;

    &:focus{
      outline: none;
    }
  }

  img{
    width: 200px;
    position: fixed;
    bottom: 150px;
    right: 20px;
    box-shadow: 0px 5px 10px rgba($color: #000000, $alpha: 0.2)
  }

</style>