vueファイル、下記のコードを実行すると、$15をこえる15.990000000000002のような記述になる。原因と解決策を簡単にわかりやすく説明してほしい。


<script setup>
  import { ref, reactive } from 'vue'

  const title = ref('Vue.js Course')
  
  // コースの価格表示
  let price = ref(9.99)
  
  // priceの価格を1ドルずつあげる処理
  function increment(){
    price.value += 1
  }

  const user = reactive({
    name : 'Yokohama Taro',
    age  : 20
  })

  const contentsInfo = {
    contents : ref(10)
  }
</script>

<template>
  <h1>{{ title }}</h1>
  <h2>Price : ${{ price - 1}}</h2>
  <button @click="increment">Button</button>

  <h3>User Name : {{ user.name }} </h3>
  <h3>contents Info : {{ contentsInfo.contents.value + 1}}</h3>
</template>

<style></style>