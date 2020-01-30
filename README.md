# [kkpay](https://kkpay.goodqp.com/) 开源个人收款码免签系统

## 服务端和监控端全部开源，自建支付平台，安全更放心，二开更方便
## 没有中间商赚差价，买家扫多少，商家收多少

### 一、系统特色
#### 1.1 支持

* 支付宝个人收款的推送通知
* 支付宝商家二维码的收款推送通知
* 支付宝店员通绑定的店员账号收款的推送通知
* 微信二维码收款推送通知
* 微信店员收款推送通知
* 微信收款商业版收款推送通知
* 微信收款商业版店员到账收款通知

#### 1.2 不用

* 不用 注册微信商家
* 不用 注册支付宝商家
* 不用 营业执照

#### 1.3 自动

* 自动 监听收款
* 自动 处理支付结果

### 二、系统原理
- 原理说明

`第一步：用户在你的网站点击购买 -> 向你的kkpay_server 发起支付订单 ->`

`第二步：kkpay_server 返回你的二维码 -> 用户扫码支付 -> 钱到你的微信/支付宝 -> kkpay_app 监听到钱支付成功 ->`

`第三步：kkpay_app 告诉kkpay_server 这个支付成功的消息 -> kkpay_server 把这个消息回调给你的网站(notify_url)`
### 三、搭建流程

#### 2.1 获取源码 ----> [kkpay](https://kkpay.goodqp.com/)

#### 2.2 购买服务器

#### 2.3 购买域名

#### 2.4 根据配套文档教程搭建

#### 2.5 配置 收款码 等信息

#### 2.6 搭建完成

### 四、当前市面上所谓的‘自动监听’

- 原生支付宝，微信支付

    - >支付宝微信只服务于有营业执照、个体工商户的商户。截止目前（2019-01-01）无法以个人身份（或以个人为主体）直接申请API。
      >结论：不可行结论：不可行

- 关联企业支付宝账号

    - >即新建企业账户，然后采用已经实名认证了的企业账户关联该账户，用其实名主体完成新账户的实名认证。一系列操作完成后，新的账户具有和企业账户一样的资质可以申请API。

      >结论：如果条件允许，推荐此方案

- 聚合支付工具，Ping++等

    - >就是个第四方聚合支付工具，简化了接入开发流程而已，个人开发者仍然需要去申请所需接口的使用权限。

      > 结论：不可行

- 第四方聚合支付

    - >支付资金进入官方账号，自己再进行提现操作。需要开通域名，提现手续费较高，支付页面不支持自定义。另外，对于此种类型的聚合支付平台，隐藏着极高的跑路风险。

      >结论：不推荐

- 有赞

    - >通过有赞微商城支付接口收款。

      >结论：不推荐，需手动提现，不免费，费用6800/年起，一旦风控资金很难取出。

- 利用拼多多店铺、淘宝代付功能等

    - >结论：不推荐，可能随时被风控。

- 挂机监听软件，PaysApi、绿点支付等

    - >采用挂机监听的策略

      >结论：第三方平台，存在安全隐患，成本高，费率高，不免费

- 其他基于Xposed挂机监听软件

    - >基于virtual xposed hook相关技术，可自动生成任意备注金额收款码 参考抢红包外挂

      >结论：成本高，配置麻烦，需24小时挂台安卓手机，量大易触发风控、不免费，黑产适用

- Payjs （疑使用[微信小微商户](https://pay.weixin.qq.com/index.php/core/affiliate/micro_intro)）

    - >结论：仅支持微信、不免费、使用官方接口收取代开费用

- 国外支付，PayPal、Strip：不可用

#### 某些安全性很低，容易被封号，一旦被查，直接冻结金额！

**[ kkpay ](https://kkpay.goodqp.com/) `完全打破现有市场，服务端和监控端全部开源，让您自建支付平台，安全更放心，二开更方便。直接收款到个人的账户，没有中间商赚差价，买家扫多少，商家收多少,永久安全正规！`**

### 五、部署补充

* 参考源码源码安装文档。

* 融合 宝塔 面板更具效率，小白不会编程也会部署！

* 支持同时并发多个收款码支付！


### 六、预览效果

- 电脑端进入→ [在线demo](https://kkpay.goodqp.com/)
