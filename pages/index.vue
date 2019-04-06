
<template>
    <section class="container2">
        <h1 class="h1k">HumanData</h1>
        <div class="wrapper" v-for="item in items"
           :key="item.id">
            <nuxt-link :to="{path: item.link}"  class="alink">
            <ul class="wriper">
                <img 
                :src="item.img" 
                class="image">
                <li class="name">{{item.name}}</li>
            </ul>
           </nuxt-link>
        </div>
        <h1></h1>
        <h1></h1>
        <h1></h1>           
    </section>
</template>
<style>

</style>

<script>
export default {
  
  data() {
    return{
      items: [
        { name: '陈冠旭',
          img: '/people/ChenGuanXu.png',
          link: '/people/chenguanxu'
        },
        { name: '陈晗',
          img: '/people/ChenGuanXu.png',
          link: '/people/chenhan'
        },
        { name: '郭慧琳',
          img: '/people/ChenXinYu.png'
          },
        { name: '蛇皮',
          img: '/people/WangYong.png'},
        { name: '王泽华',
          img: '/people/WangZeHua.png'},
        { name: '万年',
          img: '/people/WanNian.png'},
        { name: '姜敬伟',
          img: '/people/JiangJIngWei.png'},
        { name: '陈欣宇',
          img: '/people/ChenXinYu.png',
          link: '/people/chenLiangLiang'
        },
        { name: '小田',
          img: '/people/TianYingZhu.png'},
        { name: '张子木',
          img: '/people/ZhangZiMu.png'}

      ]
    }
  }
}
</script>

