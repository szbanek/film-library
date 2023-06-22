<template>
  <ModalWindow :visible="visible">
    <div v-for="caption in captions" class="mb-3">
      <label for="" class="form-label">{{ caption }}</label>
      <input type="text"
        class="form-control" name="" id="" aria-describedby="helpId" placeholder="">
    </div>
    <button type="submit" class="btn btn-primary">Submit</button>
  </ModalWindow>
</template>

<script>
import ModalWindow from './ModalWindow.vue';

export default {
  name: "NewMovieForm",
  components: {
    ModalWindow,
  },
  props: {
    visible: Boolean,
    captions: Array
  }
}

</script>