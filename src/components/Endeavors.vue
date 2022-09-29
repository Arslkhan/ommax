<template>
    <section>
        <div>
            <div class="single-content">
                <div class="content-div">
                    <img src="../assets/Bildschirmfoto1.png" alt="endeavors" class="w-100 h-100"/>
                </div>
                <div class="content-div margins">
                    <div class="row">
                        <div class="col-md-8 small-screen">
                            <h2>Lorem ipsum dolor sit amet</h2>
                            <div class="line-bar"></div>
                            <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing.</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="single-content">
                <div class="content-div  margin-top">
                    <div class="row">
                        <div class="col-md-8 small-screen">
                            <h2>Lorem ipsum dolor sit amet</h2>
                            <div class="line-bar"></div>
                            <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing.</p>
                        </div>
                    </div>
                </div>
                <div class="content-div ">
                    <img src="../assets/Bildschirmfoto1.png" alt="endeavors" class="w-100 h-100"/>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: "Endeavors"
    }
</script>

<style lang="scss" scoped>
    section {
        .single-content {
            display: flex;
            justify-content: center;
            color: #3D4D62;
            .content-div {
                width: 50%;
                @media only screen and (max-width: 775px) {
                    width: 100%;
                }
            }
            h3 {
                font-family: "IBMPlexBold", sans-serif;
                font-size: 30px;
                @media only screen and (max-width: 660px) {
                    font-size: 16px;
                }
            }
            p {
                font-family: "IBMPlexRegular", sans-serif;
                font-size: 16px  
            }
            .small-screen {
                margin: 0 auto;
                @media only screen and (max-width: 660px) {
                    padding-left: 3rem;
                    padding-right: 3rem;
                }
            }
            .margins {
                @media only screen and (max-width: 775px) {
                    margin: 1.5rem 0;
                }
            }
            .margin-top {
                @media only screen and (max-width: 775px) {
                    margin-top: 1.5rem;
                }
            }
        }
    }
</style>