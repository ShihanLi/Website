<script>
    import { onMount } from 'svelte';
  
    let items = [{ name: "Getting Started", route: "blog/yo"}];
  
    onMount(() => {
    });

  </script>
  
  <h3>Henry's Thoughts</h3>
  <ul>
    {#each items as item}
        <li ><a href={item.route}>{item.name}</a></li>
    {/each}
  </ul>
  
  <style>
    ul {
      list-style-type: disc;
    }
  </style>