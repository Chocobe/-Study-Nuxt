<template>
  <div>
    <header>
      <h1>{{ $route.name }} 페이지</h1>
      <nav>
        <ul class="menu">
          <li class="menu__item"><NuxtLink to="/">홈</NuxtLink></li>
          <li class="menu__item"><NuxtLink to="/main"> 메인</NuxtLink></li>
          <li class="menu__item"><NuxtLink to="/product">상품</NuxtLink></li>
        </ul>
      </nav>
    </header>
    <Nuxt />
  </div>
</template>

<script>
export default {
  //
}
</script>

<style>
.menu {
  margin: 20px;
  list-style: none;

  display: flex;
  justify-content: flex-start;
  align-items: center;
}

.menu__item {
  margin-right: 20px;
}

.menu__item:last-child {
  margin-right: 0;
}
</style>