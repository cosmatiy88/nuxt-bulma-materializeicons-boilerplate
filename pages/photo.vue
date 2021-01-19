<template>
  <div class="content">
    <Photo
      v-for="photo in photos"
      :photo="photo"
    />
  </div>
</template>

<script>
import Photo from "../components/photo/Photo";
export default {
  name: "photo",
  components:{
    Photo
  },
  data: () =>({
    photos:[]
  }),
  mounted() {
    this.fetchPhotos()
  },
  methods: {
    fetchPhotos(){
      this.$axios.get('https://jsonplaceholder.typicode.com/photos?_limit=10')
      .then(response => this.photos = response.data)
  }
}
}
</script>

<style scoped>

</style>
