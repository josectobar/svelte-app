<script lang="ts">
  import blob from "./assets/images/blobs.svg";
  //   const blobsEncoded = `data:image/svg+xml,${encodeURIComponent(blobs)}`;
  let count = 0;

  function increment(): void {
    count += 1;
  }
  console.log("hit");
</script>

<h1>Animated Buttons</h1>
<p>{count}</p>
<button on:click={increment}> Click here! </button>

<button on:click={() => (count = 0)}> Reset </button>
{blob}

<style>
  #blobC {
    fill: red;
  }
</style>
