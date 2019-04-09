<template>
  <section class="container">
    <div class="wraper" v-for="todo in todos"
       :key="todo.id">
      <h3 class="title">
        {{ todo.name }}
      </h3>
      <div class="wrapper2">
        <div class="radius">
            <div class="radius1">
                 <img :src="todo.img"   alt="" class="radius2">
            </div>
        </div>
      </div>
      <ul class="information">
          <li class="informationli">
              <div class="height">{{todo.height}}</div>
              <div class="heightext">身高</div>
         </li>
          <li class="informationli">
              <div class="height">{{todo.metabolism}}</div>
              <div class="heightext">代谢</div>
          </li>
          <li class="informationli">
              <div class="height">{{todo.weight}}</div>
              <div class="heightext">体重</div>
          </li>
      </ul>
      <ul class="information1">
          <li class="information2">
              <div class="informationli2">血型</div>
              <div class="informationli3">{{todo.bloodType}}</div>
          </li>
          <li class="information2">
              <div class="informationli2">星座</div>
              <div class="informationli3">{{todo.constellation}}</div>
          </li>
          <li class="information2">
              <div class="informationli2">三餐时间</div>
              <div class="informationli3">{{todo.foodTime}}</div>
          </li>
          <li class="information2">
              <div class="informationli2">睡眠时长</div>
              <div class="informationli3">{{todo.sleepTime}}</div>
          </li>
          <li class="information2">
              <div class="informationli2">入睡时间</div>
              <div class="informationli3">{{todo.sleepStart}}</div>
          </li>
          <li class="information2">
              <div class="informationli2">起床时间</div>
              <div class="informationli3">{{todo.upStrat}}</div>
          </li>
          <li class="information2">
              <div class="informationli2">运动基础</div>
              <div class="informationli3">{{todo.sf}}</div>
          </li>
          <li class="information2">
              <div class="informationli2">抽烟酗酒史</div>
              <div class="informationli3">{{todo.sd}}</div>
          </li>
          <li class="information2">
              <div class="informationli2">家族遗传</div>
              <div class="informationli3">{{todo.gd}}</div>
          </li>
          <li class="information2">
              <div class="informationli2">身体状况</div>
              <div class="informationli3">{{todo.pc}}</div>
          </li>
          <li class="information2">
              <div class="informationli2">目标</div>
              <div class="informationli3">{{todo.aims}}</div>
          </li>
          <div class="null"></div>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      todos: [
        { 
          name: '万年',
          img: '/people/wanNian.png',
          height:  '身高',
          metabolism:'代谢',
          bloodType: '血型',
          constellation:'星座',
          weight:'体重',
          foodTime:'三餐时间',
          sleepTime:'睡眠时长',
          sleepStart:'入睡时间',
          upStrat:'起床时间',
          sf:'运动基础',
          sd:'抽烟酗酒史',
          gd:'家族遗传',
          pc:'身体状况',
          aims:'目标'
          },
      ]
    }
  }
}
</script>
