<template>
  <div
    class="mb-3 pointer p-2"
    @click="$router.push({name: 'entry', params:{id}})"
  >
    <div class="entry-container">
        <span class="text-succes fs-5 fw-bold">15</span>
        <span class="mx-1 fs-5">Julio</span>
        <span class="mx-2 fw-light">2022, jueves</span>

        <div class="entry-description">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus quisquam ducimus aliquid sed excepturi explicabo quaerat recusandae qui consequuntur, eaque fugit maxime asperiores eveniet vero velit dicta possimus temporibus. Laborum.
        </div>
    </div>

    
  </div>
</template>

<script>
export default {
    name: 'Entry'
}
</script>

<style lang="scss" scoped>
    .entry-container{
        border-bottom: solid 1px #2c3e50;
        transition: 0.2s all ease-in;

        &:hover{
            background-color: lighten($color: grey, $amount: 45);
            transition: 0.2s all ease-in;
        }

        .entry-description{
            font-size: 12px
        }
    }
</style>