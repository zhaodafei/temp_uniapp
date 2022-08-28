# temp_uniapp
uni-app项目,一套代码集合了h5,微信小程序,Android版,iOS版等跨平台效果,支持Vue2

### 环境说明

```html
vue-cli 版本 @vue/cli 4.5.15
vue 2.6.11
node 14.18.0
开发工具 webstorm
测试工具: chrome, 微信开发者工具

-- 2022年8月29日 , ***温馨提示***
vant 这个ui目前支持在Vue2这个版本中使用在微信中,不支持Vue3引入微信中,在分uniapp_vue3中各种奇怪的问题
```



### 启动

```bash
#这个项目使用了 vant/weapp 所以不支持浏览器访问 
#npm run dev:h5  #h5启动,浏览器中启动
npm run dev:mp-weixin  #启动后,微信小程序中访问
```

### vant 测试

```html
测试 vant/weapp 是否引入成功
<van-button type="primary">主要按钮</van-button>
<van-switch active-color="#07c160" inactive-color="#ee0a24" />
```



