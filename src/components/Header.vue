<template>
  <div class="header">
    <nav class="header__nav">
      <ul class="header__list">
        <li class="header__item"><router-link to="/">HOME</router-link></li>
        <li class="header__item"><a href="">エージェント検索</a></li>
      </ul>
      <ul class="header__list">
        <li class="header__item"><a href="">ログイン</a></li>
        <li class="header__item"><a href="">会員登録</a></li>
        <li class="header__item"><router-link to="/signup">新規登録</router-link></li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped src="./components/css/header.css"></style>
