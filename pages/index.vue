<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest tech news!</h1>
    </section>
    <section class="featured-posts">

      <PostPreview 
       id="1"
       thumbnail="https://images.pexels.com/photos/276452/pexels-photo-276452.jpeg"
       title="Hello there 1 "
       previewText="This my frist post ! 1 "
      />

      <PostPreview 
       id="2"
       thumbnail="https://images.pexels.com/photos/574070/pexels-photo-574070.jpeg"
       title="Hello there 2 "
       previewText="This my frist post ! 2 "
      />

      <PostPreview 
       id="3"
       thumbnail="https://images.pexels.com/photos/5240544/pexels-photo-5240544.jpeg"
       title="Hello there 3 "
       previewText="This my frist post ! 3 "
      />

    </section>
  </div>
</template>


<script>
import PostPreview from '@/components/Posts/PostPreview.vue'
export default {
  components: {
    PostPreview
  }
}
</script>


<style scoped>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-image : url('~assets/images/pexels-rodolfo-clix.jpg');
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

</style>
