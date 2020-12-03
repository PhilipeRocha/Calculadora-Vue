<template>
    <div id="app">
        <h1>Calculadora</h1>
        <Calculator />
    </div>
</template>

<script>
import Calculator from './main/calculator.vue'
export default {
    components: {
        Calculator
    }
}

</script>


<style>
@font-face {
    font-family: "RobotoMono";
    src: url("./fonts/RobotoMono-Thin.ttf")
}

* {
    font-family: "RobotoMono", monospace;
}

body {
    margin: 0
}

#app {
    display: flex;
    flex-direction: column;
    height: 100vh;
    justify-content: center;
    align-items: center;
    text-align: center;

    color: #ffff;
    background: linear-gradient(to right, rgb(195, 20, 50), rgb(36, 11, 54));
}
</style>