<script>
  export let imageUrl
  export let name
</script>

<style>
  
  .avatar {
    display: flex;
    align-items: center;
    margin-bottom: 30px;
  }

  .avatar-image {
    border-radius: 30px;
    height: 30px;
    width: 30px;
    margin-right: 15px;
    background-size: cover;
  }

</style>

<div class="avatar">
  <div 
    class="avatar-image"
    style="background-image: url('{imageUrl}')"
  />
  <span>{name}</span>
</div>
