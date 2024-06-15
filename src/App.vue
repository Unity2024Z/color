<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>
<!--
双色球，大乐透。
获取往届的中奖数字，
，假定一个策略，赌开奖并不随机，理由：万一开到买的人太多怎么办？这个策略讲的是开出的奖是人数较少的一类；
第二个假定，也就是官方给出的解释，50%派奖，15%发工资，35%公益，而这个派奖除去固定奖，一等，二等浮动奖按剩余金额比例分配，最高不超过500万，
但是最低可以为1元。

1.获取现有数据，json，或者爬虫爬取。
-->
<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div>
  </header>

  <main>
    <TheWelcome />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
