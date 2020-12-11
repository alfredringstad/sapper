<script context="module">
  export async function preload() {
    await new Promise((resolve) => setTimeout(resolve, 250));
    return {
      count: 0,
    };
  }
</script>

<script>
  export let count;
</script>

<h1>{count}</h1>
<a href="/prefetch-current-page" rel="prefetch">start</a>
<a href="/prefetch-current-page/other" rel="prefetch">other</a>
