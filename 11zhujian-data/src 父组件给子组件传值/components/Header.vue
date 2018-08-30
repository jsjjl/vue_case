<template>


    <div>
    
        <h2>我是头部组件--{{a}}</h2>

      

       
    </div>
</template>




<script>
    
export default{


    data(){

        return{
            msg:'子组件的msg'
        }
    },
    methods:{
       

    },

    //https://cn.vuejs.org/v2/guide/components.html#Prop-验证
    props:{

        'a':String      
    }
    
}

</script>