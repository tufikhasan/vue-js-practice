<script setup>
const title = "Crypto Exchanges, Not Just FTX, Are All a Mess Right Now";
const description =
  "The founders of cryptocurrency exchanges face a mountain of regulatory challenges and billions in personal losses. Binance CEO Changpeng Zhao personally lost $12 billion this year as trading volumes on Binance declined, according to a Bloomberg report Friday.…";
const url =
  "https://gizmodo.com/crypto-exchanges-ftx-binance-genesis-gemini-are-a-mess-1850968083";
const urlToImage =
  "https://i.kinja-img.com/image/upload/c_fill,h_675,pg_1,q_80,w_1200/46326bbf3c33c4ddb3f18069c82167d7.jpg";
const content =
  "The founders of cryptocurrency exchanges face a mountain of regulatory challenges and billions in personal losses. Binance CEO Changpeng Zhao personally lost $12 billion this year as trading volumes … [+1852 chars]";
const buttonText = "See more";
</script>

<!-- 
Using double curly braces "{{ }}", you can bind data directly into 
the HTML template. This is known as text interpolation.

The 'v-bind' directive instructs Vue to keep the element's id attribute in sync
with the component's dynamicId property. If the bound value is null or
undefined, then the attribute will be removed from the rendered element.

'v-bind' is so commonly used, it has a dedicated shorthand syntax ':' 
-->
<template>
  <section>
    <!-- example 1 -->
    <div>
      <img v-bind:src="urlToImage" v-bind:alt="title" />
      <h1>{{ title }}</h1>
      <p>{{ content }}</p>
      <a v-bind:href="url" target="_blank">{{ buttonText }}</a>
    </div>
    <!-- example 2 -->
    <div>
      <img :src="urlToImage" :alt="title" />
      <h1>{{ title }}</h1>
      <p>{{ content }}</p>
      <a :href="url" target="_blank">{{ buttonText }}</a>
    </div>
  </section>
</template>

<style scoped>
section {
  display: flex;
  justify-content: center;
  gap: 1rem;
}
div {
  max-width: 300px;
}
img {
  width: 100%;
}
h1 {
  font-size: 2rem;
}
</style>
