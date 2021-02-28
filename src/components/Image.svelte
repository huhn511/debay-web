<script lang='ts'>
  export let imageUrl: string
</script>

<style>
  .image {
    background-size: cover;
    width: 100%;
    height: 300px;
    margin-bottom: var(--space-lg);
    border-radius: var(--radius);
  }
</style>

<div 
  class='image' 
  style="background-image: url('{imageUrl}')"
/>
