<template>
    <div class="sidebar">
        <h2>Bienvenido</h2>
        <h3>Nombre: {{ registrarStore.nombre }}</h3>
        <h3>Email: {{ registrarStore.email }}</h3>
        <ul>
            <li><router-link to="/contador">Contador</router-link></li>
            <li><router-link to="/listadetareas">Lista de tareas</router-link></li>
            <li><router-link to="/registrar">Registro</router-link></li>
            <li><router-link to="/calcular">Calculo</router-link></li>

        </ul>
    </div>
</template>
<script setup>
    import { useRegistrarStore } from '@/modules/registro/stores/registerStore';
    const registrarStore = useRegistrarStore();

   
    
</script>
<style>
    .sidebar{
        width: 200px;
        background-color: #f0f0f0;
        padding: 20px;
    }
</style>