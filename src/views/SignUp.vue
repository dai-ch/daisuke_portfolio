<template>
  <div class="signup">
    <Header></Header>

      <h3>新規会員登録</h3>
    <table class="table">
      <tr class="tr">
        <td>
          <label>ユーザ名</label><br/>
          <input type="text" placeholder="userName" v-model="displayName" />
        </td>
      </tr>
      <tr class="tr">
        <td>
          <label>メールアドレス</label><br/>
          <input type="text" placeholder="E-mail" v-model="mailAdress" />
        </td>
      </tr>
      <tr class="tr">
        <td>
          <label>パスワード(英数字8文字以上)</label><br/>
          <input type="password" placeholder="Password" v-model="password" />
        </td>
      </tr>
      <tr class="tr">
        <td>
          <label>パスワード</label><br/>
          <input
            type="password"
            placeholder="PasswordCheck"
            v-model="passwordCheck"
          />
        </td>
      </tr>
      <button class="btn" v-on:click="signUp">
        <router-link to="/" class="routerBtn">会員登録</router-link></button
      ><br />
      <router-link to="/login" class="routerBtn"
        >ログインはこちらから</router-link
      >
    </table>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue';

export default {
  name: 'Home',
  components: {
    Header,
  },
  data() {
    return {
      displayName: '',
      mailAdress: '',
      password: '',
      passwordCheck: '',
    };
  },
};
</script>

<style scoped src="./components/css/signup.css">

</style>
