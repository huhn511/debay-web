<script>
  import ToggleMode from './ToggleMode.svelte'
</script>

<style>
  .nav {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    margin-bottom: 20px;
    padding: 20px;
    box-shadow: 0 0 6px rgb(0 0 0 / 25%);
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  h3 {
    margin-bottom: 0;
    font-weight: bold;
    font-size: 20px;
  }
</style>

<div class="nav">
  <h3>Debay</h3>
  <ToggleMode />
</div>
