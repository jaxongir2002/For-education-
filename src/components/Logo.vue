<template>
    <div class="logo" v-on:click="home">
        <img src="../assets/logo.png" alt="Logo" class="logo__img">
    
    </div>
</template>

<script>
export default {
    name: "Logo",
    methods: {
        home() {
            window.location.href = "/";
        }
    }
}
</script>

<style lang="scss">
$logo-size: 3rem;

.logo {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 30rem !important;

    position: absolute;
    left: var(--logo-sideSpacing);

    font-weight: 600;

    cursor: pointer;
    

    &__img {
        width: 50%
       
    }


  
}
</style>