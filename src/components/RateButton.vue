
<template>
  <div class="rate" :class="'rate_color_'+ 2" :title="title">
    <!-- Отображение рейтинга если такой есть -->
    <a>2</a>
  </div>
</template>

<script>
// Кнопка/блок рейтинга появляется слева, меняет цвет в зависимости от рейтинга от 1 до 5
export default {
  name: "rate-button",
  props: {
    imdb_rate: [String, Number]
  },
  computed: {
    title: function() {
      return `Репутация фильма на IMDB: ${this.imdb_rate}`;
    }
  }
};
</script>

<style scoped>
.rate {
  cursor: pointer;
  position: relative;
  border-top-right-radius: 38%;
  border-bottom-right-radius: 38%;
  color: black !important;
  align-self: flex-start;
  margin-top: 14%;
  height: 30%;
  width: 10%;
  font-size: 3.3em;
  font-weight: bold;
}
.rate_color_0 {
  background: rgba(255, 250, 250, 0.8);
  color: #333;
}
.rate_color_2 {
  background: rgba(94, 2, 2, 0.8) !important;
  color: #5C124A;
}
.rate_color_3 {
  background: rgba(255, 218, 185, 0.8) !important;
  color: #4C2E0F;
}
.rate_color_4 {
  background: rgba(126, 192, 238, 0.8) !important;
  color: #002E4C;
}
.rate_color_5 {
  background: rgba(60, 179, 113, 0.8) !important;
  color: #002E00;
  color: black;
}
</style>