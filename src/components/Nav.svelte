<script>
  export let segment;
</script>

<style lang='scss'>
	nav {
    background-color: #ffb677;
		display: none;

    margin-top: 50px;

    position: fixed;
    right: 0;
    bottom: 0;
    top: 0;

    width: 300px;
	}

  #navigation-switch {
    display: none;
  }

  label {
    // background: url('/menu.png') no-repeat center; // just some weird burger menu
    width: 50px;
    height: 50px;
    font-size: 2em;
    display: block;
  }

  #navigation-switch:checked ~ nav {
    display: block;
  }
</style>

<div class="navigation">
  <input type="checkbox" id="navigation-switch" />
  <label for="navigation-switch">🍔</label>
  <nav>
    <ol>
      <li>Item</li>
      <li>Item</li>
    </ol>
  </nav>
</div>
