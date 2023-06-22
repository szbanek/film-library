<template>
  <div class="d-grid gap-2">
    <button type="button" name="" id="" class="btn btn-primary" onclick="">New movie</button>
  </div>
  <!-- TODO button w innej klasie -->
  <MoviesList :captions="captions" :movies="movies"></MoviesList>
  <NewMovieForm visible="true" :captions="captions">
    
  </NewMovieForm>
</template>

<script>
import MoviesList from './components/MoviesList.vue';
import NewMovieForm from './components/NewMovieForm.vue';

export default {
  name: "App",
  components: {
    MoviesList,
    NewMovieForm
  },
  data() {
    return {
      captions: [
        'Title',
        'Director',
        'Year',
        'Rate'
      ],
      movies: [
        {
          title: 'Gwiezdne Wojny',
          director: 'Adams',
          year: '1999',
          rate: '4.5'
        },
        {
          title: 'Gwiezdne Wojny2',
          director: 'Adams',
          year: '1999',
          rate: '4.5'
        }
      ]
    }
  }
}
</script>
