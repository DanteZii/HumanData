
<template>
    <section class="container2">
        <h1 class="h1k">HumanData</h1>
        <div class="wrapper" v-for="item in items"
           :key="item.id">
            <nuxt-link :to="{path: item.link}"  class="alink">
            <ul class="wriper">
                <li class="image">{{item.image}}</li>
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
          link: '/people/chenguanxu'
        },
        { name: '陈晗',
          link: '/people/chenhan'
        },
        { name: '郭慧琳'},
        { name: '蛇皮'},
        { name: '王泽华'},
        { name: '子慕'},
        { name: '姜敬伟'},
        { name: '陈欣宇',
          link: '/people/chenLiangLiang'
        },
        { name: '小田'},

      ]
    }
  }
}
</script>

