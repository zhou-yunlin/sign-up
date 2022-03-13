<template>
  <div id="hellow">
    <form action="https://www.baidu.com/s?tn=88093251_92_hao_pg&wd=python&ie=utf-8" class="login">
    <!-- action=后跟着跳转地址-->
    <p>{{ msg }}</p><!--{{  }}中存放一个文本对象，显示的文本可通过msg=""进行赋值和改动-->
    <input type="text" placeholder="用户名">
    <input type="password" placeholder="密码">
    <input type="submit" class="btn" value="登  录">
    </form>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
*{
    user-select: none;
    /* 整体无法选中，整体感更强 */
}
.login{
    position: absolute;
    top: 80%;
    margin-top: -200px;
    left: 100%;
    margin-left: -200px;
    /* absolute居中的一种方法 */
    background-color: whitesmoke;
    width: 400px;
    height: 400px;
    border-radius: 25px;
    text-align: center;
    padding: 5px 40px;
    box-sizing: border-box;
    /* 这样padding就不会影响大小 */
}

p{
    font-size: 42px;/*调整p大小*/
    font-weight: 600;/*字体粗细*/
}

input{
    background-color: rgb(252, 244, 230);/*输入框的背景色*/
    width: 100%;/*输入框宽度*/
    height: 48px;/*输入框高度*/
    margin-bottom: 10px;/*输入框间隔*/
    border: none;
    border-bottom: 2px solid rgb(149, 174, 221);/*底边框*/
    /* 下面的会覆盖上面的步伐 */
    outline: none;
    font-size: 22px;
}

.btn{
    background-color: #599ec5;/*按钮背景颜色*/
    width: 38%;
    height: 48px;
    border-radius: 8px;/*边框弧度化*/
    margin-top: 4px;/*顶部留白大小*/
    font-size: 28px;
    font-weight: 600;
    color: white;
}
.btn:hover{
    background-color: #59c2a0;/*悬停色*/
}

</style>
