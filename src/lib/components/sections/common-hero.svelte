<section>
  <div>
    <slot name="headline" tag="h2" class="headline" />
    <slot name="text" tag="p" class="text" />
  </div>
</section>

<style lang="scss">
  section {
    display: flex;
    justify-content: center;
    text-align: center;
    margin: 0 24px;
  }

  section div {
    width: min(1150px, calc(70% + 100px));
  }

  section div :global(h2) {
    font-weight: 600;
  }

  section div :global(p) {
    margin-top: 16px;
  }
</style>
