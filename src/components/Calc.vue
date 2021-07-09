<template>
    <div>
        <div class="calc">
            <input type="number" placeholder="op1" v-model.number="operand1" class="input">
            <input type="number" placeholder="op2" v-model.number="operand2" class="input">
            <div class="result"> = {{ result }}</div>
        </div>
        <button v-on:click="result = operand1 + operand2">+</button>
        <button v-on:click="result = operand1 - operand2">-</button>
        <button v-on:click="result = operand1 * operand2">*</button>
        <button v-on:click="result = operand1 / operand2">/</button>
        <button v-on:click="result = Math.pow(operand1, operand2)">степень</button>
        <button v-on:click="result = Math.floor(operand1 / operand2)">цел.дел.</button>
    </div>
</template>

<script>
export default {
    name: "Calc",
    data: () => ({
        operand1: null,
        operand2: null,
        result: 0,
    })
}
</script>
