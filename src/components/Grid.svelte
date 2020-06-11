<script>
  export let header;
</script>

<div class="wrapper">
  <h1>{header}</h1>
  <div class="content">
    <slot />
  </div>
</div>

<style>
  .wrapper {
    max-width: 1280px;
    margin: 0 auto;
    padding: 0 20px;
  }

  .content {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    grid-gap: 40px;
  }

  h1 {
    font-family: 'Abel', sans-serif;
    font-size: 22px;
  }

  @media screen and (min-width: 375px) {
    .content {
      grid-template-columns: repeat(2, minmax(100px, 1fr));
    }
  }

  @media screen and (min-width: 600px) {
    .content {
      grid-template-columns: repeat(3, minmax(100px, 1fr));
    }
  }

  @media screen and (min-width: 768px) {
    .content {
      grid-template-columns: repeat(4, minmax(100px, 1fr));
    }

    h1 {
      font-size: 42px;
    }
  }

  @media screen and (min-width: 1024px) {
    .content {
      grid-template-columns: repeat(5, minmax(100px, 1fr));
    }
  }
</style>
