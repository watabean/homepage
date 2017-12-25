<template>
  <div>
    <carousel></carousel>
    <div class="container index-container">
      <div class="row">
        <div class="col-sm-12 col-container business-day">
          <h3 class="subtitle">診療時間のご案内</h3>
          <table class="table table-bordered">
            <thead>
              <tr>
                <th class="col-sm-5">診療時間</th>
                <th class="col-sm-1">月</th>
                <th class="col-sm-1">火</th>
                <th class="col-sm-1">水</th>
                <th class="col-sm-1">木</th>
                <th class="col-sm-1">金</th>
                <th class="info col-sm-1">土</th>
                <th class="danger col-sm-1">日/祝</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>9:00～12:00</td>
                <td class="ok">○</td>
                <td class="ok">○</td>
                <td class="ok">○</td>
                <td></td>
                <td class="ok">○</td>
                <td class="ok">○</td>
                <td></td>
              </tr>
              <tr>
                <td>14:00～19:00</td>
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

<style lang="scss" scoped>
.business-day {
  th {
    text-align: center;
    table-layout: fixed;
    background-color: lightyellow;
  }
  td {
    text-align: center;
    &:empty {
      background-color: lightgrey;
    }
  }
}

.ok {
  font-size: 2em;
}

.subtitle {
  background: linear-gradient(transparent 70%, #a7d6ff 70%);
}

/* .col-container {
    border: solid 3px #364e96; 線色
    border-radius: 0.5em; 角丸
} */

.index-container {
  margin-top: 30px;
}
</style>
