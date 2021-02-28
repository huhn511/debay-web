<script lang='ts'>
  export let imageUrl: string
  export let name: string
</script>

<style>
  .avatar {
    display: flex;
    align-items: center;
    margin-bottom: 30px;
  }

  .avatar-image {
    border-radius: 100%;
    height: var(--space-xxl);
    width: var(--space-xxl);
    border: var(--border);
    margin-right: var(--space-xs);
    background-size: cover;
  }
</style>

<div class='avatar'>
  <div 
    class='avatar-image'
    style="background-image: url('{imageUrl}')"
  />
  <span>{name}</span>
</div>
