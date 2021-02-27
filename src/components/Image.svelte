<script>
  export let imageUrl
</script>

<style>
  .image {
    background-size: cover;
    width: 100%;
    height: 300px;
    margin-bottom: 30px;
    border-radius: 10px;
  }
</style>

<div 
  class="image" 
  style="background-image: url('{imageUrl}')"
/>
