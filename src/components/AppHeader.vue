<script>
export default {
    data() {
        return {
            elements: [
                {
                    name: 'CHARACTERS',
                    visible: true,
                },
                {
                    name: 'COMICS',
                    visible: true,
                },
                {
                    name: 'MOVIES',
                    visible: true,
                },
                {
                    name: 'TV',
                    visible: true,
                },
                {
                    name: 'GAMES',
                    visible: true,
                },
                {
                    name: 'COLLECTIBLES',
                    visible: true,
                },
                {
                    name: 'VIDEOS',
                    visible: true,
                },
                {
                    name: 'FANS',
                    visible: true,
                },
                {
                    name: 'NEWS',
                    visible: true,
                },
                {
                    name: 'SHOP',
                    visible: true,
                },
            ],
        };
    },
    methods: {

    }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="image-container">
                <img src="../../public/img/dc-logo.png" alt="DC-LOGO">
            </div>
        
            <ul>
                <li v-for="(element, i) in elements">
                    <a href="#">
                        {{ element.name }}
                    </a>
                </li>
            </ul>
        </div>
    </header>
</template>

<style lang="scss"> 
    
</style>    
