
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
                <li class="classtime">{{itme.stime}}</li>
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
          img: 'https://firebasestorage.googleapis.com/v0/b/humandata-90d81.appspot.com/o/%E9%99%88%E5%86%A0%E6%97%AD.png?alt=media&token=a21ddd05-8dbe-4409-97ed-ee96128b26ec',
          link: '/people/chenGuanXu'
        },
        { name: '陈晗',
          img: '/people/ChenHan.png',
          link: '/people/chenHan'
        },
        { name: '郭慧琳',
          img: '/people/guoHuiLin.png',
          link: '/people/guoHuiLin'
          },
        { name: '王勇',
          img: '/people/WangYong.png',
          link: '/people/wangYong'
          },
        { name: '王泽华',
          img: '/people/WangZeHua.png',
          link: '/people/wangZeHua'
          },
        { name: '万年',
          img: '/people/WanNian.png',
          link: '/people/wanNian'
          },
        { name: '姜敬伟',
          img: '/people/JiangJIngWei.png',
          link: '/people/jiangJingWei'
          },
        { name: '陈欣宇',
          img: '/people/ChenXinYu.png',
          link: '/people/chenXinYu'
        },
        { name: '田颖竹',
          img: '/people/TianYingZhu.png',
          link: '/people/tianYingZhu'
          },
        { name: '张子木',
          img: '/people/ZhangZiMu.png',
          link: '/people/zhangZimu'
          },
        { name: '张子涵',
          img: '/people/zhangZiHan.png',
          link: '/people/zhangZiHan'
          }

      ]
    }
  }
}
</script>

