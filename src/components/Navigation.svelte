<script>
  export let movie;
</script>

<div class="wrapper">
  <div class="content">
    <a href="/">
      <p>Home</p>
    </a>
    <p>|</p>
    <p>{movie}</p>
  </div>
</div>

<style>
  .wrapper {
    display: flex;
    align-items: center;
    width: 100%;
    height: 70px;
    background: #353535;
    color: #fff;
  }

  .content {
    max-width: 1280px;
    margin: 0 auto;
    padding: 0 20px;
    width: 100%;
  }

  p {
    font-size: 22px;
    float: left;
    color: #fff;
    padding-right: 10px;
    text-decoration: none;
  }

  @media screen and (max-width: 768px) {
    p {
      font-size: 16px;
    }
  }
</style>
