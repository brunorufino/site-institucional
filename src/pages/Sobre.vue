<template>
    <main>
        <section class="container">
            <h1>Sobre</h1>
            <div class="about">{{about}}</div>
        </section>
    </main>
</template>

<script>
import api from '@/services/api.js';

export default {
    name: 'Sobre',
    data(){
        return {
            about : ''
        }
    },
    mounted(){
        api.get('/about.json').then(response => {
            this.about = response.data.about;
        });
    }
}
</script>

<style scoped>
    main{
        align-items: center;
    }
</style>