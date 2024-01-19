<script>
    export default {
        data() {
            return {
            };
        },
        props: {
            product: Object
        },
    }
</script>

<template>
    <div class="single-product">
        <div>
            <img :src="product.thumb" :alt="product.series">
        </div>

        <p>
            {{ product.series }}
        </p>
    </div>
</template>


<style lang="scss" scoped>
    .single-product {
        padding: 30px;
        width: calc(100% / 5);
        transition-duration: 0.3s;

        &:hover {
            transform: scale(1.1);
            cursor: pointer;
        }

        > div:first-child {
            width: 200px;
            height: 200px;
            margin-bottom: 15px;
            overflow: hidden;

            img {
                height: 100%;
                object-fit:fill;
            }
        }

        >div:last-child > * {
            text-transform: uppercase;
        }
    }
</style>