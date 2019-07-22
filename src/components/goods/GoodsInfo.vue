<template>
    <div class="goodsinfo-container">
    <div class="mui-card">
      <div class="mui-card-content">
        <div class="mui-card-content-inner">
          <swiper :lunbotuList="lunbotu" :isfull="false"></swiper>
        </div>
      </div>
    </div>
    </div>
</template>
<script>
import swiper from "../subcomponents/swiper.vue";

export default {
    data(){
        return {
            id:this.$route.params.id,
            lunbotu:[],
        }
    },
    created(){
        this.getLunbotu();
    }
,    methods:{
       getLunbotu(){
           this.$http.get("api/getthumimages/"+this.id).then(
               result=>{
                   if(result.body.status==0){
                       result.body.message.forEach(item=>{
                           item.img=item.src;
                       });
                       this.lunbotu=result.body.message;
                   }
               });
       }, 
    },
    components:{
        swiper
    }
}
</script>
<style lang="sass" scoped>
 
</style>
