<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <h1>メイン画面</h1>
    <div class="wrapper">
      <nav>
        <RouterLink to="/">学習記録</RouterLink>
        <RouterLink to="/about">教材</RouterLink>
        <RouterLink to="/mypage">MyPage</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  background-color: #42b983;
  padding: 20px;
  color: white;
  text-align: center;
}

nav {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin-top: 10px;
}

nav a {
  color: white;
  text-decoration: none;
  font-size: 18px;
  padding: 10px 15px;
  border-radius: 5px;
  transition: background-color 0.3s;
}

nav a:hover {
  background-color: #2c3e50;
}
</style>
