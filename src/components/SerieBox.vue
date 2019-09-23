<template>
  <div class="card">
    <div class="card-body">
      <img
        :src="serie.image"
        height="400px"
        class="card-img-top"
      >
      <h3 class="text-center">
        {{ serie.title }}
      </h3>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    serie: { type: Object, required: true }
  }

}
</script>

<style>

</style>
