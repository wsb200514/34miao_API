# 34miao_API
www.34miao.com网站的公共API接口

## 一、说明

1. 这是网站[三四秒](www.34miao.com)的公共API接口。
2. 接口目前没有任何限制，请大家文明使用。

## 二、接口详情

### 1、products

（1）http://34miao.com/api/product/posts/param_count

【参数说明】

param_count:返回最新products信息的条数（比如10，意思就是获取最新10条products信息）。

【返回结果】

```
[
    {
        "fields": {
            "p_date": "2016-06-12T10:00:03Z",
            "p_source_link": "http://mindstore.io/mind/11756",
            "p_source": "mind",
            "p_name": "\n Switcher ",
            "p_link": "https://github.com/X140Yu/Switcher?utm_source=mindstore.io",
            "p_desc": "一个用 Swift 编写的 OS X 应用，可以很轻松地切换 App Store 和 iTunes 的账号"
        },
        "model": "product.product",
        "pk": 21732
    },
    {
        "fields": {
            "p_date": "2016-06-12T10:00:03Z",
            "p_source_link": "http://next.36kr.com/posts/31376?ok_url=%2Fposts%3Fref%3Dabout",
            "p_source": "next",
            "p_name": "vim-github-hub",
            "p_link": "http://next.36kr.com/posts/31376/hit",
            "p_desc": "VIM 里的 Github/hub 程序"
        },
        "model": "product.product",
        "pk": 21731
    },
    ……
]
```

（2）http://34miao.com/api/product/old/param_count/param_pk

【参数说明】

param_count:返回信息的条数。

param_pk:返回从哪个pk开始之前的信息。

这是用来加载更多信息时的api，比如param_count是10，param_pk是21728，那么返回的就是pk为21718~21727的10条信息。

【返回结果】

```
[
    {
        "fields": {
            "p_date": "2016-06-12T09:56:03Z",
            "p_source_link": "http://mindstore.io/mind/11754",
            "p_source": "mind",
            "p_name": "\n Vivv ",
            "p_link": "https://itunes.apple.com/cn/app/vivv/id1060248149?mt=8&ign-mpt=uo%3D4&utm_source=mindstore.io",
            "p_desc": "相机、视频和 GIF 三合一应用，在拍摄中即可完成去色及滤镜"
        },
        "model": "product.product",
        "pk": 21727
    },
    {
        "fields": {
            "p_date": "2016-06-12T09:56:03Z",
            "p_source_link": "http://mindstore.io/mind/11751",
            "p_source": "mind",
            "p_name": "\n Formulas ",
            "p_link": "https://itunes.apple.com/cn/app/formulas-tu-pian-shi-yan-shi/id990668324?mt=8&utm_source=mindstore.io",
            "p_desc": "复古电影仿真效果的修图应用，提供自动分析图片的颜色以及色调水平一键调整功能"
        },
        "model": "product.product",
        "pk": 21726
    },
    ……
]
```

### 2、news

（1）http://34miao.com/api/news/posts/param_count

【参数说明】

param_count:返回最新news信息的条数（比如10，意思就是获取最新10条news信息）。

【返回结果】

```
[
    {
        "fields": {
            "n_desc": "由于今年端午节假期恰逢欧洲杯开赛，也让部分身为球迷的游客拼假出游，选择亲临现场感受世界顶级赛事的独特魅力，一睹球星们的飒爽英姿。",
            "n_date": "2016-06-12T10:12:02Z",
            "n_img_url": "http://img2.donews.com/2016/0612/10242928.jpg",
            "n_source": "donews",
            "n_link": "http://m.donews.com/201606/2930238.shtm",
            "n_title": "端午出行盘点：周边游仍唱主角 欧洲杯带动境外旅游热"
        },
        "model": "news.news",
        "pk": 59162
    },
    {
        "fields": {
            "n_desc": "看看他们是如何参与新三板扩容的",
            "n_date": "2016-06-12T10:08:03Z",
            "n_img_url": "http://img3.kuailiyu.com/uploadfile/2016/0612/thumb_200_120_20160612100024357.jpg",
            "n_source": "cyzone",
            "n_link": "http://www.cyzone.cn/a/20160612/297979.html",
            "n_title": "子公司纷纷挂牌，海航、腾讯、阿里、蓝标等上市公司布局新三板大盘点"
        },
        "model": "news.news",
        "pk": 59161
    },
    ……
]
```

（2）http://34miao.com/api/news/old/param_count/param_pk

【参数说明】

param_count:返回信息的条数。

param_pk:返回从哪个pk开始之前的信息。

这是用来加载更多信息时的api，比如param_count是10，param_pk是21728，那么返回的就是pk为21718~21727的10条信息。

【返回结果】

```
[
    {
        "fields": {
            "n_desc": "小米净水器把传统净水器这种很“重”的产品变得很“轻”，把不透明的产品变得透明。我们认为这代表了未来的技术方向，究竟是不是这样，请拭目以待。",
            "n_date": "2015-11-20T17:37:01Z",
            "n_img_url": "http://7te8bu.com1.z0.glb.clouddn.com/uploads/new/article/pic/201511/564e91e462e09.jpg?imageMogr2/thumbnail/!210x140r/gravity/Center/crop/210x140/quality/90",
            "n_source": "leiphone",
            "n_link": "http://www.leiphone.com/news/201511/XL0eGbZb43zKkntW.html",
            "n_title": "「唯物」陈小平：小米净水器为何做异类"
        },
        "model": "news.news",
        "pk": 21727
    },
    {
        "fields": {
            "n_desc": "500 Startups 的创始人 Dave McClure 回顾自己这大半辈子，从碌碌无为到今天的著名投资人。",
            "n_date": "2015-11-20T17:35:02Z",
            "n_img_url": "http://d.36krcnd.com/nil_class/d2530dd3-d947-4475-938a-8106bd7b11fa/dave-mcclure-by-dancingwithwords.jpg!feature",
            "n_source": "36kr",
            "n_link": "http://36kr.com/p/5039911.html",
            "n_title": "500 Startups创始人Dave McClure：虽大器晚成，但不算失败"
        },
        "model": "news.news",
        "pk": 21726
    },
    ……
]
```

### 3、design

（1）http://34miao.com/api/design/posts/param_count

【参数说明】

param_count:返回最新design信息的条数（比如10，意思就是获取最新10条design信息）。

【返回结果】

```
[
    {
        "fields": {
            "design_link": "http://www.zcool.com.cn/work/ZMTY3NDYwMzY=.html",
            "design_date": "2016-06-12T09:53:02Z",
            "design_title": "短篇动画《海洋盒子》----河南大学2016毕业设计＃青春答卷2016＃",
            "design_img_url": "http://img.zcool.cn/community/031db41575bf2df0000018c1ba60c34.jpg@250w_188h_1c_1e_2o",
            "design_source": "zcool"
        },
        "model": "design.design",
        "pk": 13059
    },
    {
        "fields": {
            "design_link": "http://www.zcool.com.cn/work/ZMTY3NDcwMTI=.html",
            "design_date": "2016-06-12T06:53:01Z",
            "design_title": "龙岩帝国",
            "design_img_url": "http://img.zcool.cn/community/031fd5b575c140e0000012e7e236956.jpg@250w_188h_1c_1e_2o",
            "design_source": "zcool"
        },
        "model": "design.design",
        "pk": 13058
    },
    ……
]
```

（2）http://34miao.com/api/design/old/param_count/param_pk

【参数说明】

param_count:返回信息的条数。

param_pk:返回从哪个pk开始之前的信息。

这是用来加载更多信息时的api，比如param_count是10，param_pk是13058，那么返回的就是pk为13048~13057的10条信息。

【返回结果】

```
[
    {
        "fields": {
            "design_link": "http://www.zcool.com.cn/work/ZMTY3NDYwMzY=.html",
            "design_date": "2016-06-12T06:53:01Z",
            "design_title": "短篇动画《海洋盒子》----河南大学2016毕业设计",
            "design_img_url": "http://img.zcool.cn/community/031db41575bf2df0000018c1ba60c34.jpg@250w_188h_1c_1e_2o",
            "design_source": "zcool"
        },
        "model": "design.design",
        "pk": 13057
    },
    {
        "fields": {
            "design_link": "http://www.zcool.com.cn/work/ZMTY3NDU3ODg=.html",
            "design_date": "2016-06-12T06:53:01Z",
            "design_title": "rent app 租房应用设计（dribbble 100days）",
            "design_img_url": "http://img.zcool.cn/community/0311397575bee3f0000012e7efa6b6e.jpg@250w_188h_1c_1e_2o",
            "design_source": "zcool"
        },
        "model": "design.design",
        "pk": 13056
    },
    ……
]
```

### 4、development

（1）http://34miao.com/api/development/posts/param_count

【参数说明】

param_count:返回最新development信息的条数（比如10，意思就是获取最新10条development信息）。

【返回结果】

```
[
    {
        "fields": {
            "dev_link": "http://www.oschina.net/code/snippet_661306_56989",
            "dev_date": "2016-06-12T10:33:03Z",
            "dev_title": "编码转换工具",
            "dev_category": "python",
            "dev_source": "OSChina"
        },
        "model": "development.development",
        "pk": 79812
    },
    {
        "fields": {
            "dev_link": "http://my.oschina.net/u/1458120/blog/688739",
            "dev_date": "2016-06-12T10:28:05Z",
            "dev_title": "redis 的bitmap 开源包 bitmapist的应用",
            "dev_category": "mySQL",
            "dev_source": "OSChina"
        },
        "model": "development.development",
        "pk": 79811
    },
    ……
]
```

（2）http://34miao.com/api/development/old/param_count/param_pk

【参数说明】

param_count:返回信息的条数。

param_pk:返回从哪个pk开始之前的信息。

这是用来加载更多信息时的api，比如param_count是10，param_pk是79808，那么返回的就是pk为78798~79807的10条信息。

【返回结果】

```
[
    {
        "fields": {
            "dev_link": "http://www.cocoachina.com/apple/20160612/16646.html",
            "dev_date": "2016-06-12T10:14:02Z",
            "dev_title": "传苹果将把iMessage引入Android平台",
            "dev_category": "iOS",
            "dev_source": "CocoaChina"
        },
        "model": "development.development",
        "pk": 79807
    },
    {
        "fields": {
            "dev_link": "http://www.cocoachina.com/apple/20160612/16645.html",
            "dev_date": "2016-06-12T10:14:02Z",
            "dev_title": "苹果开始装修WWDC2016会场外的LOGO",
            "dev_category": "iOS",
            "dev_source": "CocoaChina"
        },
        "model": "development.development",
        "pk": 79806
    },
    ……
]
```

（3）development下面各个子分类其实和主分类类似，此处说明省略，只列出api接口。

1. 头条最新信息获取：http://34miao.com/api/development/top/posts/param_count
2. 头条加载更多获取：http://34miao.com/api/development/top/old/param_count/param_pk
3. 前端最新信息获取：http://34miao.com/api/development/front/posts/param_count
4. 前端加载更多获取：http://34miao.com/api/development/front/old/param_count/param_pk
5. 后端python最新信息获取：http://34miao.com/api/development/python/posts/param_count
6. 后端python加载更多获取：http://34miao.com/api/development/python/old/param_count/param_pk
7. 移动iOS最新信息获取：http://34miao.com/api/development/iOS/posts/param_count
8. 移动iOS加载更多获取：http://34miao.com/api/development/iOS/old/param_count/param_pk
9. 数据库MySQL最新信息获取：http://34miao.com/api/development/mySQL/posts/param_count
10. 数据库MySQL加载更多获取：http://34miao.com/api/development/mySQL/old/param_count/param_pk
11. 运维最新信息获取：http://34miao.com/api/development/operation/posts/param_count
12. 运维加载更多获取：http://34miao.com/api/development/operation/old/param_count/param_pk

### 5、marketing

（1）http://34miao.com/api/marketing/posts/param_count

【参数说明】

param_count:返回最新marketing信息的条数（比如10，意思就是获取最新10条marketing信息）。

【返回结果】

```
[
    {
        "fields": {
            "m_img_url": "http://image.meihua.info:808/upload/2016/06/08/146538107710458.jpg",
            "m_title": "毕业季，除了煽情文案和海报，品牌商还能怎么玩？",
            "m_link": "http://www.meihua.info/a/66954",
            "m_date": "2016-06-12T10:33:02Z",
            "m_desc": "毕业季，每年一次的大热点又来了！品牌商们，你们还坐得住吗？今天梅小花就给大家罗列在毕业季上品牌商追热点惯用姿势！大家赶紧码住，这些营销方法你或许用得上！",
            "m_source": "meihua"
        },
        "model": "marketing.marketing",
        "pk": 16779
    },
    {
        "fields": {
            "m_img_url": "http://image.meihua.info:808/upload/2016/06/12/146569743278459.jpg",
            "m_title": "为什么初创公司总是会在“公关”这件事上搞砸？究竟该怎么做",
            "m_link": "http://www.meihua.info/a/66955",
            "m_date": "2016-06-12T10:33:02Z",
            "m_desc": "初创公司想要在互联网上建立起自己的品牌，拓展影响力，培育出具有高忠诚度的线上社群，究竟该怎么做？如何获得媒体和网民的关注？本文给出了一些具有极强操作性的策略……",
            "m_source": "meihua"
        },
        "model": "marketing.marketing",
        "pk": 16778
    },
    ……
]
```

（2）http://34miao.com/api/marketing/old/param_count/param_pk

【参数说明】

param_count:返回信息的条数。

param_pk:返回从哪个pk开始之前的信息。

这是用来加载更多信息时的api，比如param_count是10，param_pk是13058，那么返回的就是pk为13048~13057的10条信息。

【返回结果】

```
[
    {
        "fields": {
            "m_img_url": "http://image.meihua.info:808/upload/2016/04/06/145992605476798.jpg",
            "m_title": "这些品牌的广告因为欺骗消费者被罚了数百万美元",
            "m_link": "http://www.meihua.info/a/66437",
            "m_date": "2016-04-06T16:33:02Z",
            "m_desc": "虽然广告多少都有点夸张，但夸张到什么程度是能被接受的？这个界限虽然很难界定，不过有些很明显是在欺骗消费者。此篇黑榜的10个案例，向大家展示一些大公司的虚假广告，它们不仅面临百万赔款还遭遇了品牌危机。",
            "m_source": "meihua"
        },
        "model": "marketing.marketing",
        "pk": 13057
    },
    {
        "fields": {
            "m_img_url": "http://image.meihua.info:808/upload/2016/04/06/145992873907399.jpg",
            "m_title": "定位，你不要再作死了",
            "m_link": "http://www.meihua.info/a/66438",
            "m_date": "2016-04-06T16:33:02Z",
            "m_desc": "无论是竞争环境，媒体环境，消费者的消费模式，心智认知模式都正在发生巨变。任何一个体系凡是自洽的，必是不完全的，“定位”理论也遇见了自己的“黑洞”，其再不与时俱进，真的只能作死了。",
            "m_source": "meihua"
        },
        "model": "marketing.marketing",
        "pk": 13056
    },
    ……
]
```

## 三、iOS版本提交经验参考

1. 需要添加一个可供用户举报内容的功能，否则很难通过。
2. 填写应用信息时注意不要添加任何有关android的信息，仔细检查截图，截图中也不要出现android或安卓字样。
3. 在补充说明里最好解释一下该应用的价值，因为聚合阅读应用实在太多，苹果自己也有news，所以对于这类应用，要么设计和体验很好，不然最好是解释一下该应用的价值（我当时就说我是一个开发者，每天需要在很多网站上阅读信息，十分不方便，所以弄了一个这个，不仅聚合信息，而且还分类了，十分方便，吧啦吧啦……）。
4. 在补充说明里，解释一下该应用与app store的区别。因为这里有product频道，他们认为product和app store很类似，所以会拒绝（我当时就说，app store是一个iOS应用分发平台，而本应用是产品聚合平台，这个产品不仅仅包含iOS的，安卓的，web的，甚至是什么都没有只有一个idea的，所以产品聚合和app store没有任何竞争关系，吧啦吧啦……）。
6. 提交前，最好与我联系，我会在你应用审核的这段时间暂时屏蔽掉一些安卓的文章。因为审核人员打开app的时候浏览信息如果浏览到安卓的文章，也会呵呵的。

## 四、其他

1. 我自己开发的iOS应用不久会下架。
2. 如果你的应用上架后，有需要放在[三四秒](www.34miao.com)网站上的，请与我联系，我会放上去。
3. 有任何需求，可与我联系，邮箱weisubao1987@gmail.com。
