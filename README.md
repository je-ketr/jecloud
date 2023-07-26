

# 说明
## 1、JECloud 是由10个后端子项目、12个前端子项目、4个中间件项目构成。
## 2、下载源码请点击第八、第九、第十小节目录索引。


![logo](docs/images/logo.png)

# JECloud基于微服务架构的低代码平台（项目总入口目录）
## 一、项目简介

JECloud平台后端采用微服务架构，前端采用微应用架构，可做到不同服务使用不通数据库独立运行。全平台采用基于模型驱动的设计模式，并在前后端留有大量的代码植入入口，方便开发者对平台进行改造扩充。JECloud适合软件开发公司、企业信息中心、个人开发者使用，适用于开发ERP、OA、CRM、EAM、WMS、MES、PM等企业级信息化系统，是企业数字化转型的必备工具。

## 二、常见问题
1、JECloud开源版是什么协议，商业使用免费的吗？

答：JECloud使用MIT协议，开源版商业使用是免费的。

2、JECloud诞生于哪家公司，为什么要做开源？

答：JECloud出自北京凯特伟业科技有限公司（国有全资企业），出于提高产品知名度，构建基于JECloud的生态体系为核心目标创建开源社区。

3、JECloud的成长历程是什么样的？

答：JECloud团队在低代码领域摸爬滚打十余年，从早期的JEPF到JEPaaS到最终的JECloud见证了团队和产品的持续性成长，JECloud历经3年的开发时间于2022年6月发布1.0的产品，此后历经1年的时间打磨于2023年7月正式发布2.0产品且开源版上线。

4、JECloud中提到的私有证书是什么意思？

答：JECloud免费证书会展示“技术支持：凯特伟业”字样，如需更换需使用“私有证书”，私有证书会收取少许费用用于维持JECloud团队正常运转（尊重原创，请勿破解）。

5、JECloud开发环境和运行环境是一体的吗？

答：JECloud是基于模型驱动的低代码平台，而非传统意义的代码生成器，需要配合解释器一同运行。故此二次开发的项目需要在JECloud引擎下才可运行。

6、JECloud为什么选择华为的ServiceComb作为微服务底座而非SpringCloud？

答：从三个角度阐述，首先JECloud核心团队主要服务于国央企、政府、军工，此类企业对国产化要求极高，故此选择国产微服务中间件，其次在使用过程中团队发现ServiceComb在易用性、扩展性、安全性上具有较强的优势。最后如使用者如需要更换SpringCloud对平台整体影响不大，更换成本不高。

7、JECloud是否支持全国产化适配？

答：JECloud支持全国产化环境部署但开源版本仅支持MySQL数据库。

8、学习JECloud使用需要具备的专业知识有那些？

答：基于JECloud的项目开发人员分为“配置开发”、与“代码开发”两类角色，其中配置开发角色非软件专业人员即可胜任，代码开发角色需要具备SQL、Java、JavaScript基础知识的专业人员担任。3天上手，14天上岗，3个月精通。

## 三、资源文档
- [官方网站](http://jecloud.net)
- [帮助文档](https://doc.jepaas.com/docs/je-doc-jecloud-help/je-doc-jecloud-help-1e2ka6h6mrfhi)
- [视频教程](https://space.bilibili.com/519497352/channel/series)

## 四、版本信息
- [更新日志](./CHANGELOG.md)
- [版本升级包下载](./upgrade/README.md)

## 五、系统演示
- [演示系统（每日12点、24点系统自动回复默认数据库状态）](http://example.jecloud.net)
- 用 户 名：admin
- 密    码：123456

## 六、项目部署
1、安装版（仅支持Linux）
- [安装包下载](https://jecloud.net/experience)
- [安装手册下载](https://doc.jepaas.com/docs/je-doc-jecloud-help/je-doc-jecloud-help-1eidf5a6pbrrk)

2、Docker-Compose版（支持Linux、Windows）
- [安装包下载](https://jecloud.net/experience)
- [安装手册下载](https://doc.jepaas.com/docs/je-doc-jecloud-help/je-doc-jecloud-help-1eie6mb20uqei)

3、自定义部署（请自行下载各分子项目打包部署）

## 七、技术选型
- 开发语言：Java，JavaScript
- 技术架构：后端项目采用微服务架构，前端项目采用微前端架构
- 数 据 库：开源版仅支持MySQL
- 后端项目：ServiceCenter、ServiceComb、SkyWalking、OpenResty、Service Edge、
Redis、Apollo、XXLJob、RocketMQ、Promethus、SpringBoot2、Maven、
SpringMVC、Activiti 7、MyBatis
- 前端项目：Vue3、VueRouter4、Pinia2、Vuei18n 9、Less3、Micro-zoe、Dayjs、
AntDesign Vue3、Webpack 4、Gulp4、Lerna4、VxeTable、MxGraph、
Sortablejs、Lodash

## 八、后端项目
- [基础项目（jecloud-common）](https://gitee.com/ketr/jecloud-common.git)
- [动态网关项目（jecloud-gateway）](https://gitee.com/ketr/jecloud-gateway.git)
- [元数据项目（jecloud-meta）](https://gitee.com/ketr/jecloud-meta.git)
- [RBAC项目（jecloud-rbac）](https://gitee.com/ketr/jecloud-rbac.git)
- [工作流项目（jecloud-workflow）](https://gitee.com/ketr/jecloud-workflow.git)
- [文档项目（jecloud-document）](https://gitee.com/ketr/jecloud-document.git)
- [消息项目（jecloud-messasge）](https://gitee.com/ketr/jecloud-messasge.git)
- [连接器项目（jecloud-connector）](https://gitee.com/ketr/jecloud-connector.git)
- [案例项目（jecloud-demo）](https://gitee.com/ketr/jecloud-demo.git)
- [骨架项目（jecloud-service-archetype）](https://gitee.com/ketr/jecloud-service-archetype.git)

## 九、前端项目
- [主项目（jecloud-pc-admin）](https://gitee.com/ketr/jecloud-pc-admin.git)
- [骨架项目（jecloud-pc-archetype）](https://gitee.com/ketr/jecloud-pc-archetype.git)
- [基础库项目（jecloud-pc-libs）](https://gitee.com/ketr/jecloud-pc-libs.git)
- [资源表项目（jecloud-pc-table）](https://gitee.com/ketr/jecloud-pc-table.git)
- [应用中心项目（jecloud-pc-function）](https://gitee.com/ketr/jecloud-pc-function.git)
- [工作流项目（jecloud-pc-workflow）](https://gitee.com/ketr/jecloud-pc-workflow.git)
- [RBAC项目（jecloud-pc-rbac）](https://gitee.com/ketr/jecloud-pc-rbac.git)
- [菜单项目（jecloud-pc-menu）](https://gitee.com/ketr/jecloud-pc-menu.git)
- [数据源项目（jecloud-pc-datasource）](https://gitee.com/ketr/jecloud-pc-datasource.git)
- [系统设置项目（jecloud-pc-settings）](https://gitee.com/ketr/jecloud-pc-settings.git)
- [登录项目（jecloud-pc-login）](https://gitee.com/ketr/jecloud-pc-login.git)
- [展板项目（jecloud-pc-boards）](https://gitee.com/ketr/jecloud-pc-boards.git)
## 十、中间件项目
- [认证中间件（jecloud-auth）](https://gitee.com/ketr/jecloud-auth.git)
- [工作流中间件（jecloud-bpm）](https://gitee.com/ketr/jecloud-bpm.git)
- [JEIbatis（je-ibatis）](https://gitee.com/ketr/je-ibatis.git)
- [mxgraph封装（jecloud-mxgraph）](https://gitee.com/ketr/jecloud-mxgraph.git)
## 十一、项目关系图

![项目关系图](docs/images/system/项目关系图.jpg)

## 十二、开源协议
- [MIT](./LICENSE)
- [平台证书补充协议](./SUPPLEMENTAL_LICENSE.md)
## 十三、付费服务
1、开源版（免费）

2、私有证书（默认展示“技术支持：凯特伟业” ，可使用付费证书替换）

3、专家服务（非强制性服务，可按需订阅）
- 基于docker-compose安装。
- 基于Linux传统安装。
- 基于源码，搭建git、maven、Jenkins全流水线环境搭建。（Linux）。
- 平台升级服务（官方专家操作）。
- 基于K8S安装。（Linux）
- 现场平台使用培训（平台高级培训老师）。
- 现场平台源码培训（平台前后端2位架构师）。
- 私人定制培训（按培训课程内容报价）。
- VIP专属群服务（5*8小时专人在线）。
- 平台功能定制开发（按需求内容报价）。
    
4、增加套件（联系官方，了解更多）
## 十四、联系我们
- 公  司：北京凯特伟业科技有限公司

- 联系人：云凤程
- 电  话：18610941078（微信同号）
- 公众号：

![公众号](docs/images/orcode.png)
## 十五、项目截图
1、微服务架构图

![微服务架构图](docs/images/system/01%20微服务架构图.png)

2、 平台功能架构图

![平台功能架构图](docs/images/system/02%20平台功能架构图.png)

3、资源表引擎

![资源表引擎](docs/images/system/03%20资源表引擎.png)


4、列表规划器

![列表规划器](docs/images/system/04%20列表规划器.png)

5、标准功能列表

![标准功能列表](docs/images/system/05%20标准功能列表.png)

6、列锁定+复杂表头列表

![列锁定+复杂表头列表](docs/images/system/06%20列锁定+复杂表头列表.png)

7、表单规划器

![表单规划器](docs/images/system/07%20表单规划器.png)

8、标准表单

![标准表单](docs/images/system/08%20标准表单.png)

9、主从表单

![主从表单](docs/images/system/09%20主从表单.png)

10、工作流规划器

![工作流规划器](docs/images/system/10%20工作流规划器.png)