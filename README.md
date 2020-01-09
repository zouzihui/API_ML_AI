# API_ML_AI
 |  发布日期 | 2019-12-05 |
 | -- | -- |
 |  项目名称 | 动物园游玩助手 |
 |  项目现状 | 进行中 |
 |  项目的主人 | 邹子惠 |
 |  项目的设计师 | 邹子惠 |
 |  项目的开发者 | 邹子惠 |
 |  项目头的测试者 | 邹子惠 |
 
- 20×20ppt
[文件下载链接](https://github.com/zouzihui/API_ML_AI) 

## 价值主张设计 
- 一句话版本

让动物园游览变得不拥挤，有头绪。

- 一分钟版本

本产品以动物园游客为目标用户，目的是为了解决动物园游客无法舒心观看动物信息以及对游玩路线不清楚的问题。经过市场调查我们发现市面上的动物识别类app功能都十分单一仅仅能进行识别，动物园app又只集中在路线规划功能，而动物园游玩助手app则是一个以动物识别和路线规划为主要功能的app，能给动物园游客提供一个更便捷舒适的游玩体验。第一个主要功能动物识别，运用了百度AI的动物识别api，用户通过拍摄一张动物园动物的照片，上传后立刻返回该动物名称及更多百科知识，轻松解决了人流量大时动物介绍栏阅读难问题。第二个主要功能时路线规划，运用了高德地图api的路径规划api，用户输入起点终点，自动帮助规划最佳到达路线，解决了游客看不懂地图和动物园路标指引少的问题。



## 一、背景
动物园总是我们进行亲子时光或是增长知识的场所之一 ，大部分动物园特点是介绍信息在对应园区的信息栏中，现在流行的放养式动物园区对动物的详细介绍更是少之又少。在我们去动物园游玩时总是会遇到一个无法避免的问题。无论工作日或节假日园区内人流量都有不少，这时人们大多聚集到较小的动物介绍栏进行信息解读，而无法走到前面的游客则无法阅读动物相关信息，有时更是因为距离问题影响了动物观赏。这时，一个能给游客进行解说和领导的动物园游玩助手app似乎就能帮上许多忙，只需一步轻松得到动物相关信息及其在园区位置，再根据用户所拍的动物给用户制定动物园游玩线路。

## 二、加值宣言
经过调查,我们可以发现市面上已经有相类似的动物/昆虫识别app，上传照片进行识别得到对应动物信息例如“自然观察”app。但同时我们也发现此类app大多功能单一，只能简单的对动物进行识别。此外，我们还发现许多动物园也开发了其app，但此类app中均无动物识别功能。若基于动物园app上，运用动物识别api和路径规划api，app整体则显得更加实用，联系整个动物园园区，与其他功能进行结合，得到更强大的效用。

优先级：运用百度AI中动物识别api,拍下园区内任意动物照片并输入，输出照片动物对应名称、种类以及百度百科详细信息。

次优先级：运用高德地图的路径规划api，在输入不同动物馆名称（如：熊猫馆）后显示为用户制定到达线路。

## 三、核心价值（最小可行性产品）
着眼与动物园游客游玩的基本需求，解决园区拥挤时用户及时获得动物介绍信息的问题。

## 四、目标
1. 拍下或上传动物照片，返回该动物种类、名称及跳转相关百科信息。
2. 输入动物馆名，返回步行路径规划，带领游客找到场馆。

## 五、目标用户
* 动物园无法清楚得到动物信息的游客
* 动物园想要了解更多知识的儿童群体游客
* 看不懂动物园地图，对场馆位置不清晰的游客

## 六、核心价值与用户痛点

| 加值	| 痛点	|
| -- | -- |
| 动物识别功能可以通过拍摄动物照片得到动物名称、品种 	| 动物园人流量太多了，没有办法看到动物介绍栏 	|
| 动物识别功能可以通过拍摄动物照片得到动物详细信息	| 孩子第一次见这个动物，想给他普及多点动物知识	|
| 路线规划功能可以对你从当前位置到动物园任一游览馆进行路线导航| 在动物园某一处，此时不清楚自己所在位置，也不知道想去场馆该怎么走 |

## 七、需求列表与人工智能API加值
| 用户案例	| 对应api	| 重要程度 |
| -- | -- | -- |
| 用户想知道当前观赏动物的名字 	| 动物识别 	| 非常重要 |
| 用户想知道当前观赏动物的更多详细信息	| 动物识别	| 非常重要 |
| 用户想知道当前位置到想去场馆的路线| 路径规划 | 次重要 |

**具体应用场景**
1. 小王来动物园游玩，此时他见到一个新奇的动物，想要知道他的名字，但这时他没有找到动物介绍栏，于是他打开动物园游玩助手app，拍下此动物照片进行动物识别，自动识别出了该动物的名字和品种。
2. 周末妈妈带着儿子小明来来动物园游玩，但动物园人太多了，人们都里三层外三层地围在了动物介绍栏旁。这时妈妈拿出手机打开了动物园游玩助手app，让小明拍下动物照片，立即得到了该动物的百度百科介绍。
3. 小李在路上走着，准备去找“飞鸟馆”，但不识路也不太会看地图的她不知怎么去。这时小李打开app，输入了“飞鸟馆”，立刻返回了当前位置到飞鸟馆的路线导航。

## 八、人工智能概率性与用户痛点
* 百度AI中的**动物识别api**:
1. 识别近八千种动物，接口返回动物名称，支持自定义返回结果数
2. 支持获取识别结果的百科信息，接口返回百科词条URL、图片和描述，支持自定义返回词条数

综上可得出，用户在使用动物识别时可识别动物种类多，基本能满足整个动物园游览识别动物的使用，识别动物基本能返回百科词条信息。但在拍摄和上传图片极为模糊时或网络断连和卡顿的情况下，会影响该功能的使用，但正常情况的手机拍摄和网络下不会影响使用，对用户基本影响不大。

* 高德地图api中的**路径规划api**
1. 基于全面的路网信息
2. 结合精准的实时路况
3. 有着全面的导航方式

综上可得出，用户通过输入起始地便能得到精准导航路线。此功能基于全面的路网信息和实时路况更新而精准率高。但可能会因非功能原因（用户没有及时更新app使路面信息没更新，导致导航错误）或位置太偏路网信息未更新而影响使用。但此类事件均为小概率事件，不影响绝大部分用户使用。

## 原型
## 一、交互及界面设计
1. “权限”页面

![位置授权](https://images.gitee.com/uploads/images/2019/1209/221810_ef123f93_1648195.png "授权1.png")

![拍照授权](https://images.gitee.com/uploads/images/2019/1209/221829_cdd1a8c5_1648195.png "授权2.png")

![拍照](https://images.gitee.com/uploads/images/2019/1209/221952_3b031fb0_1648195.png "拍照.png")

![图识别](https://images.gitee.com/uploads/images/2019/1208/225342_0e38691e_1648195.png "59855be1a65398e169a8757cce0512c.png")

![图库](https://images.gitee.com/uploads/images/2019/1209/222011_a280e483_1648195.png "图库.png")

![识别](https://images.gitee.com/uploads/images/2019/1209/222023_cf368ef0_1648195.png "识别.png")

![百度](https://images.gitee.com/uploads/images/2019/1209/223001_b05c2c4c_1648195.png "百度.png")

3. “路线规划”页面

![路线](https://images.gitee.com/uploads/images/2019/1209/222125_89028a7d_1648195.png "路线.png")

4. “我的”页面

![我的](https://images.gitee.com/uploads/images/2019/1209/222656_bfa72bcf_1648195.png "我的.png")

## 二、信息设计
### 产品信息架构
![信息结构图](https://images.gitee.com/uploads/images/2019/1206/204114_ad2cced8_1648195.png "”动物园游玩助手“产品信息结构图.png")
### 产品功能结构图
![功能结构图](https://images.gitee.com/uploads/images/2019/1206/204128_dfbbbe7a_1648195.png "”动物园游玩助手“功能结构图.png")
### 产品结构图
![产品结构图](https://images.gitee.com/uploads/images/2019/1206/204055_c493a916_1648195.png "”动物园游玩助手“产品结构图.png")
### 产品流程图
![流程图](https://images.gitee.com/uploads/images/2019/1206/204030_1ca06733_1648195.png "“动物园游玩助手”流程图.png")


## 三、原型文档
1. 页面链接:
[产品页面](http://nfunm110.gitee.io/api_end_of_term/#g=1&p=%E8%B7%AF%E7%BA%BF%E8%A7%84%E5%88%92)

2. 产品axure文档:
[原型文档](https://github.com/zouzihui/API_ML_AI)

## 四、口头操作说明
大家好，我是本产品的负责人，今天我来为大家讲解我们推出的“动物园游玩助手”app。本产品主要有两个动能，第一是动物识别功能，此功能运用了百度AI中的动物识别api，用户可以在app内通过拍照或使用手机内照片，选中照片后点击确认即可进行动物识别，功能会通过用户输入照片进行识别，返回照片中动物的名称，种类以及百度百科信息，从而提升用户在动物园的观赏体验。第二是路线规划功能，此功能运用了高德地图api中的路劲规划api，用户点击tab栏中的路径规划图标跳转到路径规划页面，输入起始地与目的地后按搜索键即可进行路径规划，功能会通过输入起点与终点自动为用户规划最佳路线，并以地图形式显示。


## 产品使用关键AI或机器学习之API的输出入展示
### 一、 使用水平
1. 功能一：动物识别（百度AI）
* 图像技术：动物识别api
* 接口描述：该请求用于识别一张图片，即对于输入的一张图片（可正常解码，且长宽比较合适），输出动物识别结果。
* 接口地址：[百度AI的动物识别api](http://https://ai.baidu.com/ai-doc/IMAGERECOGNITION/Zk3bcxdfr)
* 请求方法：POST
* 输入代码：

![输入代码](https://images.gitee.com/uploads/images/2019/1209/145934_6c867ccf_1648195.png "22b393bdb0b0bfea5a080b6d18e8753.png")

*输出代码：

![输出代码](https://images.gitee.com/uploads/images/2019/1209/150207_2d4ad03b_1648195.png "c30182a59770668235428ae1bcd68a7.png")
![输出代码](https://images.gitee.com/uploads/images/2019/1209/150218_183f1b95_1648195.png "0f445e51d1ad9e078a88b4b7e9fcdb9.png")

2. 功能二：路线规划（高德地图api）
* web服务：路径规划api
* 接口描述：步行路径规划 API 可以规划100KM以内的步行通勤方案，并且返回通勤方案的数据。
* 接口地址： [高德地图api的路径规划api](https://lbs.amap.com/api/webservice/guide/api/direction/)
* 请求方法： POST
* 输入代码：

![输入](https://images.gitee.com/uploads/images/2019/1209/151505_36e5f151_1648195.png "输入.png")

* 输出代码

![输出1](https://images.gitee.com/uploads/images/2019/1209/151513_18e3a8a3_1648195.png "1.png")
![输出2](https://images.gitee.com/uploads/images/2019/1209/151522_b055225c_1648195.png "2.png")
![输出3](https://images.gitee.com/uploads/images/2019/1209/151531_f542bc19_1648195.png "3.png")
![输出4](https://images.gitee.com/uploads/images/2019/1209/151540_a4de97aa_1648195.png "4.png")

### 二、 使用比较分析
#### 动物识别api
1. 腾讯AI中的图片识别
* 单一主体识别

![腾讯AI](https://images.gitee.com/uploads/images/2019/1209/154918_2728662c_1648195.png "腾讯AI.png")

* 多主体识别

![腾讯2](https://images.gitee.com/uploads/images/2019/1209/155233_e3397d3b_1648195.png "腾讯AI2.png")

2. 阿里云的图像识别
* 单一主体识别

![阿里云](https://images.gitee.com/uploads/images/2019/1209/154935_80f3ef1a_1648195.png "阿里云.png")

* 多主体识别

![百度2](https://images.gitee.com/uploads/images/2019/1209/155252_dcb9fd9e_1648195.png "百度AI2.png")

3. 百度AI的动物识别
* 单一主体识别

![百度AI](https://images.gitee.com/uploads/images/2019/1209/154951_0392f82b_1648195.png "百度AI.png")

* 多主体识别

![阿里2](https://images.gitee.com/uploads/images/2019/1209/155302_6725836a_1648195.png "阿里云2.png")

**百度AI与腾讯AI、阿里云的使用比较**

(1) 三个AI开放平台只有百度AI有针对动物图像的动物识别，且单一主体与多主体图像均能识别，输出结果在三款图像识别api中也是最精准的。此外，也只有百度AI在识别玩图像后还会返回对应百科信息链接。

(2) 腾讯AI的图像识别api中，只有多标签识别能识别出动物，但输出结果并不准确。

(3) 阿里云的图像识别api中，可以进行单一和多主体动物图像识别，但只返回动物名称，比较适用于图像打标。


## 使用后风险报告
### 一、 API市场竞争程度

### 二、 输入输出限制

**动物识别api**

(1) 请求图片需经过base64编码：图片的base64编码指将一副图片数据编码成一串字符串，使用该字符串代替图像地址。您可以首先得到图片的二进制，然后用Base64格式编码即可。
注意：图片的base64编码是不包含图片头的，如（data:image/jpg;base64,）

(2) 请求格式支持：PNG、JPG、JPEG、BMP、GIF**

(3) base64编码后大小不超过4M，最短边至少15px，最长边最大4096px，长宽比3：1以内

**路径规划api**

(1)服务调用量限制 

![路限制1](https://images.gitee.com/uploads/images/2019/1209/163918_d2917a87_1648195.png "路径规划限制1.png")
![限制2](https://images.gitee.com/uploads/images/2019/1209/163931_5e0c6d8d_1648195.png "路径规划限制2.png")
![限制3](https://images.gitee.com/uploads/images/2019/1209/163940_e0653ca7_1648195.png "路径规划限制3.png")

### 三、 API定价
**动物识别api**

![百度定价](https://images.gitee.com/uploads/images/2019/1209/164607_8d82738b_1648195.png "百度收费.png")

**路径规划api**

高德地图api调用均不收费，不同类型开发者有每日调用次数限制，详情见（二、输入输出限制）


### 四、 产品可行性

(1) 该产品是动物识别+路线规划的动物园游玩助手app，现行并没有两功能共存的动物园app出现，市场竞争力较小。

(2) 该产品目标用户明确，提供给动物园游玩群体、儿童以及动物园需导航路线者使用。

(3) 该产品很好的解决了动物园参观人流量大导致汲取信息难和动物园园区迷路者的问题，提升了动物园游客的游玩体验。

### 五、 结果预期

上线初期，先推出试用版供动物园游客体验使用，试用结束后根据游客反馈和使用期间出现的问题对产品进行合理化修改和提升，最终面向市场广泛使用。由于是基于动物园推出的app，所以积累用户相对压力小。到app运行稳定阶段，可通过与广告商合作、销售商合作，推出商城等其他功能，吸引新用户，留住旧用户。
