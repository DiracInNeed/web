<template>
    <div class="person">
        <h2>姓名：{{ name }}</h2>
        <h2>年龄：{{ age }}</h2>
        <button @click="changeName">修改名字</button>
        <button @click="changeAge">年龄+1</button>
        <button @click="showTel">点我查看联系方式</button>
    </div>
</template>

<script lang="ts">
export default {
    name: 'App',
    data() {
        return {
            name: '张三',
            age: 18,
            tel: '13888888888'
        }
    },
    methods: {
        changeName() {
            this.name = 'zhang-san'
        },
        changeAge() {
            this.age += 1
        },
        showTel() {
            alert(this.tel)
        }
    },
}
</script>

<style>
    .person {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        height: 100%;
        width: 100%;
        background-color: #da9ff2;
        border-radius: 5dvh;
        opacity: 0.8;
    }
</style>