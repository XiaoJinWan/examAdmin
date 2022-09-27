<template>
  <div class="home">
    <div class="cont">
      <div class="left" @click="cont1">
        五栋-1单元-选择栋
      </div>
      <div class="right right1">
        <div class="box">
          <table>
            <tr>
              <td @click="td($event)">11楼</td>
              <td @click="td($event)">12楼</td>
              <td @click="td($event)">13楼</td>
              <td @click="td($event)">14楼</td>
              <td @click="td($event)">15楼</td>
              <td @click="td($event)">16楼</td>
              <td @click="td($event)">17楼</td>
              <td @click="td($event)">18楼</td>
            </tr>
          </table>
        </div>
        <div class="box">
          <table>
            <tr>
              <td @click="td($event)">11楼</td>
              <td @click="td($event)">12楼</td>
              <td @click="td($event)">13楼</td>
              <td @click="td($event)">14楼</td>
              <td @click="td($event)">15楼</td>
              <td @click="td($event)">16楼</td>
              <td @click="td($event)">17楼</td>
              <td @click="td($event)">18楼</td>
            </tr>
          </table>
        </div>
        <div class="box">
          <table>
            <tr>
              <td @click="td($event)">11楼</td>
              <td @click="td($event)">12楼</td>
              <td @click="td($event)">13楼</td>
              <td @click="td($event)">14楼</td>
              <td @click="td($event)">15楼</td>
              <td @click="td($event)">16楼</td>
              <td @click="td($event)">17楼</td>
              <td @click="td($event)">18楼</td>
            </tr>
          </table>
        </div>
      </div>
    </div>
    <div class="cont cont2">
      <div class="left left2" @click="cont2">
        五栋-2单元-选择栋
      </div>
      <div class="right right2">
        <div class="box">
          <table>
            <tr>
              <td @click="td($event)">11楼</td>
              <td @click="td($event)">12楼</td>
              <td @click="td($event)">13楼</td>
              <td @click="td($event)">14楼</td>
              <td @click="td($event)">15楼</td>
              <td @click="td($event)">16楼</td>
              <td @click="td($event)">17楼</td>
              <td @click="td($event)">18楼</td>
            </tr>
          </table>
        </div>
        <div class="box">
          <table>
            <tr>
              <td @click="td($event)">11楼</td>
              <td @click="td($event)">12楼</td>
              <td @click="td($event)">13楼</td>
              <td @click="td($event)">14楼</td>
              <td @click="td($event)">15楼</td>
              <td @click="td($event)">16楼</td>
              <td @click="td($event)">17楼</td>
              <td @click="td($event)">18楼</td>
            </tr>
          </table>
        </div>
        <div class="box">
          <table>
            <tr>
              <td @click="td($event)">11楼</td>
              <td @click="td($event)">12楼</td>
              <td @click="td($event)">13楼</td>
              <td @click="td($event)">14楼</td>
              <td @click="td($event)">15楼</td>
              <td @click="td($event)">16楼</td>
              <td @click="td($event)">17楼</td>
              <td @click="td($event)">18楼</td>
            </tr>
          </table>
        </div>
      </div>
    </div>
    <div class="cont">
      <div class="left" @click="cont3">
        五栋-3单元-选择栋
      </div>
      <div class="right right3">
        <div class="box">
          <table>
            <tr>
              <td @click="td($event)">11楼</td>
              <td @click="td($event)">12楼</td>
              <td @click="td($event)">13楼</td>
              <td @click="td($event)">14楼</td>
              <td @click="td($event)">15楼</td>
              <td @click="td($event)">16楼</td>
              <td @click="td($event)">17楼</td>
              <td @click="td($event)">18楼</td>
            </tr>
          </table>
        </div>
        <div class="box">
          <table>
            <tr>
              <td @click="td($event)">11楼</td>
              <td @click="td($event)">12楼</td>
              <td @click="td($event)">13楼</td>
              <td @click="td($event)">14楼</td>
              <td @click="td($event)">15楼</td>
              <td @click="td($event)">16楼</td>
              <td @click="td($event)">17楼</td>
              <td @click="td($event)">18楼</td>
            </tr>
          </table>
        </div>
        <div class="box">
          <table>
            <tr>
              <td @click="td($event)">11楼</td>
              <td @click="td($event)">12楼</td>
              <td @click="td($event)">13楼</td>
              <td @click="td($event)">14楼</td>
              <td @click="td($event)">15楼</td>
              <td @click="td($event)">16楼</td>
              <td @click="td($event)">17楼</td>
              <td @click="td($event)">18楼</td>
            </tr>
          </table>
        </div>
      </div>
    </div>
    <button @click="cz">重置</button>
  </div>
</template>

<script setup lang="ts">
const cont1 = () => {
  document.querySelectorAll('.right1').forEach((item:any) => {
    console.log(item)
    item.style.backgroundColor = 'skyblue'
  })
  document.querySelectorAll('.right2,right3').forEach((item:any) => {
    console.log(item)
    item.style.backgroundColor = ''
  })
}
const cont2 = () => {
  document.querySelectorAll('.right2').forEach((item:any) => {
    console.log(item)
    item.style.backgroundColor = 'skyblue'
  })
  document.querySelectorAll('.right1,.right3').forEach((item:any) => {
    console.log(item)
    item.style.backgroundColor = ''
  })
}
const cont3 = () => {
  document.querySelectorAll('.right3').forEach((item:any) => {
    console.log(item)
    item.style.backgroundColor = 'skyblue'
  })
  document.querySelectorAll('.right1,.right2').forEach((item:any) => {
    console.log(item)
    item.style.backgroundColor = ''
  })
}
const cz = () => {
  document.querySelectorAll('.right,td').forEach((item:any) => {
    console.log(item)
    item.style.backgroundColor = ''
  })
}
const td = (e:any) => {
  console.log(e)
  e.currentTarget.style.backgroundColor = 'skyblue'
}
</script>
<style>
.cont{
  display: flex;
}
button{
  margin-top: 20px;
  margin-left: 40%;
}
.left{
  width: 300px;
  height: 135px;
  border-bottom: 1px solid rgb(171, 170, 170);
}
.right{
  width: 800px;
  height: 130px;
  /* background-color: pink; */
}
.right2{
  width: 800px;
  height: 130px;
  /* background-color: goldenrod; */
}
.right3{
  width: 800px;
  height: 130px;
  /* background-color: yellowgreen; */
}
td{
  width: 100px;
  height: 40px;
  border-bottom: 1px solid rgb(235, 234, 234);
}
</style>
