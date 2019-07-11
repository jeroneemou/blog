<script>
  import { onMount } from "svelte";

  // let MyComponent;

  onMount(async () => {
    
    const lazyImportStackEdit = await import("stackedit-js");
    let Stackedit = lazyImportStackEdit.default;

    const el = document.querySelector("textarea");

    // Create the Stackedit object.
    const stackedit = new Stackedit();

    // Open the iframe
    stackedit.openFile({
      name: "Filename", // with a filename
      content: {
        text: el.value // and the Markdown content.
      }
    });

    // Listen to StackEdit events and apply the changes to the textarea.
    stackedit.on("fileChange", file => {
      el.value = file.content.text;
    });
  });

  export let segment;
</script>

<textarea name="stackedit" />
