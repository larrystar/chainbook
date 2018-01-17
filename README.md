# 链书

## 简介

[链书](https://github.com/b3log/chainbook)（Chainbook）是 B3 社区的去中心化书籍共享服务，通过数字货币 [B3T](TBD) 实现共享激励与价值链。

## 使用流程

### 链书服务

* x：存书奖励 x 个 B3T，x 为定值 `100`
* y：分享书奖励 y 个 B3T，y 为定值 `20`
* 用户 A 存入 a 书：获取 x 个冻结的 B3T
* 用户 B 向 A 需求 a 书：
  1. B 提供真实地址和电话给 A
  2. A 快递 a 书给 B（A 支付快递费，使用小程序扫描录入快递单号）
  3. B 冻结 x 个 B3T 同时 A 解冻 x 个 B3T，并获得系统奖励的 y 个 B3T
  4. B 看完书后把 a 书进行分享
  5. 用户 C 向 B 索取 a 书，以此类推 1-5

### 站内交易

* B3T 在大多数情况下会在 B3 社区**站内**围绕具体服务场景进行交易流转
* 可以对 B3T 进行充值或提现
* 后续可能会引入[雷电网络](https://raiden.network)来支持实时交易

## 技术设计

### 

### 平台扩展性

* 后续对接 QTUM、NEO 等其他平台的能力
* 多平台发布令牌后的互交互性
* 去中心化的 B3log Coin 主网  

## 关于 B3T

B3T（B3log Token）是 B3 社区在以太坊上发行的 ERC20 令牌，可用于支付 B3 社区上提供的各类应用和服务，为 B3 社区在更大范围内的影响实现基础价值的统一。

B3T 的发行总量是 20 亿个，具体的分配比例如下：

* 3% 早期用户：按[黑客派](https://hacpai.com)注册时间、邀请数、积分余额、活跃度等历史数据进行计算并赠送排名前 5000 的用户
* 7% 团队持有：主要用于社区服务的开发和调试
* 10% 社区激励：用于奖励为社区发展创造价值的用户
* 80% 认购：目前暂不对外公开认购

## 冲币流程

1. 通过 DApp 把 ETH 兑换为对应平台的 B3T
   1. 打 ETH 到指定合约地址
   2. 该合约将 B3T 存入社区银行账户
2. 更新社区该用户 B3T 站内可用余额

1 ETH = 10000 B3T

* 35% 市场营销、地推及培训 
* 20% 产品设计和技术开发
* 20% 法务，例如各地政策咨询、专利申请） 
* 15% 社区服务基础，例如购书
* 10% 社区基金 

**目前暂不对外公开认购**。

## 提币流程

1. 输入钱包地址、提现金额及 gas
2. 人工审核（提现申请表）成功后，把 B3T 从社区银行账户转入用户输入的地址上
3. 更新社区该用户 B3T 站内可用余额

## 发展历程

* 2016 年萌生原始创意[疯狂的想法 C：书籍共享计划](https://hacpai.com/article/1483240295087)
* 2017 年通过微信小程序实现[客户端](https://github.com/b3log/symphony-weapp)并上线[书单计划](https://hacpai.com/tag/book_share)
* 2018 年通过区块链解决信任问题，实现书籍共享激励与价值链

## 开源协议

链书使用 GPLv3 作为开源授权协议，请尽量遵循，即使是在中国。

## 鸣谢

链书的诞生离不开以下项目：

* [Ethereum Project](https://www.ethereum.org)：运行智能合约的去中心化平台
* [OpenZeppelin](https://github.com/OpenZeppelin/zeppelin-solidity)：安全的智能合约基础库
