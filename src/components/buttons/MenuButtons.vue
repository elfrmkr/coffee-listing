<template>
    <div class="center">
        <div class="button" :class="flagAllProducts ? 'button-selected': 'buttonEmpty'" @click="showAllProducts">
            All Products
        </div>
        <div class="button" :class="flagAvailableProducts ? 'button-selected': 'buttonEmpty'" @click="showAvailableProducts">
            Available Now
        </div>
    </div>
</template>

<script>

export default {
    data() {
        return {
            flagAllProducts: true,
            flagAvailableProducts: false
        }
    },
    methods: {
        showAllProducts() {
            this.flagAllProducts = true;
            this.flagAvailableProducts = false;
            console.log("Show All Products");
        },
        showAvailableProducts() {
            this.flagAllProducts = false;
            this.flagAvailableProducts = true;
            console.log("Show Available Products");
        }
    }
}
</script>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=DM+Sans:opsz,wght@9..40,500&display=swap');
.center {
  display: flex;
  font-family: 'DM Sans', sans-serif;
  justify-content: center;
  }

.button {
    border-radius: 7px;
    padding: 6px 10px; /* Top, Right, Bottom, Left */
    color: #FEF7EE;
    font-weight: 500;
    font-size: 14px;
    margin: 10px;
    cursor: pointer;
}
.button-selected {
    background-color: #6F757C;
    transition: background-color 0.3s ease; /* Add a transition to background-color */
} 

.button-empty {
    background-color: transparent;
    transition: background-color 0.3s ease; /* Add a transition to background-color */
}
</style>