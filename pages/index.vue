<template>
  <div>
    <carousel/>
    <div class="container index-container">
      <div class="row">
        <div class="col-sm-8 col-container">
          <h3 class="subtitle">診療日</h3>
          <table class="table table-bordered business-day">
            <thead>
              <tr>
                <th>月</th>
                <th>火</th>
                <th>水</th>
                <th>木</th>
                <th>金</th>
                <th class="info">土</th>
                <th class="danger">日・祝</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td class="ok">○</td>
                <td class="ok">○</td>
                <td class="ok">○</td>
                <td></td>
                <td class="ok">○</td>
                <td class="ok">○</td>
                <td></td>
              </tr>
            </tbody>
          </table>
        </div>
        <!-- <div class="col-sm-4 col-container">
          <h3 class="subtitle">診療時間</h3>
          <table class="table table-bordered business-hour">
            <tr>
              <th>午前</th>
              <td>9:00～12:00</td>
            </tr>
            <tr>
              <th>午後</th>
              <td>14:00～19:00</td>
            </tr>
          </table>
        </div> -->
      </div>
      <div class="row">
        <div class="col-sm-12">
          <h3>診療内容</h3>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Carousel from '~/components/Carousel.vue'
export default {
  components: {
    Carousel
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
