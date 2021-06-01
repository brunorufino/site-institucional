<template>
    <main>
        <section class="container">
            <h1>Contatos</h1>
            <div class="contacts"></div>
        </section>
    </main>
</template>

<script>
import api from '@/services/api.js';

export default {
    name: 'Contato',
    data(){
        return {
            contacts : []
        }
    },
    mounted(){
        api.get('/contacts.json').then(response => {
            this.contacts = response.data;
        });
    }
}
</script>

<style scoped>
    main{
        align-items: center;
    }
</style>