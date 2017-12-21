<template>
  <nav class="navbar navbar-default navbar-fixed-top">
    <div class="container">
      <div class="navbar-header">
        <a class="navbar-brand" href="#">わたなべ歯科</a>
      </div>
      <div id="navbar" class="navbar-collapse collapse">
        <ul class="nav navbar-nav">
          <li><nuxt-link to="/">TOP</nuxt-link></li>
          <li><nuxt-link to="/about">当医院について</nuxt-link></li>
          <li><nuxt-link to="/introduce">院長あいさつ</nuxt-link></li>
          <li><nuxt-link to="/access">アクセス</nuxt-link></li>
        </ul>
        <ul class="nav navbar-nav navbar-right">
          <li><a href="#"><i class="fa fa-home fa-lg fa-fw" aria-hidden="true"></i>多治見市金岡町2-104-1</a></li>
          <li><a href="tel:0572-25-3612"><i class="fa fa-phone-square fa-lg fa-fw" aria-hidden="true"></i>0572-25-3612</a></li>
        </ul>
      </div>
      <!--/.nav-collapse -->
    </div>
  </nav>
</template>

<style lang="scss" scoped>
.navbar-header a {
  font-size: 1.2em;
}
</style>
