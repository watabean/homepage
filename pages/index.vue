<template>
<div>
  <Header></Header>
  <div id="carousel-example-generic" class="carousel slide" data-ride="carousel">
    <!-- Indicators -->
    <ol class="carousel-indicators">
      <li data-target="#carousel-example-generic" data-slide-to="0" class="active"></li>
      <li data-target="#carousel-example-generic" data-slide-to="1"></li>
      <li data-target="#carousel-example-generic" data-slide-to="2"></li>
    </ol>

    <!-- Wrapper for slides -->
    <div class="container">
      <div class="carousel-inner" role="listbox">
        <div class="item active">
          <img src="サボテン君.jpg" alt="写真1">
        </div>
        <div class="item">
          <img src="サボテン君.jpg" alt="写真2">
        </div>
        <div class="item">
          <img src="サボテン君.jpg" alt="写真3">
        </div>
      </div>
    </div>
    <!-- Controls -->
    <a class="left carousel-control" href="#carousel-example-generic" role="button" data-slide="prev">
      <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
      <span class="sr-only">Previous</span>
    </a>
    <a class="right carousel-control" href="#carousel-example-generic" role="button" data-slide="next">
      <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
      <span class="sr-only">Next</span>
    </a>
  </div>

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
          <tr>
            <th>午前</th>
            <td>9:00～12:00</td>
          </tr>
          <tr>
            <th>午後</th>
            <td>14:00～19:00</td>
          </tr>
        </table>
      </div>
    </div>
    <div class="row">
      <div class="col-sm-12">
        <h3>診療内容</h3>
      </div>
    </div>
  </div>

  <footer class="footer">
    <div class="container">
      <p class="text-muted text-right"><span class="glyphicon glyphicon-copyright-mark" aria-hidden="true"></span> 2015 わたなべ歯科</p>
    </div>
  </footer>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Header from '~/components/Header.vue'
export default {
  components: {
    Logo,
    Header
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
