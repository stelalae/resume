# 雷银春 - 个人简历

## 个人信息

* 手机：18980914937（微信同号）
* Email：a@wyolo.com
* 年龄：31
* 住址：成都市龙泉驿区大面镇
* 工作年限：8年
* 教育背景：成都信息工程大学 - 通信专业（2008.09-2012.06），大学本科
* Github：https://github.com/stelalae （[个人博客](https://github.com/stelalae/blog)，开源项目：[WebCacheFile](https://github.com/stelalae/WebCacheFile)）
* 期望职位：前端开发负责人，ReactNative高级开发，iOS高级开发，应用架构师
* 期望城市：成都

## 工作经历

### 四川三松医疗管理集团有限公司 （2019.05~至今） — 前端负责人

![](https://cdn.jsdelivr.net/gh/stelalae/oss@master/files/2020/05/28/3RtO65.jpg)

集团新成立互联网事业部，带领三人小组开发互联网医院产品的前端，包含医生App端、用户微信端和App端、运营后台。我主要负责前段项目搭建、技术选型及指导、iOS独立开发，参与产品讨论。IM和音视频基于融云的二次开发。

1. 产品一期（2019.06~2019.09）包含在线问诊、云药房及电子处方等模块。在线问诊衍生出快速问诊、专家问诊、推荐医生等差异化业务，实现签到、三级分销、积分抵扣等营销功能。技术上选择umijs作为用户微信端、运营后台的项目基础框架，医生App端采用Tabbar+IM为原生、RN编写业务插件化方式。带领团队解决人手不够、业务不清晰、需求反复修改等问题。
2. 产品二期（2019.12~2020.01）新增远程门诊业务，患者从用户端预约及支付，实现iOS/Android App、Android TV等两两音视频互通。
3. 产品三期（2020.03~2020.04）是将用户微信端已有功能，一个月内内快速迁移到新App上，复用了部分微信端的页面。利用umijs多渠道功能，结合预加载和本地缓存功能，解决iOS并协助Android上WebView加载速度慢和低端机型的页面兼容问题，研究了WKWebView和NSURL，整理出iOS开源库WebCacheFile。

### 成都华西公用医疗信息服务有限公司 （2017.9~2019.04） — 前端负责人

![](https://cdn.jsdelivr.net/gh/stelalae/oss@master/files/2020/05/28/Uo5oKQ.jpg)

工作内容：
1. 由iOS开发者身份应聘到公司后，因微信端业务发展需要，研究React全家桶，从0开始组建一个5人的Web小组，同时推动ReactNative在App上的应用，为公司业务快速扩展提供技术基础，后面逐渐负责公司的APP/公众号/管理端等所有前端相关工作。
2. 参与华医通产品每个版本和新项目的需求评审、技术方案、前端任务安排及开发协调。技术上负责React内部框架的开发和维护更新。在组内协调对技术难点整理、业务培训、接口审核、风险和质量控制，跟踪代码中的架构落地和编码质量，同时输出文档。

工作业绩：
1. 推动华医通医生APP使用ReactNative重构，RN的功能占比高达85%，设计出能随时上线新业务的架构能力。开发周期相比原生开发缩短2/3，紧急版本次数从2017年的8次降到2018年的1次，闪退率也大幅降低，极大的提升了医生的使用体验和品牌接受度。
2. 推动华医通大众APP里轻量交互的模块改为React开发，同时能在公众号、生活号等复用，在保证质量的前提下缩短了开发周期、更快速响应院方需求，重构以前jsp前端模块后，提升了广大患者的就医体验。
3. 将以前独立5个的管理后台使用ant design库重构融合为华医通综合管理平台，引入权限控制，更加方便运营、运维和客服的使用，杜绝手动修改数据库，整体提高华医通相关工作人员的岗位价值。
4. 积极推动华医通品牌产品的业务规范，提升IM、表单为基础系统服务，构建业务前置系统Aux，资源存储、域名的使用规范标准。输出PPT、Markdown等文档培训相关人员。
5. 因组建Web小组，提高APP组开发质量，对前端人才进行培养，给产品开发带来新理念，荣获公司『2018年最佳技术奖』！

#### 华医通APP及公众号，2017.09~2019.04    前端负责人

本项目属于SaaS项目，支持多医院上架，也是华西医院的官方项目，包含患者端（App、微信公众号、支付宝生活号等渠道）和医生端（App、PC），内容覆盖就医事务、在线问诊、医药云等。其中我负责在线问诊、医药云的所有前端开发，带领前端团队实现架构落地和业务迭代更新，后期研究项目引入TypeScript支持。

1. 在线问诊：业务上分为在线咨询、在线门诊，病人搜索开通在线服务的医生，提供病例资料并购买服务（基于腾讯云通信和实时音视频，支持文字/图片/语音/视频），医生的所有业务均是基于IM基础服务开展。
	- 患者端上App原生IM、公众号Web IM，React全家桶构建两端复用的业务页面，负责项目框架搭建和封装接口请求，引入dva解决使用redux繁琐问题，配置webpack插件解决打包慢和大的问题，协助处理业务上逻辑与交互的难点。
	- 医生端APP除IM对话使用原生外，其他均使用RN开发，包括Tabbar和IM列表、负责解决医生端RN重构过程中遇到如启动白屏、IM列表性能、与原生通信和跳转设计、iOS与Android上兼容性、第三方库筛选和引入、URL路由模式设计等技术问题，推动IM提升为基础服务，后期业务迭代增加入院证、检查检验医嘱。
2. 医药云一期包含线上电子处方，支持第三方CA签名，关联线上问诊记录、开诊断、选药开药、HIS审方、CA备案、患者支付、药师的审方/备注/发货等。负责技术方案选型和业务预演，熟悉了药品和处方的医疗流程。
3. 就医事务是在原挂号缴费的基础上，新增电子报告、电子票据、住院日清单、康护计划等，负责需求评审和协调任务安排。

#### 互联网医院，2018.12~2019.05    前端负责人

迎合互联网医院的建设要求，由华医通平台升级为华西互联网医院五大业务平台：就医事务、在线问诊、患者管理、家庭医生、医药云。根据华医通现有业务，配合基础数据重构，将华医通的大部分功能业务搬迁至互联网医院平台，完成华西互联网医院的验收，另协调前端和佰医汇科技联合开发上绕互联网医院。负责梳理前端的开发内容和开发任务，升级前端架构。

### 深圳市玩赚地球信息有限公司 （2016.10~2017.08，创业公司） — iOS开发负责人

#### YesYOLO夢想實踐者，2017.04~2017.07    项目职位：Web/Node开发

极致旅游分享网站YesYOLO，结合冒险王宥胜Facebook专页，成功打造用新台币6万5游玩南美20天的项目，在台湾引起一股极旅热潮，网站上还提供其他台湾本地极旅体验项目。上线3个月累积有14.3万个人访问UV、20.8万次会话数UPV、60.5万次页面访问量PV。

1. 学习Reactjs、Sass并完成前端页面，用ant design框架完成管理后台。
2. 使用Node+MySQL提供前端需要的数据接口，Node脚本处理每次活动需要发送的Email、统计报名等。

#### YesYOLO App，2016.10~2017.03    职位：iOS项目负责人

专注达人旅游定制线路和旅游分享的APP平台。用户在平台上选择感兴趣的线路和目的地，达人协助定制独一无二的旅游体验。

1. 接手之前多人兼职的代码，封装控件和中间件完成剩余功能，修改bug。
2. 处理不同坐标系的兼容转换和港澳地区定位偏差，使用MapKit完成打点、定位、显示图片等功能。
3. 解决大量图片显示占用内存过高的问题，完成行程发布草稿功能，和常用数据本地缓存管理。

### 索贝数码科技有限公司（2015.05~2016.09） — C++/iOS开发工程师

工作内容：负责存储文件系统SDK编写、新闻类iOS APP的模块开发。

### 成都荣耀科技有限公司 （2013.05~2015.04） — C++开发工程师

工作内容：负责安防设备的音视频接入。

### 成都安之巅信息技术有限公司（2011.10~2013.03，实习） — Windows开发工程师

工作内容：负责Windows远端控制项目的插件编写。

## 技能清单

1. 熟练ES6+/TypeScript/ReactNative/React技术栈，了解Nest.js、Egg等Node框架；
2. 熟练ReactNative/React的各种常用库和脚手架，如react-redux、react-navigator、dva/umi、ant design(pc/mobile/rn)、code-push等，对原理有一定了解。
3. 熟练Objective-C开发及相关工具使用，熟练iOS常用技术和库，对底层和源码有一定了解；
4. 熟悉中大型前端项目开发规范和流程，对移动跨平台和混合APP有一定研究，能制定前端产品架构、输出文档，并跟踪架构落地和推动产品积极优化迭代，喜欢探索解决方案和新技术，如大前端、BFF、DevOps；
5. 有大型项目和同时开发多项目的领导经验，掌握项目管理基本知识，有较强的协调能力、解决问题和抗压能力。

## 自我评价

从下面纬度自我剖析：
**开发人员**：有实际的能力和经验解决并完成iOS、RN的独立开发，能处理简单Web页面开发和熟练使用ant design框架完成管理后台，了解大前端开发需要Node/Android知识。
**前端负责人**：有多个大前端的上线项目经验，有丰富的技术架构设计能力，能主动协调项目进度，积极参与产品设计和规划，能带领团队利用现有优势完成开发，并保证质量和用户体验。
**产品与运营**：有较深的医疗行业行业，特别是问诊、药品处方等方面，一直关注最新的医疗政策。对竞品的运营和技术有自己的分析理解，熟悉互联网产品的运作方式。

---
期待您的联系，愿与您共创辉煌！




