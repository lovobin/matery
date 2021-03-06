###   matery



###  同步刷新插件

```bash
# (缺点:依赖网络环境)修改文章后，当你按下Ctrl+S保存时，页面自动刷新产生改变，同时右上角显示 Connected to BrowserSync 字样
npm install hexo-browsersync --save
```

###  搜索插件

```bash
npm install hexo-generator-search --save
# 在 hexo 根目录的  _config.yml 添加如下信息
search:
  path: search.xml
  field: post
```

###   代码高亮插件

```bash
npm i -S hexo-prism-plugin

prism_plugin:
  mode: 'preprocess'    # realtime/preprocess
  theme: 'default'
  line_number: false    # default false
  custom_css: 'path/to/your/custom.css'     # optional

highlight:
  enable: 
  
theme[可选参数]:
    default
    coy
    dark
    funky
    okaidia
    solarizedlight
    tomorrow
    twilight
    atom-dark
    base16-ateliersulphurpool.light
    cb
    duotone-dark
    duotone-earth
    duotone-forest
    duotone-light
    duotone-sea
    duotone-space
    ghcolors
    hopscotch
    pojoaque
    vs
    xonokai
```

 ###  文章是否添加到轮播图

```bash
Front-matter 选项详解
cover: # 默认false
img: # 开启特色图 轮播图显示和卡片显示图
```

### 图片预加载插件
```bash
有一些BUG可能出现:
    + 第一次使用该主题时插件效果正确体现
    + 第二次安装插件 全部显示 loading(网上的一些我暂时可查到的方法使我未生效)
```

```bash
# 图片预加载插件
npm install hexo-lazyload-image --save
# 在博客根目录配置 _config.yml文件加入对应字段
lazyload:
  enable: true 
  #如果为真，则只有文章或页面中的图像支持延迟加载。
  #如果为假，整个网站的图像将使用惰性加载，包括来自主题的图像，但不包括来自CSS样式的背景图像。
  onlypost: true
  loadingImg: /loading.gif
```



###  文章短链接显示插件

```bash
npm install hexo-abbrlink --save  
# 显示效果 显示改动: 121217726.html
http://域名/hexoblog/hexoblog/2020/121217726.html
```

