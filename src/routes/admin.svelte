<script>
  import Editor from '../components/Editor.svelte'

  export let segment;
</script>

<svelte:head>
  <title>Administrator</title>
</svelte:head>

<h1>Adminstration</h1>
<Editor {segment}/>	

