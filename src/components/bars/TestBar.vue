<template>
    <div class="test-bar">
        <div class="test_bar__icon">
            <slot name="icon"></slot>
        </div>
        <div class="test-bar__title">
            <slot>Bar Title</slot>
        </div>
        <div class="test-bar__btn">
            <slot name="button"></slot>           
        </div>

    </div>
</template>

 
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Manrope:wght@500;700&display=swap');
.test-bar{
    display: flex;
    align-items: center;
    width: 100%;
    max-width: 1024px;
    height: min-content;
    min-height: 52px;
    background: linear-gradient(90deg, #E81F2F 0%, #FF8983 100%);
    border-radius: 20px;
    padding: 8px;
}
.test-bar .test-bar__title{
    font-family: 'Manrope';
    font-style: normal;
    font-weight: 700;
    font-size: 20px;
    line-height: 24px;
    color: #FFFFFF;
    padding: 6px 8px 6px 12px;
    word-break: break-all;

}
.test-bar .test-bar__btn{
    margin-left: auto;
}
</style>