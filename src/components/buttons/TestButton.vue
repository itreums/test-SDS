<template>
    <button class="btn btn_standart">
        <slot>Button</slot>
    </button>
</template>

<style scoped>
.btn{
    font-family: 'Manrope';
    border:none;
    border-radius: 12px;
    padding: 8px 16px;
    font-weight: 500;
    font-size: 14px;
    line-height: 20px;
    text-align: center;
    width: max-content;
    letter-spacing: 0.0025em;
}
.btn:hover{
    cursor: pointer;
    background-color: #ebebeb;
}
.btn_standart{
    background-color: #ffffff;
    color: #E81F2F;
}
</style>