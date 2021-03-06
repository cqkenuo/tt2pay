### 项目介绍  
- 项目说明： 支持个人网站、安卓App、微信公众号、Pc软件收款的接入，所有的资金都会实时到账您的支付宝/微信余额中，支付宝无需上传收款二维码，支持H5唤醒支付，支持回调通知、支持补单、后台功能简单。

- 特点：支付回调通知，0手续费实时到账（不经过任何第三方，直接到账微信/支付宝余额），全部服务端源代码，支持php/java/python等语言直接接入(请使用Api版本傻瓜式接入)，监听方式非xp框架HOOK的方式，独立App监听安全无风险，无需root权限。

- 实现原理： 当收到支付宝、微信、实时收款信息，客户端会实时通知服务器收款金额和方式，服务器收到有效期订单金额后处理订单状态，使用随机减免的方式区分订单（5分钟订单有效期内有相同金额的订单会随机减免0.01 - 0.10的方式用来区分订单。

### 支持的通道：除特别说明外均可自动回调 

- 1.支付宝唤醒支付（转账码）

- 2.支付宝扫码（个码）

- 3.微信扫码（收款码）

- 4.微信转手机号（无自动回调）

- 5.微信转卡
 
- 6.银行卡转账网关

- 7.支付宝转卡 

- 8.云闪付

- 9.聚合码（如钱方好近）

- 10.银行码（如农信易扫） 

- 11.持续更新中……


### 在线demo
- 本项目演示地址： [点此测试](http://ttpay.goodqp.com/)

### 开始部署
- 本项目源码下载： [点此下载](http://ttpay.goodqp.com/)

### 更新日志：

V1.0.1  更新日期2019/04/12

Ø 添加新订单声音提醒

**<font color="#ff0000" style="margin: 0px auto;">Ø重要更新： 添加同城优先匹配功能</font>**

Ø 优化支付引导页面

Ø 重要更新：优化码商代理和商户代理，无限层

V1.0.2  更新日期2019/05/02

**<font color="#ff0000" style="margin: 0px auto;">Ø 重要更新：支付界面添加我已支付按键，点击后锁仓，直至订单完成或取消</font>**

Ø 新增订单匹配码商功能，用于支付金额不一致进行补单操作

Ø 后台可设置码商提现手续费

Ø 修复其他已知BUG

V1.0.3  更新日期2019/07/23

<font color="#ff0000" style="margin: 0px auto;">**Ø重要更新： 订单在未超时或确认支付前不匹配同一个码商相同金额**</font>

Ø 后台订单统计功能：分待支付，已提交，已超时，已取消，已完成状态，统计更直观

Ø 优化前台订单页面，显示效果

Ø 修复其他已知BUG

V1.0.4  更新日期2019/08/20

**<font color="#ff0000" style="margin: 0px auto;">Ø 重要更新：增加自动确认，支持支付宝，微信，钱方好近，云闪付的自动回调</font>**

Ø 增加代理一键上下线功能，只有允许的情况，代理下面的所有会员才可上线

Ø 增加识别无效码功能，连续5笔发起没支付的自动下线15分钟，并提示码商：该收款方式疑似异常，请确认正常后再上线（数字后台可调）

V2.0.5  更新日期2019/09/28

Ø 后台订单界面增加收款支付宝信息，用户删除后仍可显示，避免码商收款恶意不确认

Ø 显示每个码的调用次数，成功支付次数

**<font color="#ff0000" style="margin: 0px auto;">Ø 重要更新：优付二维码上传，用户支付体验，简化程序流程</font>**

Ø 码商删除收款码后，在垃圾站里还会保存一段时间

V2.1.6 更新日期2019/10/12

**<font color="#ff0000" style="margin: 0px auto;">Ø重要更新：增加回款模式，码商免保障金收一笔回一笔</font>**

Ø增加码商信任模式，仅需代理充值保障金，码商免保障金收款

Ø修复界面兼容性

V2.1.7更新日期2019/11/03

**<font color="#ff0000" style="margin: 0px auto;">Ø优化手机监听功能，一台安卓手机可监听4个支付宝和51个微信</font>**

Ø支持支付宝H5，微信转手机号，微信转卡

Ø修复其他已知BUG

V3.1.8更新日期2019/11/08

**<font color="#ff0000" style="margin: 0px auto;">Ø重要更新：集成手机监控和主程序，码商只要安装一个APP</font>**

Ø调试APP适配虚拟安卓系统，针对红手指平台调试

Ø优化H5体验，跳转支付宝自动复制金额

V4.0更新日期2019/12/10

**<font color="#ff0000" style="margin: 0px auto;">Ø重要更新：添加授信额度，完美解决授信问题</font>**

Ø加入RSA加密传输，数据传输更安全

Ø增加可给特定商户指定码商或码商代理来收款

Ø更新socket框架，连接数从2048个提升到无限，速度提升20%，有效提高并发量

V4.1更新日期2019/12/10

**<font color="#ff0000" style="margin: 0px auto;">Ø重要更新：增加支付宝转账模式带金额（风控过的支付宝也可以用）</font>**

Ø增加回款导入银行收款账单批量确认

Ø优化信任模式，授信额度不可提现，返佣可直接提现

V5.0更新日期2019/12/31

<font color="#ff0000" style="margin: 0px auto;">**Ø重要更新：增加短信和银行a-p-p监听**</font>

Ø结合监听更新，增加银行收款码，聚合收款码通道及自动回调，如农信易扫

Ø完善银行卡转账，支付宝转卡，微信转卡的自动回调

Ø后台新增清除数据，可按照日期选择性清除冗余数据

Ø修复其他已经BUG
