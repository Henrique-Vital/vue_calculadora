<template>
    <div class="calculator">
        <p>Digite um numero escolha o operador aritimetico digite outro numero e seu calculo sera realizado automaticamente.</p>
        <input v-model="num1" @input="calculate" type="number" placeholder="Enter number 1" />
        <select v-model="operation" @change="calculate">
            <option value="add">+</option>
            <option value="subtract">-</option>
            <option value="multiply">*</option>
            <option value="divide">/</option>
        </select>
        <input v-model="num2" @input="calculate" type="number" placeholder="Enter number 2" />
        <p>Resultado: {{ result }}</p>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                num1: 0,
                num2: 0,
                operation: 'add',
                result: 0,
            };
        },
        methods: {
            calculate() {
                switch (this.operation) {
                    case 'add':
                    this.result = this.num1 + this.num2;
                    break;
                    case 'subtract':
                    this.result = this.num1 - this.num2;
                    break;
                    case 'multiply':
                    this.result = this.num1 * this.num2;
                    break;
                    case 'divide':
                    this.result = this.num1 / this.num2;
                    break;
                    default:
                    this.result = 0;
                }
            },
        },
    };
</script>

<style>

</style>
