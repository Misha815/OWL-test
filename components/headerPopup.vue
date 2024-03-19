<template>

    <div class="popupp">
        <div class="popup__containerr">
            <div class="exit-btn">
                <div class="exit-btn__inner"><button><img src="~/assets/close-icon.svg" alt=""></button></div>
            </div>
            <div class="breadcrumb-navigation">
                <ul class="breadcrumb-navigation__inner">
                    <li><span class="new">главная</span></li>
                    <li><span>новости</span></li>
                    <li>
                        <span>Средняя ставка по ипотеке в России превысила 8%</span>
                    </li>
                </ul>

            </div>
        </div>
    </div>


</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.popupp {
    width: 1536px;
    margin: 0 auto;

    overflow: auto;



    border-radius: 16px 16px 0 0;
    background-color: #fff;
    position: relative;


    .popup__containerr {
        top: 0;

        display: flex;



        .exit-btn {
            position: absolute;
            right: 0;

            width: 128px;
            height: 80px;
            background-color: #fff;
            background-image: url('~/assets/close-btn.png');
            box-shadow: 1px 1px 5px 10px #ffffffd6;
            transition: 0.3s ease-in;

            &:hover {
                background-color: #fff;
                transition: 0.3s ease-in;
                opacity: 0.5;
            }

            .exit-btn__inner {
                position: absolute;
                right: 16px;
                top: 12px;



                button {
                    all: unset;
                    padding: 12px;



                    img {

                        width: 32px;
                        height: 32px;
                    }
                }

            }

        }

        .breadcrumb-navigation {
            width: 1056px;
            margin: 0 auto;
            margin-bottom: 4px;
            height: 80px;
            display: flex;


            .breadcrumb-navigation__inner {
                all: unset;
                display: flex;
                align-items: center;
                list-style-position: inside;

                li {


                    list-style-type: none;
                    margin-left: 8px;

                    span {
                        margin: 0 auto;
                        font-size: 16px;
                        font-weight: 500;
                    }

                    letter-spacing: 4%;
                    text-transform: uppercase;


                    &::after {

                        content: " •";
                    }

                    &:last-of-type::after {
                        content: none;
                        margin-left: 0px;

                    }

                    &:last-child {
                        color: #423f3f94;
                    }
                }
            }
        }

    }
}

@media (width: 375px) {


    .popupp {
        width: 352px;
        position: -webkit-sticky;
        position: sticky;
        top: 50px;

        margin-top: 60px;

        .popup__containerr {


            .exit-btn {
                width: 77px;
                height: 48px;
                background-color: #fff;
                background-image: url('~/assets/close-btn-mobile.png');
                box-shadow: 2px 2px 5px 20px #ffffff60;


                .exit-btn__inner {
                    position: absolute;
                    right: 7.9px;
                    top: 7.2px;

                    button {
                        all: unset;
                        padding: 7.2px;

                        img {

                            width: 19px;
                            height: 19px;
                        }
                    }

                }
            }

            .breadcrumb-navigation {
                width: 352px;
                height: 49px;
                border-radius: 30px;
                margin: 0 auto;

                .breadcrumb-navigation__inner {
                    display: flex;
                    white-space: nowrap;
                    overflow: hidden;

                    li {
                        text-transform: uppercase;

                        list-style-type: none;
                        margin-left: 8px;
                        font-size: 12px;
                        font-weight: bolder;

                        span {
                            margin: 0 auto;
                            font-size: 12px;
                            font-weight: 500;
                        }

                        letter-spacing: 4%;
                        text-transform: uppercase;

                        &::after {
                            content: " •";
                        }

                        &:first-child {
                            overflow: hidden;
                        }

                        &:last-of-type::after {
                            content: none;
                            margin-left: 0px;

                        }

                        &:last-child {
                            color: #423f3f94;
                        }
                    }
                }
            }
        }
    }
}
</style>