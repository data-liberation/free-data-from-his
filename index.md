title: data liberation for healthcare
speaker: wanghaisheng
plugins:
    - echarts

<slide class="bg-black-blue aligncenter" image="https://source.unsplash.com/C1HhAQrbykQ/ .dark">

# data liberation for healthcare {.text-landing.text-shadow}
如何基于已有系统搭建数据中台 {.text-intro.animated.fadeInUp.delay-500}

By wanghaisheng {.text-intro}

[:fa-github: Github](https://github.com/data-liberation/free-data-from-his){.button.ghost}


<slide class="bg-apple aligncenter">

# **第一部分：医疗信息化现状** {.text-landing.text-shadow}
:::note
## Note here
:::
<slide  class="bg-apple aligncenter ">
### **假如你在某三甲医院看病** {.text-landing.text-shadow}

!![](public/clinicalpractice2.png .aligncenter)



<slide class="bg-apple aligncenter ">


### **医疗数据生产的源头**


:::flexblock {.specs}
::fa-wifi::

## 以HIS为核心的传统系统


His、Lis、PACS等.

---

::fa-battery-full::

## 以临床为核心的临床业务系统


面向医生、护士、药师等

---

::fa-life-ring::

## 其他
面向管理人员的、其他业务创新的系统、office套件、以及没有电子化的停留在纸张中的
:::

---



<slide  class="bg-apple aligncenter ">

### 医疗数据躺在哪些系统里

!![](public/hissystems.png .fullscreen)



<slide  class="bg-apple aligncenter ">

### 医疗数据还躺在哪里

!![](public/datacontainer.png .fullscreen)




<slide  class="bg-apple aligncenter ">

### 医疗数据的载体

!![](public/dataformat.png .fullscreen)



<slide class="bg-apple aligncenter">

# **第二部分：时代在呼唤** {.text-landing.text-shadow}



<slide  class="bg-apple aligncenter ">


!![](public/digitalization1.png .fullscreen)

<slide  class="bg-apple aligncenter ">


!![](public/digitalization2.png .fullscreen)



<slide  class="bg-apple aligncenter ">
## **数字化转型中可能的“挑战”**

:::column
### **:fa-line-chart: 数据层面**

格式不统一        
调用方式不统一    
数据标化处理能力弱

---
### **:fa-film: 系统层面**

系统孤岛    
系统复杂度太高    
开发能力弱

---
### **:fa-hospital-o: 业务层面**

业务需求变化快    
难度大、流程长、创新慢    


---
### **:fa-th: 信息技术**
信息架构落后    
IT交付能力的瓶颈    
集成技术(单点-ESB-API)
:::


<slide  class="bg-apple aligncenter ">

### 医院信息化规划和现实的鸿沟

!![](public/hitdream.png .fullscreen)
:::note
## Note here
:::


<slide  class="bg-apple aligncenter ">

### 医院信息化面临的挑战

!![](public/hitchallenge.png .fullscreen)
:::note
## Note here
:::




<slide class="bg-apple aligncenter">

# **第三部分：API、数据中台、微服务** {.text-landing.text-shadow}




<slide  class="bg-apple aligncenter ">


!![](public/api-time.png .fullscreen)
:::note
## Note here
从上图可以看到2015年后全球对API的认可，API相关公司的并购与上市持续不断。所有大图标都是这些年并购收购了一些相对小的公司，比如IBM收购StrongLoop，Google、Oracle这些公司收购API公司的意义就是更好的给企业提供整体架构层面的系统及应用集成的解决方案和产品。
:::

<slide  class="bg-apple aligncenter ">

## 数据中台

!![](public/api_pool.png .fullscreen)
:::note
## Note here
我们说的API是指三层API架构，这个架构只做三件事：第一件事是资源型API，即如何把系统、数据API化，用统一格式更方便被大家调用，是服务中间的流程。第二件事是协同流程API，即做业务编排、重组。第三件事是用户体验API，将企业的内部能力赋能并对外输出，交付给企业的内部与外部的合作伙伴，，为业务创新提供基础。
:::



<slide  class="bg-apple aligncenter ">

## 数据中台


!![](public/api-platform.png .fullscreen)
:::note
## Note here

数据中台包括了3个平台：API构建平台、API管理平台、集成编排平台。API构建平台解决了如何API化。让数据可以被访问和暴露，基于各种格式的API，以及浏览器架构、客户端架构，都可以到资源池里进行统一的管理，不需要依赖原厂。
 
　　API化不是目的，关键是要做集成。刚刚我们回顾了集成二十几年走过的路。最开始的点对点集成，系统多了以后无法管理、复用。之后我们找到一个突破口--SOA。其实就是把原来的业务和IT功能变成无处不在的、可以重复利用的服务。ESB也没有错，但是始终忽略一个问题，那就是所有系统连接、系统之间的接口复杂性一直没有解决，这就是造成我们所有应用集成的痛点所在。我们提出API的架构并不是要取代系统集成，而是要从更高的抽象层面把业务和数据抽象出来，把资源真正交到IT部门业务应用研发的手里，让自主可控的把业务研发实现。ESB是说我们把所有系统适应总线做集成。而我们这个恰恰是反过来，这就是我们说的解耦。

编排平台如何操作的？ERP、OA等系统，如何在他们之间做数据的集成，这里面穿插着业务集成甚至连接设备，我们在工业互联网连接IOT时如何把他们连接起来。上图我们一个3系统集成的编排流程事例，这个平台包括260多个组件，开发人员可以在平台上通过拖拽组件的方式完成流程的编排。
 
　　我们做的研发最终都服务于业务，如果这个交付延缓会影响到创新，这需要API管理平台。在管理平台上可以进行端到端的访问、控制、监控，谁访问的频次，以及所有系统的连接性、业务都可以进行展示。
 
　　我们的目标就是在这个领域做中国的第一名，我们希望用最强劲的互联网技术实力、最懂传统企业的实践经验来满足大B市场企业服务的需求，在整个数字化转型之路上与企业用户一路披荆斩棘，通过数字化转型真正实现弯道超车，使每个人都能受益。我想这是我们每一位CIO的职责。
:::


<slide  class="bg-apple aligncenter ">

## 数据中台

!![](public/api-vs-esb.png .fullscreen)
:::note
## Note here
API智能构建
政府机构和企业客户需要快速实现业务互联互通，而传统的方式无法快速响应频繁变化的业务需求，所以以API的方式连接业务应用系统，实现业务快速交互，利用核心构建技术，针对不同类型业务系统快速生成API。
1.原生API智能构建
每个业务应用系统内部不同模块之间都依赖内部接口进行通讯，内部接口以特定方式封装在系统内部环境，并不对外提供服务。数聚蜂巢能够利用AI方式实现智能发现接口，按照客户需求应用系统只能发现原生数据API和功能API，并只能对其进行封装，生成简洁易用的RESTful API。
2.模型驱动API构建
智能识别数据类型和模型规则，构建模型，驱动构建REST API。
3.多元数据API构建
全业务、全数据、全系统覆盖，针对不同数据源不同结构的数据构建REST API。

API全生命周期管理
1.API全方位动态感知
API全方位、多维度“透视”，通过360度API肖像，高效直观的呈现观测数据。
2.API全生命周期管理
发布、测试、运行、授权、流控、安全、告警、分析、退休等全生命周期的管理。
3.API全象限运营分析
API信息以四象限方式分析，实现数据价值最大化以支撑运营管理。

API跨界融合
API管网全域覆盖
应用、数据、IoT以API为载体，打通全域数据，消除数据孤岛，重塑数据价值。 
异构系统精准融合
异构系统功能API和数据API，按需精准实现云与云、云与本地、本地与本地融合。 
跨界资源敏捷编排
资源敏捷重构，重塑商业模式，让数据流通、应用集成更敏捷、应用服务更安全。 
在云计算逐渐成为主流，新的威胁不断冲击旧的防护手段的今天，白山云科技以其出众的云技术获得了广泛好评，以API作为数据和服务的载体，颠覆了传统的数据融合模式，为政府机构、企业部门提供精准的个性化服务。
:::


<slide  class="bg-apple">

## 数据发现的挑战

:::flexblock

## :fa-bar-chart: DB数据库数据

代码开发能力    
数据库表的理解

---

## :fa-bar-chart: C/S客户端数据

系统封闭程度     
操作系统版本(xp、win7、linux).

---

## :fa-balance-scale: B/S客户端数据

系统封闭程度

---

## :fa-cog: API接口数据

现有接口数量   
稳定性     
标准化程度(模型+术语字典).

:::

---
## API构建过程
:::flexblock {.blink.border}

## :fa-cog: DB -> API    

脱码API构建-商用软件    
脱码API构建-开源DIY    
有码API构建-商用软件    
有码API构建-开源DIY    
    

---

## :fa-bar-chart: C/S -> API  

高度定制       
逆向分析     

---

## :fa-balance-scale: B/S -> API  
       
脱码API构建-商用软件    
有码API构建-开源DIY  

---

## :fa-cog: API -> API  

高度定制    
脱码转换-商用软件    

:::

<slide  class="bg-apple aligncenter ">

## API管理平台
!![](public/api-gateway3.png .fullscreen)
:::note
## Note here
API管理平台提供API 的全生命周期管理，帮助企业获得运营洞察，企业可以进一步优化流程、改进产品与服务模式。API管理平台通过流控、权限管理、安全管理、运行、监控分析等功能可以实现：自主定义访问行为，按需控制频次;控制访问权限，保证访问安全;提高使用的保密性、完整性与可用性;快速弹性扩展;业务调用全程端到端监控、分析、大屏展示。通过多维度、细粒度的可视化分析，实时掌握数据使用情况，洞察企业内资源价值。
:::




<slide  class=" aligncenter ">

## 无网关系统架构<-->API网关架构

!![](public/api-gateway2-after.png .fullscreen)


<slide  class="bg-apple aligncenter ">

## 服务编排
!![](public/api-orch.png .fullscreen)
:::note
## Note here
:::


<slide class="bg-apple aligncenter">

# **第四部分：API构建的技术思路** {.text-landing.text-shadow}


<slide class=" aligncenter">

!![](public/api-creation-method.png .fullscreen)


<slide  class="bg-apple">

## API构建过程
:::flexblock {.blink.border}

## :fa-cog: DB -> API    

智能识别数据类型和模型规则，构建模型，驱动构建API。
    
    

---

## :fa-bar-chart: C/S -> API  

每个业务应用系统内部不同模块之间都依赖内部接口进行通讯，
内部接口以特定方式封装在系统内部环境，并不对外提供服务。
利用AI方式实现智能发现接口，     
只能发现原生数据API和功能API，
并只能对其进行封装。
      
     

---

## :fa-balance-scale: B/S -> API  
       
所见即所得，浏览器中可以查看的业务数据都可以将其封装成API

---

## :fa-cog: API -> API  

系统供应商提供的非标接口    
系统供应商提供的标化接口     

:::


<slide class="bg-apple aligncenter">

## 思路A

---

* 传统信息平台/集成平台/ESB多采用此思路
* 需医院协调不同系统供应商
* 需不同系统供应商确定接口文档、提供开发资源、完成接口实现
* 合作伙伴配合意愿、积极性差
* 接口费狮子大张口
* 接口开发、联调测试工期失控
* 接口可靠性、安全性差
* 接口调整、版本更新时沟通、开发成本高
* 无法一次开发、多次利用
* 视图是一种特殊的表，需按需创建，供调用方后端使用(前端调用会暴露数据库地址端口)


<slide class=" aligncenter">
## 思路B

!![](public/bs-api.png .fullscreen)
<slide  class="bg-apple">

## 针对BS架构业务系统的API构建技术方案
:::flexblock {.blink.border}
## :fa-cog: 数据库层面    

* ETL(以备库、dump形式实现实时/定时、全量/增量数据抽取)
* 开放数据库表
* 视图
* 接口自动生成(apijson/graphql/prisma/postgrest)
* 商用解决方案
    
---

## :fa-balance-scale: UI层面  
       
* 开源DIY：爬虫技术不做赘述
* 商用：diffbot、import.io、metabase

---

## :fa-cog: 服务端层面

系统供应商不配合、没有数据库表结构，      
逆向分析发现原生数据API和功能API，

:::
## 优缺点

:::flexblock {.blink.border}
## :fa-cog: 数据库层面    

* 需要数据库用户名密码
* 需熟悉表结构
* 脱码(拖拽配置)VS代码开发
* 数据最丰富全面
* 自助、无需厂商配合
* 无接口费、成本低    
---

## :fa-balance-scale: UI层面  
       
* 不需要数据库用户名密码
* 数据只能采集局部
* 成本最低    

---

## :fa-cog: 服务端层面

* 数据只能采集局部
* 逆向分析需耗费人力时间
* 成本高   


:::



<slide class=" aligncenter">
## 思路C

!![](public/cs-api.png .fullscreen)
<slide  class="bg-apple">

## 针对CS架构业务系统的API构建技术方案
:::flexblock {.blink.border}
## :fa-cog: 数据库层面    

* ETL(以备库、dump形式实现实时/定时、全量/增量数据抽取)
* 开放数据库表
* 视图
* 接口自动生成(apijson/graphql/prisma/postgrest)
* 商用解决方案
    
---

## :fa-balance-scale: 客户端层面  
       
* 虚拟打印：自助打印设备厂商应用很成熟
* 桌面截屏：RPA公司 (UIPATH/按键精灵)提供类似产品
* 开源 VS 商用，拖拽 VS 代码
---

## :fa-cog: 服务端层面

系统供应商不配合、没有数据库表结构，      
逆向分析发现原生数据API和功能API，

:::
## 优缺点

:::flexblock {.blink.border}
## :fa-cog: 数据库层面    

* 需要数据库用户名密码
* 需熟悉表结构
* 脱码(拖拽配置)VS代码开发
* 数据最丰富全面
* 自助、无需厂商配合
* 无接口费、成本低    
---

## :fa-balance-scale: 客户端层面  
       
* 不需要数据库用户名密码
* 数据只能采集局部
* 脱码(拖拽配置)VS代码开发
* 逆向分析需耗费人力时间
* 数据可直接入库 VS 不可以直接入库
* 成本最低    

---

## :fa-cog: 服务端层面

* 数据只能采集局部
* 逆向分析需耗费人力时间
* 成本高   


:::


<slide class=" aligncenter">
## 不可直接入库的数据处理

!![](public/data-process.png .fullscreen)



<slide class="bg-apple aligncenter">

# **第五部分：具体技术、产品介绍** {.text-landing.text-shadow}




<slide class="bg-apple aligncenter">
#  DB---API系列工具


:::flexblock {.border}

传统 rest  
* `php-crud-api`
* `DreamFactory`
* `sandman2`
* `ZenQuery`
* `postgrest`
* `xmysql`
* `oracle-rest-api`

---

apijson

* `APIJSON.NET`
* `apijson-php`
* `uliweb-apijson`
* `APIJSONParser`

---

graphql

* `Prisma`
* `Sequelize`
* `join-monster`
* `tentaQL`

:::



<slide class="bg-apple aligncenter">

# **5.1：apijson 产品介绍** {.text-landing.text-shadow}




<slide class="bg-apple aligncenter">

##  如果你满足以下若干条件请考虑使用
---

* 1 有业务创新的需求 {.animated.fadeInUp}
* 1.1 想基于已有业务系统的数据开发新的应用 {.animated.fadeInUp.delay-400}
* 1.1.1 拥有已有业务系统的数据库用户名密码 {.animated.fadeInUp.delay-800}
* 1.1.2 已有业务系统厂商配合意愿低、开发水平差、接口费高 {.animated.fadeInUp.delay-1200}
* 1.1.3 接口数量大且需求可能会持续变化，需协调多方配合 {.animated.fadeInUp.delay-1600}
* 1.1.4 开发人员不足 工期短 {.animated.fadeInUp.delay-2s}
* 1.2 想从头开始开发新的应用 培养技术人员能力 {.animated.fadeInUp.delay-2400}
* 1.2.1 快速实现  专注业务逻辑 {.animated.fadeInUp.delay-2800}
* 1.2.2 文档清晰可读永远最新  减少沟通 {.animated.fadeInUp.delay-3200}
* 1.2.2 前后端分离 {.animated.fadeInUp.delay-3600}



<slide class="size-80  aligncenter">
### c# 版本安装配置一览-基础环境安装

---

```shell {.animated.fadeInUp}
# 第一步、运行命令验证sdk是否安装成功：
# windows:https://www.microsoft.com/net/download/thank-you/dotnet-sdk-2.1.301-windows-x64-installer        
# linux:https://www.microsoft.com/net/download/linux     
# macos:https://www.microsoft.com/net/download/macos

$ dotnet -v

```
<slide class="size-80  aligncenter">
### c# 版本安装配置一览-项目发布

---

```shell {.animated.fadeInUp}
# 第二步、发布项目
# APIJSON.NET文件夹下运行cmd命名
# 生成在bin/release/netcoreapp2.1/publish目录下

$ dotnet publish -c release 

```

<slide class="size-80  aligncenter">
### c# 版本安装配置一览-运行项目

---

```shell {.animated.fadeInUp}
# 第三步、运行项目
# 打开publish文件 运行cmd命令： 

$ dotnet APIJSON.NET.dll

```

<slide class="size-80  aligncenter">
### c# 版本安装配置一览-配置

---

```shell {.animated.fadeInUp}
# 第四步、修改配置文件。appsettings.json文件配置说明（数据库配置，权限配置，表映射配置） 
# 根据你要用到的数据库、数据库中待开放的表和字段、以及开放的用户和对象
# 如下图所示
```
!![figure](public/api-setting.png .aligncenter.animated.fadeInUp.delay-400)

<slide class="bg-apple aligncenter">

## appsettings.json文件配置说明
!![figure](public/api-setting.png .aligncenter.animated.fadeInUp.delay-400)



<slide class="bg-apple aligncenter">
# 开启apijson的旅程吧 {.text-landing}


<slide class="bg-apple aligncenter">
# 请求中的JSON------>后台的SQL {.text-landing}
## 支持MySQL, PostgreSQL, MS SQL Server, Oracle, SQLite



<slide class="bg-apple aligncenter">
## 特点功能

| 接口管理工具 | 前端开发的优势 | 后端开发的优势 |
| :----------- | :------------: | ------------: |
| 自动生成文档，清晰可读永远最新   |   不用再向后端催接口、求文档   |   提供通用接口，大部分API不用再写 |
| 自动生成请求代码，支持Android和iOS    |   数据和结构完全定制，要啥有啥    |    支持增删改查、模糊搜索、正则匹配、远程函数等 |
| 自动管理与测试接口用例，一键共享  |   可一次获取任何数据、任何结构   |   自动校验权限、自动管理版本、自动防SQL注入 |
| 自动校验与格式化JSON，支持高亮和收展  |  能去除重复数据，节省流量提高速度  |   开放API无需划分版本，始终保持兼容 |




<slide class="bg-apple aligncenter">
## 以java为例，传统rest方式接口开发流程
![](https://raw.githubusercontent.com/TommyLemon/APIJSON/master/assets/1545468341131.png)


<slide class="bg-apple aligncenter">
## 以java为例，基于apijson的接口开发流程
![](https://raw.githubusercontent.com/TommyLemon/APIJSON/master/assets/1545468361962.png)

:::note
换句说，使用这个项目作为后端的支持的话，是不需要对每个表写增删改等接口的，只需在该项目连接的数据里进行表的创建，以及配置接口权限即可。无需进行过多的开发，哪怕是要改结构也仅仅只需要修改表字段而已。想想仅仅是部署一个后端项目，现在需要些的接口就基本写好了，直接调用就行了，是不是挺爽的。

:::

<slide class="bg-apple aligncenter">

## 开发流程对比

| 开发流程 | RESTful | APIJSON |
| :----------- | :------------: | ------------: |
| 接口传输   |   等后端编辑接口，然后更新文档，前端再按照文档编辑请求和解析代码   |   前端按照自己的需求编辑请求和解析代码。 |
| 兼容旧版    |   后端增加新接口，用v2表示第2版接口，然后更新文档    |    什么都不用做！ |


<slide class="bg-apple aligncenter">

## 前端请求对比

| 前端请求 | RESTful | APIJSON |
| :----------- | :------------: | ------------: |
| 要求   |   前端按照接口文档在对应URL后面按照事先约定拼接键值对   |   前端按照自己的需求在固定URL后拼接JSON |
| URL    |   不同的请求对应不同的URL，基本上有多少个不同的请求就得有多少个接口URL    |    相同的操作方法(增删改查)都用同一个URL，大部分请求属于7个通用接口 |
| 键值对   |   key=value   |   key:value |
| 结构   |   同一个URL内table_name只能有一个    |   同一个URL后TableName可传任意数量个  |

<slide class="bg-apple aligncenter">

## 后端开发对比

| 前端请求 | RESTful | APIJSON |
| :----------- | :------------: | ------------: |
| 解析和返回   |   取出键值对，把键值对作为条件用预设的的方式去查询数据库，最后封装JSON并返回给前端   |   把Parser#parse方法的返回值返回给前端就行 |
| 返回JSON结构的设定方式    |   事先约定，前端不能修改    |    由前端自由控制 |



<slide class="bg-light aligncenter">


:::flexblock

## **前端的请求**

数据需求：User

---

## **传统rest方式**

```
base_url/get/user?id=38710
```
---

## **APIJSON**

```
base_url/get/
{
   "User":{
     "id":38710
   }
}
```

:::

---


:::flexblock {.blink.border}

## **后端的返回结果**
数据需求：User


---

## **传统rest方式**

```
{
   "data":{
     "id":38710,
     "name":"xxx",
     ...
   },
   "code":200,
   "msg":"success"
}
```
---

## **APIJSON**

```
{
   "User":{
     "id":38710,
     "name":"xxx",
     ...
   },
   "code":200,
   "msg":"success"
}
```
:::

:::note



1.base_url指基地址，一般是顶级域名，其它分支url都是在base_url后扩展。如base_url:http://apijson.cn:8080/ ，对应的GET分支url:http://apijson.cn:8080/get/ 。下同。
2.请求中的key或value任意一个为null值时，这个 key:value键值对 被视为无效。下同。
3.请求中的 / 需要转义。JSONRequest.java已经用URLEncoder.encode转义，不需要再写；但如果是浏览器或Postman等直接输入url/request，需要把request中的所有 / 都改成 %252F 。下同。
4.code，指返回结果中的状态码，200表示成功，其它都是错误码，值全部都是HTTP标准状态码。下同。
5.msg，指返回结果中的状态信息，对成功结果或错误原因的详细说明。下同。
6.code和msg总是在返回结果的同一层级成对出现。对所有请求的返回结果都会在最外层有一对总结式code和msg。对非GET类型的请求，返回结果里面的每个JSONObject里都会有一对code和msg说明这个JSONObject的状态。下同。
7.id等字段对应的值仅供说明，不一定是数据库里存在的，请求里用的是真实存在的值。下同。
::::


<slide class="bg-light aligncenter">


:::flexblock

## **前端的请求**

数据需求：Moment和对应的User

---

## **传统rest方式**

```
分两次请求
Moment:
base_url/get/moment?userId=38710

User:
base_url/get/user?id=38710
```
---

## **APIJSON**

```
base_url/get/
{
   "Moment":{
     "userId":38710
   },
   "User":{
     "id":38710
   }
}
```

:::

---


:::flexblock {.blink.border}

## **后端的返回结果**
数据需求：Moment和对应的User


---

## **传统rest方式**

```
分别返回两次请求的结果，获取到Moment
后取出userId作为User的id条件去查询User

Moment:
{
   "data":{
     "id":235,
     "content":"xxx",
     ...
   },
   "code":200,
   "msg":"success"
}

User:
{
   "data":{
     "id":38710,
     "name":"xxx",
     ...
   },
   "code":200,
   "msg":"success"
}
```
---

## **APIJSON**

```
一次性返回，没有传统方式导致的
长时间等待结果、两次结果间关联、线程多次切换 等问题

{
   "Moment":{
     "id":235,
     "content":"xxx",
     ...
   },
   "User":{
     "id":38710,
     "name":"xxx",
     ...
   },
   "code":200,
   "msg":"success"
}
```
:::
<slide class="bg-light aligncenter">


:::flexblock

## **前端的请求**

数据需求：User列表

---

## **传统rest方式**

```
base_url/get/user/list?
page=0&count=3&sex=0
```
---

## **APIJSON**

```
base_url/get/
{
   "User[]":{
     "page":0,
     "count":3,
     "User":{
       "sex":0
     }
   }
}
```

:::

---


:::flexblock {.blink.border}

## **后端的返回结果**
数据需求：User列表


---

## **传统rest方式**

```
{
   "data":[
     {
       "id":38710,
       "name":"xxx",
       ...
     },
     {
       "id":82001,
       ...
     },
     ...
   ],
   "code":200,
   "msg":"success"
}
```
---

## **APIJSON**

```
{
   "User[]":[
     {
       "id":38710,
       "name":"xxx",
       ...
     },
     {
       "id":82001,
       ...
     },
     ...
   ],
   "code":200,
   "msg":"success"
}
```
:::
<slide class="bg-light aligncenter">


:::flexblock

## **前端的请求**

数据需求：Moment列表，
每个Moment包括
1.发布者User
2.前3条Comment

---

## **传统rest方式**

```
Moment里必须有
1.User对象
2.Comment数组

base_url/get/moment/list?
page=0&count=3&commentCount=3
```
---

## **APIJSON**

```
base_url/get/
{
   "[]":{
     "page":0,
     "count":3,
     "Moment":{},
     "User":{
       "id@":"/Moment/userId"
     },
     "Comment[]":{
       "count":3,
       "Comment":{
         "momentId@":"[]/Moment/id"
       }
     }
   }
}
```

:::

---


:::flexblock {.blink.border}

## **后端的返回结果**
数据需求：Moment列表，
每个Moment包括
1.发布者User
2.前3条Comment


---

## **传统rest方式**

```
Moment里必须有
1.User对象
2.Comment数组

{
   "data":[
     {
       "id":235,
       "content":"xxx",
       ...,
       "User":{
         ...
       },
       "Comment":[
         ...
       ]
     },
     {
       "id":301,
       "content":"xxx",
       ...,
       "User":{
         ...
       },
       ...
     },
     ...
   ],
   "code":200,
   "msg":"success"
}
```
---

## **APIJSON**

```
1.高灵活，可任意组合
2.低耦合，逻辑很清晰

{
   "[]":[
     {
       "Moment":{
         "id":235,
         "content":"xxx",
         ...
       },
       "User":{
         ...
       },
       "Comment[]":[
         ...
       ]
     },
     {
       "Moment":{
         "id":301,
         "content":"xxx",
         ...
       },
       "User":{
         ...
       },
       ...
     },
     ...
   ],
   "code":200,
   "msg":"success"
}
```
:::
<slide class="bg-light aligncenter">


:::flexblock

## **前端的请求**

数据需求：User发布的Moment列表，每个Moment包括发布者User和前3条Comment

---

## **传统rest方式**

```
1.Moment里必须有User对象和Comment数组
2.字段名必须查接口文档，例如评论数量字段名可能是
commentCount,comment_count或者简写cmt_count等各种奇葩写法...

base_url/get/moment/list?
page=0&count=3
&commentCount=3&userId=38710
```
---

## **APIJSON**

```
1.Moment里必须有User对象和Comment数组
2.字段名必须查接口文档，例如评论数量字段名可能是
commentCount,comment_count或者简写cmt_count等各种奇葩写法...

base_url/get/moment/list?
page=0&count=3
&commentCount=3&userId=38710 	有以下几种方式:

① 把以上请求里的
"Moment":{}, "User":{"id@":"/Moment/userId"}
改为
"Moment":{"userId":38710}, "User":{"id":38710}

② 或把User放在上面的最外层省去重复的User
base_url/get/
{
   "User":{
     "id":38710
   },
   "[]":{
     "page":0,
     "count":3,
     "Moment":{
       "userId":38710
     },
     "Comment[]":{
       "count":3,
       "Comment":{
         "momentId@":"[]/Moment/id"
       }
     }
   }
}

③ 如果User之前已经获取到了，还可以不传User来节省请求和返回数据的流量并提升速度
base_url/get/
{
   "[]":{
     "page":0,
     "count":3,
     "Moment":{
       "userId":38710
     },
     "Comment[]":{
       "count":3,
       "Comment":{
         "momentId@":"[]/Moment/id"
       }
     }
   }
}
```

:::

---


:::flexblock {.blink.border}

## **后端的返回结果**
数据需求：User发布的Moment列表，每个Moment包括发布者User和前3条Comment


---

## **传统rest方式**

```
1.大量重复User，浪费流量和服务器性能
2.优化很繁琐，需要后端扩展接口、写好文档，前端/前端再配合优化

{
   "data":[
     {
       "id":235,
       "content":"xxx",
       ...,
       "User":{
         "id":38710,
         "name":"Tommy"
         ...
       },
       "Comment":[
         ...
       ]
       ...
     },
     {
       "id":470,
       "content":"xxx",
       ...,
       "User":{
         "id":38710,
         "name":"Tommy"
         ...
       },
       "Comment":[
         ...
       ]
       ...
     },
     {
       "id":511,
       "content":"xxx",
       ...,
       "User":{
         "id":38710,
         "name":"Tommy"
         ...
       },
       "Comment":[
         ...
       ]
       ...
     },
     {
       "id":595,
       "content":"xxx",
       ...,
       "User":{
         "id":38710,
         "name":"Tommy"
         ...
       },
       "Comment":[
         ...
       ]
       ...
     },
     ...
   ],
   "code":200,
   "msg":"success"
}
```
---

## **APIJSON**

```
以上不同请求方式的结果:

① 常规请求
{
   "[]":[
     {
       "Moment":{
         "id":235,
         "content":"xxx",
         ...
       },
       "User":{
         "id":38710,
         "name":"Tommy"
         ...
       },
       "Comment[]":[
         ...
       ]
     },
     ...
   ],
   "code":200,
   "msg":"success"
}

② 省去重复的User
{
   "User":{
     "id":38710,
     "name":"Tommy",
     ...
   },
   "[]":[
     {
       "Moment":{
         "id":235,
         "content":"xxx",
         ...
       },
       "Comment[]":[
         ...
       ]
     },
     ...
   ],
   "code":200,
   "msg":"success"
}

③ 不查询已获取到的User
{
   "[]":[
     {
       "Moment":{
         "id":235,
         "content":"xxx",
         ...
       },
       "Comment[]":[
         ...
       ]
     },
     ...
   ],
   "code":200,
   "msg":"success"
}
```
:::
<slide class="bg-light aligncenter">

## APIJSON 接口说明
```
1.TableName指要查询的数据库表Table的名称字符串。第一个字符为大写字母，剩下的字符要符合英语字母、数字、下划线中的任何一种。对应的值的类型为JSONObject，结构是 {...}，里面放的是Table的字段(列名)。下同。
2."tag":tag 后面的tag是非GET、HEAD请求中匹配请求的JSON结构的key，一般是要查询的table的名称，由后端Request表中指定。下同。
3.GET、HEAD请求是开放请求，可任意组合任意嵌套。其它请求为受限制的安全/私密请求，对应的 方法、tag、结构 都必须和 后端Request表中所指定的 一一对应，否则请求将不被通过。下同。
4.GETS与GET、HEADS与HEAD分别为同一类型的操作方法，请求稍有不同但返回结果相同。下同。
5.在HTTP通信中，自动化接口(get,gets,head,heads,post,put,delete) 全用HTTP POST请求。下同。
6.所有JSONObject都视为容器(或者文件夹)，结构为 {...} ，里面可以放普通对象或子容器。下同。
7.每个对象都有一个唯一的路径(或者叫地址)，假设对象名为refKey，则用 key0/key1/.../refKey 表示。下同。

```
<slide class="bg-light aligncenter">

:::flexblock

## **名称**

GET:
普通获取数据，
可用浏览器调试

---

## **url**


```
base_url/get/
```
---

## **请求**

```
{
   TableName:{
     …
   }
}
{…}内为限制条件

例如获取一个id为235的Moment：
{
   "Moment":{
     "id":235
   }
}
```
---

## **响应**

```
{
   TableName:{
     ...
   },
   "code":200,
   "msg":"success"
}
例如
{
   "Moment":{
     "id":235,
     "userId":38710,
     "content":"APIJSON,let interfaces and documents go to hell !"
   },
   "code":200,
   "msg":"success"
}
```

:::

<slide class="bg-light aligncenter">

:::flexblock

## **名称**

HEAD:
普通获取数量，
可用浏览器调试

---

## **url**


```
base_url/head/
```
---

## **请求**

```
{
   TableName:{
     …
   }
}
{…}内为限制条件

例如获取一个id为38710的User所发布的Moment总数：
{
   "Moment":{
     "userId":38710
   }
}
```
---

## **响应**

```
{
   TableName:{
     "code":200,
     "msg":"success",
     "count":10
   },
   "code":200,
   "msg":"success"
}
例如
{
   "Moment":{
     "code":200,
     "msg":"success",
     "count":10
   },
   "code":200,
   "msg":"success"
}
```

:::

<slide class="bg-light aligncenter">

:::flexblock

## **名称**

GETS:
安全/私密获取数据，
用于获取钱包等
对安全性要求高的数据

---

## **url**


```
base_url/gets/
```
---

## **请求**

```
最外层加一个"tag":tag，其它同GET
```
---

## **响应**

```
同GET
```

:::
<slide class="bg-light aligncenter">

:::flexblock

## **名称**

HEADS:
安全/私密获取数量，
用于获取银行卡数量等
对安全性要求高的数据总数

---

## **url**


```
base_url/heads/
```
---

## **请求**

```
最外层加一个"tag":tag，其它同HEAD
```
---

## **响应**

```
同HEAD
```

:::
<slide class="bg-light aligncenter">

:::flexblock

## **名称**

POST:
新增数据

---

## **url**


```
base_url/post/
```
---

## **请求**

```
{
   TableName:{
     …
   },
   "tag":tag
}
{…}中id由后端生成，不能传

例如一个id为38710的User发布一个新Moment：
{
   "Moment":{
     "userId":38710,
     "content":"APIJSON,let interfaces and documents go to hell !"
   },
   "tag":"Moment"
}
```
---

## **响应**

```
{
   TableName:{
     "code":200,
     "msg":"success",
     "id":38710
   },
   "code":200,
   "msg":"success"
}
例如
{
   "Moment":{
     "code":200,
     "msg":"success",
     "id":120
   },
   "code":200,
   "msg":"success"
}
```

:::
<slide class="bg-light aligncenter">

:::flexblock

## **名称**

PUT:
修改数据，
只修改所传的字段

---

## **url**


```
base_url/put/
```
---

## **请求**

```
{
   TableName:{
     "id":id,
     …
   },
   "tag":tag
}
{…}中id必传

例如修改id为235的Moment的content：
{
   "Moment":{
     "id":235,
     "content":"APIJSON,let interfaces and documents go to hell !"
   },
   "tag":"Moment"
}
```
---

## **响应**

```
同POST
```

:::
<slide class="bg-light aligncenter">

:::flexblock

## **名称**

DELETE:
删除数据

---

## **url**


```
base_url/delete/
```
---

## **请求**

```
{
   TableName:{
     "id":id
   },
   "tag":tag
}
{…}中id必传，一般只传id

例如删除id为120的Moment：
{
   "Moment":{
     "id":120
   },
   "tag":"Moment"
}
```
---

## **响应**

```
同POST
```

:::



<slide class="bg-light aligncenter">

## **参考资料**

---

* 1.更多资料请查看 https://github.com/TommyLemon/APIJSON
* 2.自动化接口管理工具 http://apijson.org/
* 3.多语言支持(c#/nodejs/java/php/python)
