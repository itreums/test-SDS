<template>
    <div class="icon-wrap">
        <img :src="path+icon" alt="" class="test-icon">
        </div>
</template>
<script>
export default{
    props:['icon'],
    data(){
        return{
            path:'/icons/'
        }
    }
}
</script>
<style scoped>
.icon-wrap{
    width: 36px;
    height: 36px;
    display: flex;
    align-items: center;
    justify-content: center;
}
</style>