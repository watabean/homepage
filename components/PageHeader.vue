<template>
  <nav class="navbar navbar-default fixed-top navbar-toggleable-md">
    <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <a class="navbar-brand" href="#">わたなべ歯科</a>
    <div class="collapse navbar-collapse" id="navbarCollapse">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item"><nuxt-link to="/" class="nav-link">TOP</nuxt-link></li>
        <li class="nav-item"><nuxt-link to="/about" class="nav-link">当医院について</nuxt-link></li>
        <li class="nav-item"><nuxt-link to="/introduce" class="nav-link">院長あいさつ</nuxt-link></li>
        <li class="nav-item"><nuxt-link to="/access" class="nav-link">アクセス</nuxt-link></li>
      </ul>
      <ul class="navbar-nav mt-2 mt-md-0">
        <li class="nav-item"><a href="#"><i class="fa fa-home fa-lg fa-fw" aria-hidden="true"></i>多治見市金岡町2-104-1</a></li>
        <li class="nav-item"><a href="tel:0572-25-3612"><i class="fa fa-phone-square fa-lg fa-fw" aria-hidden="true"></i>0572-25-3612</a></li>
      </ul>
    </div>
  </nav>
</template>

<style lang="scss" scoped>
.navbar-header a {
  font-size: 1.2em;
}
</style>
