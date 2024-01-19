<script>
export default {
    data() {
        return {
            elements: [
                {
                    name: 'CHARACTERS',
                    visible: false,
                },
                {
                    name: 'COMICS',
                    visible: true,
                },
                {
                    name: 'MOVIES',
                    visible: false,
                },
                {
                    name: 'TV',
                    visible: false,
                },
                {
                    name: 'GAMES',
                    visible: false,
                },
                {
                    name: 'COLLECTIBLES',
                    visible: false,
                },
                {
                    name: 'VIDEOS',
                    visible: false,
                },
                {
                    name: 'FANS',
                    visible: false,
                },
                {
                    name: 'NEWS',
                    visible: false,
                },
                {
                    name: 'SHOP',
                    visible: false,
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
                <li v-for="(element, i) in elements" :key="i ">
                    <a href="#" :class="{'active': element.visible}">
                        {{ element.name }}
                    </a>
                </li>
            </ul>
        </div>
    </header>
</template>

<style lang="scss"> 
    
</style>    
