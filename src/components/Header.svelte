<script>
  import Nav from './Nav.svelte';

  export let segment;
</script>

<style lang="scss">
  header {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    background-color: #616f39;
  }

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
</style>

<header>
  <div class="container">
    <img src="https://place-hold.it/100px50px" alt="">
    <Nav {segment}/>
  </div>
</header>
