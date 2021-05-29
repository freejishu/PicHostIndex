<template>
  <div id="app">
    <el-container>
      <el-header>
        <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal">
          <el-menu-item index="1"><a href="https://www.freejishu.com" target="_blank">freejishu的美丽世界</a></el-menu-item>
          <el-menu-item index="2">PicHost</el-menu-item>
          <el-menu-item index="3">情况说明</el-menu-item>
          
        </el-menu>
      </el-header>
      <el-main>
        <el-col style="padding:5vh 10vw">
          <div>
            <p>PicHost遇到了一些情况，所以暂停服务了。</p>
            <h1>发生了什么？</h1>
            <p>原先PicHost是放在eg的服务器上的（非常感谢eg能拿出闲置资源提供服务）。后来eg调整了运营计划，服务器不再续费了，咱就把数据备份出来了。也就是因为当时没仔细检查，导致压缩包数据损坏了（或者可能是没有下载完整）。</p>
            <p>经过一整晚的修复，恢复了<b>2019年6月29日</b>之前的数据，之后的<b>图片</b>和<b>所有数据库内数据</b>损坏后无法修复了。</p>
            <h1>现在的情况是怎样的？</h1>
            <p>我们已经将数据上传到了由DogeCloud赞助的对象存储内，并恢复了图片的访问。您可以凭原先复制链接直接访问图片。</p>
            <p>尽管现在还可以访问，但是我们建议将图片暂时转移到其他地方，因为我们也说不准哪天会处理这些图片。</p>
            <h1>是否存在数据泄露情况？</h1>
            <p>请您放心，原服务器释放后数据连服务商都无法找回，在没有备份的情况下，数据会消失但不会泄露。</p>
            <h1>未来PicHost将会？</h1>
            <p>考虑重建，但是目前学业比较繁忙，哪天不忙了、这个页面消失了，可能就意味着重建开始了。</p>
            <p>新一代的PicHost定位可能是开发脚手架，将从此方面入手进行维护和管理。</p>
            <h1>还有什么想说的吗？</h1>
            <p>说来惭愧，丢数据可能是free的传统艺能，这几年偶尔出个问题的毛病也一直没改掉。</p>
            <p>对于之前信赖我们、把图片存在PicHost的大家，说一声抱歉了。</p>
            <br />
            <br />
            <br />
            <p class="p_last">@freejishu</p>
            <p class="p_last" style="color:#cccccc">最后更新时间：2021/05/29</p>

          </div>
        </el-col>
      </el-main>
    </el-container>
    
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
      return {
        activeIndex: '3',
        activeIndex2: '1'
      };
    },
  methods: {
      goBack() {
        console.log('go back');
      }
    }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 10px;
}
p,h1{
   line-height: 1.8em;

}

.p_last{
  text-align: right
}
</style>
