<template>
    <div class="subject">
        <div class="subject__inner">
            <div class="media">
                <span>в СМИ</span>
            </div>
            <div class="sale">
                <span>акция</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.subject {
    .subject__inner {
        display: flex;

        .media {
            margin-right: 8px;
            border-radius: 20px;
            text-align: center;
            width: 69px;
            height: 26px;
            border: 1px solid rgba(91, 68, 129, 1);
            display: flex;
            flex-direction: row;
            justify-content: center;

            span {
                font-size: 14px;

                color: rgba(91, 68, 129, 1);
                display: flex;
                align-items: center;
            }
        }

        .sale {
            border: 1px solid rgba(202, 34, 80, 1);
            text-align: center;
            border-radius: 20px;
            width: 88px;
            height: 26px;
            display: flex;
            flex-direction: row;
            justify-content: center;

            span {
                color: rgba(202, 34, 80, 1);
                font-size: 14px;
                display: flex;
                justify-content: center;
                align-items: center;



                &::before {
                    display: flex;
                    align-items: center;
                    content: url('~/assets/icon-sale.svg');

                }
            }
        }
    }
}
</style>