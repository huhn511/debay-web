<script>
  import ToggleMode from './ToggleMode.svelte'
</script>

<style>
  .nav {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    margin-bottom: var(--space-md);
    padding: var(--space-lg);
    box-shadow: var(--box-shadow);
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: var(--color-layout);
    z-index: 1;
  }
  
  h3 {
    margin: 0;
    font-weight: bold;
    font-size: var(--space-lg);
  }
</style>

<div class='nav'>
  <h3>Debay</h3>
  <ToggleMode />
</div>
