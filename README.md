# 基于SpringBoot+Vue的民宿管理系统

![Spring Boot](https://img.shields.io/badge/-Spring%20Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white) ![Vue3](https://img.shields.io/badge/-Vue3-grey?style=flat-square) ![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![MyBatis](https://img.shields.io/badge/-MyBatis-000000?style=flat-square&logo=mybatis&logoColor=white) 

## 项目介绍

本系统是一款面向短途游与周末度假场景的民宿在线预订与运营平台，针对线下微信询价撞期、房态与订单散落在表格、评价游记难沉淀、优惠券与退款难追溯等问题，把房源检索、分时预订支付、入住核销、评价晒单、游记互动、卡券收藏，以及管理端房型设施维护、订单退款审核与经营看板整合到同一套前后端分离工程中。

系统采用 SpringBoot + Vue 架构，区分普通房客与系统管理员：房客端完成找房筛选、下单支付、领券收藏、游记社区与个人中心；管理端维护分类设施与房源上下架、处理预订核销与退款、审核评价游记、配置优惠券与公告，并在 ECharts 看板查看订单与营收趋势。预订扣减库存、未支付可取消回滚，核销码一次有效，适合作为毕设、课设与民宿电商学习参考。

## 主要功能模块

- **用户认证与角色分流**：房客与管理员统一登录注册，JWT 鉴权；登录后按角色进入门户首页或管理看板，/admin 路由与接口双重隔离
- **门户首页大厅**：轮播公告、精选房源推荐与快捷入口，导流至探索、领券与游记
- **房源探索与筛选**：按分类、价格、人数、关键词筛选房源列表，支持收藏
- **房源详情与预订**：查看图文介绍、设施清单与可订日历，选择入住离店日期提交订单
- **支付结算与核销**：收银台支付后生成核销码；管理端支持入住核销，保证一次有效
- **领券中心与优惠**：浏览可领优惠券并下单抵扣，未支付取消时回滚券权益与库存
- **游记社区与公告**：发布/浏览游记互动，查阅运营公告详情
- **个人中心**：资料与密码维护，我的订单、收藏、优惠券集中管理
- **经营数据看板**：订单量、营收与房源占比等 KPI，ECharts 趋势图辅助运营
- **房源主数据中台**：房型分类、设施配置、房源上下架与库存维护
- **履约与审核**：预订订单发货式核销、退款审核、评价/游记审核、用户启停与公告发布
- **论文与 UML 概览**：配套论文设计实现页拼图与 UML 图列表，便于答辩材料对照

## 技术架构

- **后端**：Spring Boot + MyBatis-Plus + JWT + Lombok
- **前端**：Vue 3 + TypeScript + Vue Router + Pinia + Element Plus + Vite + ECharts
- **数据库**：MySQL

<!-- screenshots-start -->
## 系统截图

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/homestaymanage/%E7%99%BB%E5%BD%95%E9%A1%B5%E9%9D%A2.png" alt="登录页面" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/homestaymanage/%E7%94%A8%E6%88%B7%E9%A6%96%E9%A1%B5.png" alt="用户首页" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/homestaymanage/%E6%88%BF%E6%BA%90%E6%8E%A2%E7%B4%A2.png" alt="房源探索" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/homestaymanage/%E6%88%BF%E6%BA%90%E8%AF%A6%E6%83%85.png" alt="房源详情" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/homestaymanage/%E9%A2%84%E8%AE%A2%E8%AE%A2%E5%8D%95.png" alt="预订订单" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/homestaymanage/%E6%B8%B8%E8%AE%B0%E5%88%86%E4%BA%AB.png" alt="游记分享" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/homestaymanage/%E7%AE%A1%E7%90%86%E5%91%98%E4%BB%AA%E8%A1%A8%E7%9B%98.png" alt="管理员仪表盘" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/homestaymanage/%E6%88%BF%E6%BA%90%E7%AE%A1%E7%90%86.png" alt="房源管理" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/homestaymanage/%E8%AE%BA%E6%96%87%E5%9B%BE1.png" alt="论文图1" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/homestaymanage/%E8%AE%BA%E6%96%87%E5%9B%BE2.png" alt="论文图2" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/homestaymanage/UML%E5%9B%BE%E5%88%97%E8%A1%A8.png" alt="UML图列表" width="600" />

<!-- screenshots-end -->

## 接毕业设计和论文

### 作者微信：vvsgxmn  (支持修改、 部署调试、 支持代做毕设)

### 接网站建设、小程序

### 选题+开题报告+任务书+程序定制+安装调试+论文+答辩ppt 都可以做

### 购买地址：[https://www.vvxx.love](https://www.vvxx.love)（vv毕设网）

### 支持 **一键生成 UML 图**：上传项目压缩包即可自动产出功能模块图、用例图、流程图、E-R 图、时序图等全套毕设图表。

### 提供 **免费配套软件下载 + 安装说明 + 部署教程**

![vv毕设网 - 一键画图](https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/uml-draw.png)

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/image-20260825133349317.png" alt="image-20260825133349317" />

⚠️ Bug添加微信**免费修复**，免费修复。其他平台的私信一律不管（微信方便发送文件）
