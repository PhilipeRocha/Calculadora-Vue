<template>
    <div class="display">
        {{ value }}
    </div>
</template>

<script>
export default {
    props: ["value"]
}

</script>

<style>
.display {
    grid-column: span 4;
    background-color: #0003;

    display: flex;
    justify-content: flex-end;
    overflow: hidden;
    align-items: center;
    padding: 20px;
    font-size: 2.2em;
}
</style>