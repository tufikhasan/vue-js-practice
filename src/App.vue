<script setup>
// object
const article = {
  title: "Crypto Exchanges, Not Just FTX, Are All a Mess Right Now",
  description:
    "The founders of cryptocurrency exchanges face a mountain of regulatory challenges and billions in personal losses. Binance CEO Changpeng Zhao personally lost $12 billion this year as trading volumes on Binance declined, according to a Bloomberg report Friday.…",
  url: "https://gizmodo.com/crypto-exchanges-ftx-binance-genesis-gemini-are-a-mess-1850968083",
  urlToImage:
    "https://i.kinja-img.com/image/upload/c_fill,h_675,pg_1,q_80,w_1200/46326bbf3c33c4ddb3f18069c82167d7.jpg",
  content:
    "The founders of cryptocurrency exchanges face a mountain of regulatory challenges and billions in personal losses. Binance CEO Changpeng Zhao personally lost $12 billion this year as trading volumes … [+1852 chars]",
  buttonText: "See more",
};
// array
const news = [
  {
    title: "Crypto Exchanges, Not Just FTX, Are All a Mess Right Now",
    description:
      "The founders of cryptocurrency exchanges face a mountain of regulatory challenges and billions in personal losses. Binance CEO Changpeng Zhao personally lost $12 billion this year as trading volumes on Binance declined, according to a Bloomberg report Friday.…",
    url: "https://gizmodo.com/crypto-exchanges-ftx-binance-genesis-gemini-are-a-mess-1850968083",
    urlToImage:
      "https://i.kinja-img.com/image/upload/c_fill,h_675,pg_1,q_80,w_1200/46326bbf3c33c4ddb3f18069c82167d7.jpg",
    content:
      "The founders of cryptocurrency exchanges face a mountain of regulatory challenges and billions in personal losses. Binance CEO Changpeng Zhao personally lost $12 billion this year as trading volumes … [+1852 chars]",
    buttonText: "See more",
  },
];
</script>
<template>
  <section>
    <!-- Display object data -->
    <div>
      <img v-bind:src="article.urlToImage" v-bind:alt="article.title" />
      <h1>{{ article.title }}</h1>
      <p>{{ article.content }}</p>
      <a v-bind:href="article.url" target="_blank">{{ article.buttonText }}</a>
    </div>
    <!-- Display array data -->
    <div>
      <img v-bind:src="news[0].urlToImage" v-bind:alt="news[0].title" />
      <h1>{{ news[0].title }}</h1>
      <p>{{ news[0].content }}</p>
      <a v-bind:href="news[0].url" target="_blank">{{ news[0].buttonText }}</a>
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
