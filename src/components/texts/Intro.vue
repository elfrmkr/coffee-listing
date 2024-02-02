<template>
    <div class="center">
        <div class="header">
            Our Collection
        </div>
        <div class="body">   
            Introducing our Coffee Collection, a selection of unique coffees from different roast types and origins, expertly roasted in small batches and shipped fresh weekly.
        </div>
    </div>
</template>    

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=DM+Sans:opsz@9..40&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=DM+Sans:opsz,wght@9..40,100;9..40,400&display=swap');
.header {
    font-family: 'DM Sans', sans-serif;
    font-size: 32px;
    font-weight: 600;
    letter-spacing: 2px; /* Adjust the value based on your preference */
    color:#FEF7EE;
}
.body {
    font-family: 'DM Sans', sans-serif;
    font-size: 16px;
    font-weight: 300;
    color:#FEF7EE;
    margin-top:7px;
    text-align: center;
    letter-spacing: 2px; /* Adjust the value based on your preference */
    max-width:500px;
}

.center {
    position: absolute;
    top: 60px;
    transform: translateY(50%); /* Move the item down by 50% of its own height to vertically center it */
    text-align: center;
    z-index: 2;
}
</style>