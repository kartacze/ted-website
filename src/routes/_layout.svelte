<script>
	import Nav from '../components/Nav.svelte';
	export let segment;
</script>

<style>
	main {
    width: 100%;
    flex: 1;
		background-color: var(--fourth-color);
    color: var(--second-color);
    display: flex;
	}

  .layout {
		margin: 0 auto;
		box-sizing: border-box;
		max-width: 56em;
    width: 100%;
    min-height: 100%;
    display: flex;
    flex-direction: column;
  }

  .in-wrapper {
		position: relative;
    margin: 2em;
    flex: 1;
  }
</style>

<Nav {segment}/>

<main>
  <div class="layout">
    <div class="in-wrapper">
	    <slot></slot>
    </div>
  </div>
</main>
