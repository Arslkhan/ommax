<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col-md-6">
                    <div class="img-bg">
                        <img src="../assets/partners.png" alt="partners" >
                    </div>
                </div>
                <div class="col-md-6">
                    <div class="work-with">
                        <h2 >Who we work with</h2>
                        <div class="line-bar"></div>
                        <p>We are the trusted partner for customs matters of more than 7000 companies across Europe. Since 20 years we successfully operate with customers from small and large good owners to freight forwarders and digital platforms across various industries.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Partners"
};
</script>

<style lang="scss" scoped>
section {
    padding: 60px 0;
    @media only screen and (max-width: 660px) {
        padding: 0;
    }
    .img-bg {
        background-color: #F0F0F0;  
        width: 511px;
        height: 281px;
    }
    .work-with {
        padding: 40px 20px;
        @media only screen and (max-width: 660px) {
            padding: 10px;
        }
    }
    h2 {
        font-family: "IBMPlexBold", sans-serif;
        font-size: 30px;
    }
    p {
        font-family: "IBMPlexRegular", sans-serif;
        color: #3D4D62;
        font-size: 16px;
    }
}
</style>