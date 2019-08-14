<template>
    
</template>

<script>
    export default {
        name: "封装上传组件"
        //上传图片和文件
        /*
        * 表单用自定义表单 label标签                                         监听success success执行方法
        * input 加 file 前端唯一获得文件的方法  <input type='file' class='hs-upload' @chanage='change'>
        * 封装组件不要用scope 别人无法覆盖你的样式
        * 清除默认样式 display:none;
        * 上传按钮 div 设置样式就可以上传文件
        * 按钮可以用slot 替代 为了组件复用用slot
        *
        * data(){
        * return{
        *   token:
        * }
        * }
        * 定义方法 (第一步拿到token) methods:{
        *   getToken(){
        *     axios.get('url/getoken').then(res=>{
        *        this.token = res.data.data
        *     })
        *   },
        *   // 获取事件对象
        *   change(event){
        *     const file = $event.target.files[0] //拿到这个文件
        *     const form = new FormData()
        *     form.append('file', file)
        *     form.append('token', this.token)
        *
        *     //开始上传  之前要创建一个表单 form
        *     axios.post('七牛上传地址 华北区客户端上传'，form(放内容)).then(res=>{
        *       console.log(res)
        *       //子向父传值 把data中url 中具体上传的文件
        *       this.$emit('success', res.data.url) //抛出去
        *     })
        *   }
        * }
        * //获取token 先有token 才能传
        * created（）{
        *   this.getToken()
        * }
        *
        *
        * 要用的view 页面中
        * 引入组件
        * 声明组件
        * 组件标签 中来一个上传按钮 label中不能放置另一个表单元素button 浏览器不知道解析哪一个
        *
        *
        * 配置路由
        * router引入路由才能用组件
        *
        * changeUer 接口怎么用
        * changeAvatar(url){                     把值带过去 字段avatar + url
        *   this.$axios.put(this.$api.chagneUser, {avatar:url}).then(res=>{
        *     if(res.code == 200){
        *       Toast({
        *         message:'头像修改成功'
        *       })
        *       //更新数据 改了要跟新页面
        *       this.$store.dispatch('getUserData')   ('store 当中的action 定义的名字')
        *     }
        *   })
        * }
        *
        * */


    }
</script>

<style scoped>

</style>