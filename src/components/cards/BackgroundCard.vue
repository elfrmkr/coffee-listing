<template>
  <div>
    <img alt="background" src="@/assets/bg-cafe.jpg" class="bg" />
    <div class="base">
      <img src="@/assets/vector.svg" alt="Vector Image" class="vector-image" />
      <Intro />
      <MenuButtons />
    </div>
  </div>
</template>


<script>
import Intro from '@/components/texts/Intro.vue'
import MenuButtons from '@/components/buttons/MenuButtons.vue';

export default {
    components: {
        Intro,
        MenuButtons,
    }
}
</script>

<style scoped>

.base {
  position: absolute;
  display: flex;
  align-items: center; /* Align to the top */
  justify-content: center; /* Align to the right */
  background: #1b1d1f;
  border-radius: 15px;
  height: 75%;
  width: 70%;
  left: 15%;
  top: 17%;
  z-index: 0;
}

.bg {
  top: 0;
  left: 0;
  position: absolute;
  width: 100%;
  min-height: 25%;
  aspect-ratio: 256 / 60; /* Set the aspect ratio to the desired width:height ratio */
  z-index: -1;
}

.vector-image {
  position: absolute;
  top: 40px; /* Adjust the top position as needed */
  right: 15%; /* Adjust the right position as needed */
  max-height: 100%;
  max-width: 100%;
  z-index: 1;
}


</style>