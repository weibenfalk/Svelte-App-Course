<script>
  import { calcTime, convertMoney } from '../helpers';

  export let time;
  export let budget;
  export let revenue;
</script>

<div class="wrapper">
  <div class="content">
    <div class="content-col">
      <p>Running Time: {calcTime(time)}</p>
    </div>
    <div class="content-col">
      <p>Budget: {convertMoney(budget)}</p>
    </div>
    <div class="content-col">
      <p>Revenue: {convertMoney(revenue)}</p>
    </div>
  </div>
</div>

<style>
  .wrapper {
    display: flex;
    align-items: center;
    width: 100%;
    min-height: 100px;
    height: auto;
    background: #1c1c1c;
    padding: 20px;
    box-sizing: border-box;
    font-size: 20px;
  }

  .content {
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
    max-width: 1280px;
    width: 100%;
    margin: 0 auto;
    color: #fff;
    box-sizing: border-box;
  }

  .content-col {
    display: flex;
    align-items: center;
    justify-content: center;
    background: #333;
    border-radius: 20px;
    margin: 0 20px;
    flex: 1;
  }

  .content-col:first-child {
    margin-left: 0;
  }

  .content-col:last-child {
    margin-right: 0;
  }

  @media screen and (max-width: 768px) {
    .content {
      display: block;
    }

    .content-col {
      margin: 20px 0;
    }
  }

  @media screen and (max-width: 425px) {
    .wrapper {
      font-size: 14px;
    }
  }
</style>
