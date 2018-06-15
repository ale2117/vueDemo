<template>
    <div>
        <ul>
            <li @click="showSth(index,$event)" v-for="(name,index) in user" :key="index">
                {{name}}
            </li>
        </ul>
        <button @click="showSth">点击</button>
        <a href="#" @click.prevent>aaa</a>
        <input type="text" @keyup.enter="getkeyinfo">
    </div>
</template>
<script>
export default {
    data(){
        return {
            msg:"123",
            name:'1112',
            show:true,
            user:['aaa','bbb','ccc','ddd'],
            numbers:[1,2,3,4,5,6,7]
        }
    },
    methods:{
        showSth(data,e){
            this.numbers.filter((num) => {
                if(num % 2 === 0){
                    console.log(num)
                }
                return num % 2 === 0;
            })
            console.log(this.numbers)
            //this.user.push('eee');
            //this.user.concat("eee")
        },
        getkeyinfo(e){
            console.log(e)
        }
    }
}
</script>
<style>

</style>


