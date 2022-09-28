<template>
    <section>
        <div class="container">
            <div class="row">
                <h2 class="heading">
                    The leading customs agent in Europe and UK
                </h2>
                <div class="projects">
                    <div class="single-block">
                        <span class="count">20 +</span>
                        <span class="text">years of experience</span>
                    </div>
                    <div class="single-block">
                        <span class="count">400</span>
                        <span class="text">qualified customs specialists</span>
                    </div>
                    <div class="single-block">
                        <span class="count">20</span>
                        <span class="text">strategic locations</span>
                    </div>
                    <div class="single-block">
                        <span class="count">5</span>
                        <span class="text">countries</span>
                    </div>
                </div>
                <button class="btn default-btn">Get in touch</button>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: "CompanyProjects"
    };
</script>

<style lang="scss" scoped>
    section {
        background-color: #006B6E;
        color: #FFFFFF;
        padding: 4.688rem 0;
        text-align: center;
        h2 {
            font-size: 30px;
        }
        .heading {
            position: relative;
            margin-bottom: 3.75rem;
            &::after {
                content: "";
                position: absolute;
                bottom: -1.875rem;
                left: 50%;
                width: 50px;
                background: rgb(1, 164, 183);
                height: 3px;
                width: 50px;
                transform: translateX(-50%);
            }
        }
        .projects {
            display: flex;
            align-items: center;
            justify-content: space-between;
            margin-bottom: 2.5rem;
            @media only screen and (max-width: 775px) {
                    flex-wrap: wrap;
                }
            .single-block {
                font-family: "IBMPlexBold", sans-serif;
                display: flex;
                flex-direction: column;
                align-items: center;
                flex-grow: 1;
                flex-basis: 0;
                border-right: 1px solid rgba(255, 255, 255, 0.25);
                @media only screen and (max-width: 775px) {
                    flex: 100% !important;
                    border-bottom: 1px solid rgba(255, 255, 255, 0.25);
                    border-right: unset !important;
                    padding-bottom: 2rem;
                    margin-bottom: 1rem rem;
                }
            .count {
                font-size: 3.125rem;
                }
            .text {
                font-size: 1.25rem;
                }
            }
            .single-block:last-child {
                border-right: unset;
                @media only screen and (max-width: 775px) {
                    flex: 50% !important;
                    border-bottom: unset !important;
                }
            }
        }
        .default-btn {
            background: rgb(1, 164, 183) !important;
            border-radius: 5px !important;
            color: #fff !important;
            padding: 12px 10px !important;
            width: 9.375rem;
            font-family: "IBMPlexBold", sans-serif !important;
            transform: scale( 1 );
            transition: 0.15s all ease;
            justify-content: center;
            &:hover,
            &:focus {
                background: rgb(0, 126, 145) !important;
                color: #fff !important;
                transform: scale(1.06);
            }
        }
    }
</style>