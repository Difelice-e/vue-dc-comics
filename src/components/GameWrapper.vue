<template>
  <div class="game__item">
    <figure>
      <img class="game__image" :src="thumb" alt="" />
    </figure>

    <h4 class="game__title">{{ title }}</h4>
  </div>
</template>

<script>
export default {
  name: "GameWrapper",
  props: ["title", "thumb"],
};
</script>

<style lang="scss" scoped>
.game__item {
    width: calc((100% / 6) - 20px);
    padding: 10px 0;
        
        .game__image {
            object-fit: cover;
            object-position: center;
            aspect-ratio: 1/1;
            width: 100%;
        }
        

        .game__title {
            text-transform: uppercase;
            color: white;
            font-size: 0.7rem;
            padding-top: 15px;
        }
}   
</style>