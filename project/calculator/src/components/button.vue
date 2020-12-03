<template>
    <button class="button"
    @click="$emit('onclick', label)"
    :class="{ double, triple, operation }">
        {{ label }}
    </button>
</template>

<script>
export default {
    props: {
        label: {},
        operation: { type: Boolean },
        double: { type: Boolean },
        triple: { type: Boolean }
    }
}

</script>

<style>
:root {
    --bg-button:  rgb(255, 225, 232);
    --border-button: solid 1px rgb(42, 42, 42);
}

.button {
    font-size: 1.4rem;
    background-color: var(--bg-button);
    border: none;
    border-right: var(--border-button);
    border-bottom: var(--border-button);
    outline: none;
}

.button:active {
    background-color:  rgb(235, 172, 182);
}

.button.double {
    grid-column: span 2;
}

.button.triple {
    grid-column: span 3;
}

.button.operation {
    background-color:  rgb(167, 39, 60);
    color: #fff;
}

.button.operation:active {
    background-color: rgb(139, 23, 42);
}
</style>