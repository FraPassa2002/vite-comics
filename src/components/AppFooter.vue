<script>
export default {
    data() {
        return {

        };
    },
    methods: {

    }
}
</script>
            
<template>
    <footer>
        <div class="container">
            <button class="btn">SIGN-UP NOW</button>

            <div class="social-container">
                <h3>
                    FOLLOW US
                </h3>

                <ul>
                    <li>
                        <a href="#">
                            <img src="../../public/img/footer-facebook.png" alt="facebook">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../../public/img/footer-twitter.png" alt="twitter">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../../public/img/footer-youtube.png" alt="youtube">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../../public/img/footer-pinterest.png" alt="pinterest">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../../public/img/footer-periscope.png" alt="periscope">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </footer>
</template>

<style lang="scss">
    .btn{

        font-family: Roboto, sans-serif;
        font-weight: 500;
        font-size: 15px;
        color: #fff;
        background-color: #303030;
        padding: 10px 30px;
        border: solid #0282f9 3px;
        box-shadow: rgba(0, 0, 0, 0.2) 0px 12px 28px 0px, rgba(0, 0, 0, 0.1) 0px 2px 4px 0px, rgba(255, 255, 255, 0.05) 0px 0px 0px 1px inset;
        border-radius: 0px 1px 1px;
        transition : 1413ms;
        transform: translateY(0);
        display: flex;
        flex-direction: row;
        align-items: center;
        cursor: pointer;
        text-transform: uppercase;
    }

    .btn:hover{

        transition : 1413ms;
        padding: 10px 23px;
        transform : translateY(-0px);
        color: #0066cc;
        border: solid 3px #0066cc;
    }

</style>

