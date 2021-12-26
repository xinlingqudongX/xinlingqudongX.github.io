

##  商城系统表设计
#### 用户收货地址表
address_user是为了区分用户字段和其他表的用户字段

| 字段名称     | 类型         | 字段说明     |
| :----------- | :----------- | :----------- |
| address_id   | int          | 主键自增     |
| address_user | int          | 用户id       |
| name         | varchar(255) | 收货人姓名   |
| phone        | varchar(255) | 收货人电话   |
| province     | varchar(255) | 省份         |
| city         | varchar(255) | 城市         |
| area         | varchar(255) | 区域         |
| detail       | varchar(255) | 详细地址     |
| is_default   | int          | 是否默认地址 |
| create_time  | datetime     | 创建时间     |
| update_time  | datetime     | 更新时间     |
---
####    用户表
存放初始的用户信息
| 字段名称    | 类型         | 字段说明   |
| :---------- | :----------- | :--------- |
| user_id     | int          | 主键自增   |
| username    | varchar(255) | 用户名     |
| password    | varchar(255) | 密码       |
| phone       | varchar(255) | 电话       |
| email       | varchar(255) | 邮箱       |
| nickname    | varchar(255) | 昵称       |
| avatar      | varchar(255) | 头像       |
| is_login    | int          | 是否登录   |
| gender      | int          | 性别       |
| birthday    | varchar(255) | 生日       |
| age         | int          | 年龄       |
| alipay      | varchar(255) | 支付宝账号 |
| wx          | varchar(255) | 微信账号   |
| wx_openid   | varchar(355) | 微信openid |
| create_time | datetime     | 创建时间   |
| update_time | datetime     | 更新时间   |
| status      | int          | 状态       |

---
####    订单表
订单信息,包含支付信息，用户信息，商品信息
| 字段名称            | 类型         | 字段说明            |
| :------------------ | :----------- | :------------------ |
| order_id            | int          | 主键自增            |
| order_user          | int          | 用户id              |
| order_no            | varchar(255) | 订单号              |
| price               | money        | 订单价格            |
| currency            | varchar(255) | 订单币种            |
| pay_no              | varchar(255) | 支付单号            |
| pay_time            | datetime     | 支付时间            |
| pay_type            | int          | 支付方式            |
| pay_status          | int          | 支付状态            |
| pay_money           | money        | 支付金额            |
| shipping_type       | int          | 配送方式 自提或物流 |
| shipping_no         | varchar(255) | 物流单号            |
| shipping_start_time | datetime     | 发货时间            |
| shipping_status     | int          | 发货状态            |
| receipt_name        | varchar(255) | 收货人姓名          |
| receipt_phone       | varchar(255) | 收货人电话          |
| receipt_email       | varchar(255) | 收货人邮箱          |
| receipt_address     | varchar(255) | 收货人地址          |
| receipt_province    | varchar(255) | 收货人省份          |
| receipt_city        | varchar(255) | 收货人城市          |
| receipt_area        | varchar(255) | 收货人区域          |
| receipt_detail      | varchar(255) | 收货人详细地址      |
| receipt_time        | datetime     | 收货时间            |
| status              | int          | 订单状态            |
| goods_id            | int          | 商品id              |
| goods_sku           | int          | 商品sku             |
| goods_name          | varchar(255) | 商品名称            |
| goods_price         | money        | 商品价格            |
| goods_num           | int          | 商品数量            |
| goods_image         | varchar(255) | 商品图片            |
| goods_attr          | varchar(255) | 商品属性            |
| remark              | varchar(255) | 订单备注            |
| refund_status       | int          | 退款状态            |
| refund_time         | datetime     | 退款时间            |
| refund_money        | money        | 退款金额            |
| refund_reason       | varchar(255) | 退款原因            |
| refund_remark       | varchar(255) | 退款备注            |
| create_time         | datetime     | 创建时间            |
| update_time         | datetime     | 更新时间            |
| flag                | int          | 删除标志位          |
---

####    商品表
商品信息
| 字段名称     | 类型           | 字段说明         |
| :----------- | :------------- | :--------------- |
| goods_id     | int            | 主键自增         |
| title        | varchar(255)   | 商品标题         |
| keywords     | [varchar(255)] | 商品关键词       |
| dsec         | varchar(255)   | 商品描述         |
| category_id  | int            | 商品分类id       |
| brand_id     | int            | 商品品牌id       |
| main_img     | [varchar(255)] | 商品主图列表     |
| detail_img   | [varchar(255)] | 商品详情图列表   |
| sales        | int            | 商品销量         |
| shop_price   | money          | 商品价格         |
| market_price | money          | 商品市场价格     |
| shop_id      | int            | 商品所属店铺id   |
| supplier_id  | int            | 商品所属供应商id |
| price        | money          | 商品价格         |
| props        | {}             | 商品属性         |
| create_time  | datetime       | 创建时间         |
| update_time  | datetime       | 更新时间         |
| status       | int            | 商品状态         |
| flag         | int            | 删除标志位       |
---

####    商品分类表
| 字段名称    | 类型           | 字段说明   |
| :---------- | :------------- | :--------- |
| category_id | int            | 主键自增   |
| pid         | int            | 父级id     |
| name        | varchar(255)   | 分类名称   |
| sort        | int            | 排序       |
| status      | int            | 分类状态   |
| pids        | [varchar(255)] | 父级id列表 |
| create_time | datetime       | 创建时间   |
| update_time | datetime       | 更新时间   |
| flag        | int            | 删除标志位 |
---

####    商品SKU表
| 字段名称    | 类型         | 字段说明 |
| :---------- | :----------- | :------- |
| sku_id      | int          | 主键自增 |
| stock       | int          | 库存     |
| price       | money        | 价格     |
| sku_goods   | int          | 商品id   |
| img         | varchar(255) | 图片地址 |
| attr        | {}           | 属性对象 |
| create_time | datetime     | 创建时间 |
| update_time | datetime     | 更新时间 |
| flag        | int          | 标志位   |
---

####    用户购物车表
| 字段名称    | 类型     | 字段说明 |
| :---------- | :------- | :------- |
| cart_id     | int      | 主键自增 |
| cart_user   | int      | 用户id   |
| goods_id    | int      | 商品id   |
| goods_sku   | int      | 商品sku  |
| goods_num   | int      | 商品数量 |
| create_time | datetime | 创建时间 |
| update_time | datetime | 更新时间 |
---

####    用户收藏表
| 字段名称     | 类型     | 字段说明   |
| :----------- | :------- | :--------- |
| collect_id   | int      | 主键自增   |
| collect_user | int      | 用户id     |
| goods_id     | int      | 商品id     |
| create_time  | datetime | 创建时间   |
| update_time  | datetime | 更新时间   |
| flag         | int      | 删除标志位 |
| collect_type | int      | 收藏类型   |

####    用户足迹表
| 字段名称       | 类型     | 字段说明   |
| :------------- | :------- | :--------- |
| footprint_id   | int      | 主键自增   |
| footprint_user | int      | 用户id     |
| goods_id       | int      | 商品id     |
| create_time    | datetime | 创建时间   |
| update_time    | datetime | 更新时间   |
| flag           | int      | 删除标志位 |
---

####    活动海报表
| 字段名称    | 类型         | 字段说明   |
| :---------- | :----------- | :--------- |
| poster_id   | int          | 主键自增   |
| title       | varchar(255) | 海报标题   |
| img         | varchar(255) | 海报图片   |
| url         | varchar(255) | 海报链接   |
| type        | int          | 海报类型   |
| goods_id    | int          | 商品id     |
| start_time  | datetime     | 开始时间   |
| end_time    | datetime     | 结束时间   |
| status      | int          | 海报状态   |
| create_time | datetime     | 创建时间   |
| update_time | datetime     | 更新时间   |
| flag        | int          | 删除标志位 |
---

####    配置表
| 字段名称    | 类型         | 字段说明 |
| :---------- | :----------- | :------- |
| config_id   | int          | 主键自增 |
| name        | varchar(255) | 配置名称 |
| value       | varchar(255) | 配置值   |
| key_index   | varchar(255) | 配置键   |
| create_time | datetime     | 创建时间 |
| update_time | datetime     | 更新时间 |
| flag        | int          | 标志位   |
---

### 管理员表
| 字段名称         | 类型           | 字段说明   |
| :--------------- | :------------- | :--------- |
| admin_id         | int            | 主键自增   |
| username         | varchar(255)   | 用户名     |
| password         | varchar(255)   | 密码       |
| create_time      | datetime       | 创建时间   |
| update_time      | datetime       | 更新时间   |
| flag             | int            | 标志位     |
| status           | int            | 状态       |
| admin_role       | int            | 角色id     |
| admin_permission | [varchar(255)] | 权限id列表 |