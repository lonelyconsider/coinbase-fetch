# 用途
从交易所Coinbase Pro取汇率数据到数据仓库中，同时生成一张订单汇总分析表。

# API信息
文档网址：https://docs.pro.coinbase.com/
API限制：每秒3次API calls。
用到的接口：（调用官方提供的Python public client）
 get_product_ticker
 get_product_24hr_stats

# 环境
Python 3.7.3

# 依赖库
requests 
pymssql 
csv 
zimbrasmtp

# 备注
*zimbrasmtp是自定义的一个模块，用于当程序出错时，发送一封邮件到zimbrasmtp邮箱
*代码见SVN："004 DA关联\成果物\self-module"