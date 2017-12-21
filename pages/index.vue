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
        <div class="col-sm-4 col-container">
          <h3 class="subtitle">診療時間</h3>
          <table class="table table-bordered business-hour">
            <thead>
              <tr>
                <th>午前</th>
                <td>9:00～12:00</td>
              </tr>
              <tr>
                <th>午後</th>
                <td>14:00～19:00</td>
              </tr>
            </thead>
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
.business-hour {
  th, td {
    text-align: center;
  }
  th {
    background-color: lightyellow;
  }
}

.business-day {
  th {
    text-align: center;
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

.business-day {
  table-layout: fixed;
  th {
    background-color: lightyellow;
    width: 40px;
  }
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
