<script setup>
const props = defineProps(["valor1", "valor2", "trocarFiltro"]);
</script>

<template>
    <form>
        <div class="row d-flex align-items-center">
            <div class="col gap-2 d-flex">
                <input @input="props.valor1" class="form-control" type="number" />
                <input @input="props.valor2" class="form-control" type="number" />
            </div>
            <div class="col">
                <select @change="props.trocarFiltro" class="form-control text-center">
                    <option value="adicao">Adição +</option>
                    <option value="subtracao">Subtração -</option>
                    <option value="multiplicacao">Multiplicação *</option>
                    <option value="divisao">Divisão /</option>
                </select>
            </div>
        </div>
    </form>
</template>

<style scoped>
form {
    margin-top: 20px;
    padding: 20px;
    background-color: #f8f9fa;
}
</style>
