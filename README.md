手拉手业务基础平台hihsoft-sso
==============================================================================================================
1.1框架简介
----------------------------------------------------------------------------------------------------
###
Hihsoft业务基础平台目标定位有两个：
###
一是通过持续提供丰富的可复用组件和图形化开发方式，降低应用开发人员对技术细节的依赖，提高项目的开发效率；
###
二是通过业务基础平台拥有良好地编程规范和统一的技术开发框架，保障应用的高稳定性和高扩展性
###
最终服务于各行业的“信息管理”领域，可用作后台管理类系统、各行业的信息化管理系统建设等。
###
着力打造一个轻量级、性能良好、快速开发的业务基础平台。
###
本框架以Spring Framework为核心、Spring MVC作为模型视图控制器、JDBC + Hibernate作为数据库持久化，
###
前端引入开源版本的JQuery EasyUI是一个简单、易学的综合性业务基础平台。
1.2文档精要：
------------------------------------------------------------------
###
1、[hihsoft业务基础平台开发手册.pdf](https://github.com/hihsoft/sso/raw/master/hihsoft-sso/doc/hihsoft%E4%B8%9A%E5%8A%A1%E5%9F%BA%E7%A1%80%E5%B9%B3%E5%8F%B0%E5%BC%80%E5%8F%91%E6%89%8B%E5%86%8C.pdf)
###
2、[hihsoft业务基础平台总体设计方案.pdf](https://github.com/hihsoft/sso/raw/master/hihsoft-sso/doc/hihsoft%E4%B8%9A%E5%8A%A1%E5%9F%BA%E7%A1%80%E5%B9%B3%E5%8F%B0%E6%80%BB%E4%BD%93%E8%AE%BE%E8%AE%A1%E6%96%B9%E6%A1%88.pdf)
###
文档持续更新中。。。。。。。
1.3在线体验：
------------------------------------------------------------------
体验地址：http://www.javahih.com/sso

用户名：admin 密码：admin
###
![hihsoft](https://github.com/hihsoft/sso/raw/master/hihsoft-sso/doc/login.png "hihsoft") 
![hihsoft](https://github.com/hihsoft/sso/raw/master/hihsoft-sso/doc/main.png "hihsoft") 

1.4 为何选择
---------------------------------------------------------------------------
###
1、使用[Apache License 2.0协议](http://www.apache.org/licenses/LICENSE-2.0)，源代码完全开源，无商业限制。
###
2、使用目前最主流的J2EE开发框架，简单易学，学习成本低。
###
3、数据库无限制，支持MySql、Oracle、SQL Server、H2等数据库
###
4、能良好地支持各种应用服务器：Tomcat、weblogic、websphere、JBoss、Jetty等
###
5、完全兼容目前最流行浏览器（IE7+、Firefox、Chrome等）。
###
6、模块化设计，MVC架构，层次结构清晰。内置一系列信息管理的基础功能。
###
7、内置和封装了一系列标签taglibs：字典标签、分页标签、权限标签等
###
8、权限支持按钮级控制、分级授权、分级管理。
1.5  应用场景
-------------------------------------------------------------------------------
###
主要应用于集团型企业信息管理系统：例如企业型：集团、股份公司、分公司、网点等不同级别的
综合业务管理系统,例如：企业ERP系统、人力资源系统、客户关系系统等。
不同行业数据集中型的业务管理系统，政府行业的省、市、县、乡镇多级的数据型的业务管理系统：
例如国家财政、两税（地税、国税）、金融、公安、电信等不同体系下的联网系统。
1.6 核心技术
-------------------------------------------------------------------------
###
1、  Services相关
###
Core Framework：Spring Framework 3.2。
###
2、	Web相关
###
a)	MVC Framework：Spring MVC 3.2。
###
b)	JavaScript Library：JQuery。
###
c)	JSTL:统一标签语言
###
d)	JavaScript/CSS Compressor：YUI Compressor 2.4。
###
e)	Front Validation：JQuery Validation Plugin 1.11。
###
3、	Database相关
###
a)	ORM Framework：Hibernate 3.6。
###
b)	Connection Pool：BoneCP 0.7
###
c)	Cache：Ehcache 2.6。
###
4、	模板语言
###
a)	Freemarker：2.3.16
###
5、	Tools 相关
###
a)	Commons：Apache Commons
###
b)	JSON Mapper：json
###
c)	Log Manager：Log4j 1.2.16
###
6、	Other
###
a)	Excel处理：jxl
###
b)	图形化处理：Fusionchart
###
7、	测试框架
###
a)	单元测试：Junit4
1.7框架特点
---------------------------------------------------------------------------------
### 
1、分辨率自适应：解决在不同分辨率下，系统能够正常显示。
###
2、开发语言：系统采用Java 语言开发，具有卓越的通用性、高效性、平台移植性和安全性。
###
3、分层设计：（数据库层，数据访问层，业务逻辑层，展示层）层次清楚，低耦合，
各层必须通过接口才能接入并进行参数校验（如：在展示层不可直接操作数据库），保证数据操作的安全。
###
4、双重验证：用户表单提交双验证：包括服务器端验证及客户端验证，防止用户通过浏览器恶意修改
    （如不可写文本域、隐藏变量篡改、上传非法文件等），跳过客户端验证操作数据库。
###
5、安全编码：用户表单提交所有数据，在服务器端都进行安全编码，防止用户提交非法脚本
及SQL注入获取敏感数据等，确保数据安全。
###
6、密码加密：登录用户密码进行SHA1散列加密，此加密方法是不可逆的。保证密文泄露后的安全问题。
###
7、强制访问：系统对所有管理端链接都进行用户身份权限验证，防止用户直接通过URL进行未授权页面
1.8    交流、反馈、参与贡献
-------------------------------------------------------------------------------
###
QQ群：80186309，身份验证码：以码会友
###
E-mail：hihsoft@gmail.com
###
Github：https://github.com/hihsoft/sso
###
如果你想参与进来共同完善它或有更好的建议，请联系我吧(^_^)。
