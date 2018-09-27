## laravel shop 购物商城项目 
本项目基于Laravel-china教程5《电商实战》，在此基础上进行扩展开发

## 扩展内容
1、用户模块
- 支持手机号注册、登录、找回密码（腾讯云验证码和短信发送）
- 提供微信网页授权登录、小程序登录、注册API支持


2、商品模块
- 扩展商品SKU为多维度。（在原本的products(商品表)+product_skus（SKU表）基础上增加商品属性表（product_attributes）和商品属性值表（attributes）,以属性值表ID字符串构成SKU)
- 增加商品分类模块，无限级分类。
- 增加商品轮播图管理（PC页面上无轮播图条目（一直没找到好看的页面哈哈哈））

3、API模块
- 使用DingoApi进行API开发，为小程序提供完整接口支持

## 本项目模块概述
1、用户模块
- 登录注册（找回密码）
- 商品收藏
- 收货地址
- 查看订单
- 购物流程：选择商品-》下单-》付款-》确认收货-》发表评价、申请退款

2、商品模块
- 商品分类
- 后台添加商品、设置商品属性、设置商品库存
- 前台展示显示商品列表，提供简单筛选

3、订单模块
- 用户订单页面显示已经提交过的订单，管理员后台显示已支付订单
- 后台输入物流信息，进行发货操作

5、优惠券模块
- 多种优惠方案（满减、打折）
- 后台设置优惠券，前台提供优惠券使用接口

6、支付模块
- PC端前台提供微信/支付宝扫码支付
- 小程序端提供微信支付
- 前台提供用户申请退款接口、后台审核是否同意退款

## 安装方法
- 1、git clone或者下载解压到本地
- 2、将public设置为网站根目录
- 3、composer install
- 4、npm install
- 5、npm run production
- 6、配置env数据库，运行php artisan migrate
- 7、导入后台管理数据，admin.sql (导入后http://域名/admin 进入后台登录，管理员账号为admin 密码为 admin)
- 提示:APP_DEBUG为true时，注册时的短信验证码不会发送，固定为1234



