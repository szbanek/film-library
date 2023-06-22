<template>
  <div class="table-responsive">
    <table class="table table-primary">
      <thead>
        <tr>
          <th v-for="caption in captions"
          :key="caption">{{ caption }}</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="movie in movies" class="">
          <td>{{ movie.title }}</td>
          <td>{{ movie.director }}</td>
          <td>{{ movie.year }}</td>
          <td>{{ movie.rate }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: 'ListElement',
  props: {
    captions: Array,
    movies: Array
  }
}
</script>