<template>
    <div>
        <h1>{{title}}</h1>
        <h2>Count: {{ count }}</h2>
        <button @click="increment">+</button>
        <button @click="decrement">-</button>
    </div>
</template>

<script>
export default{
    name: 'Counter',
    props: {
        title: String,
        default: ()=> 'Counter'
    },
    data(){
        return{
            count:0
        }
    },
    methods:{
        increment(){
            this.count++
        },
        decrement(){
            this.count--
        }
    }
}
</script>