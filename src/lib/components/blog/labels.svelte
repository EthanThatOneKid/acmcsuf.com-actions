<script lang="ts">
  export let data: string[] = [];
</script>

{#if data.length > 0}
  <div class="labels">
    {#each data as label}
      <small class="label">#{label}</small>
    {/each}
  </div>
{/if}

<style lang="scss">
  .labels {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 0.2em;
    font-size: 1em;
    small {
      background-color: var(--acm-light);
      border-radius: 5px;
      padding: 0.3em;
    }
  }
</style>
