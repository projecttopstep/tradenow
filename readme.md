## **tradenow模拟交易平台**

tradenow是兼容CTP接口的模拟交易平台，一定程度上可替代simnow等模拟平台进行功能测试。 CTP程序无需修改代码也无需重新编译，只需在这里下载与CTP API版本号一致的交易dll，覆盖掉自己的即可，行情dll不用改，行情的接入地址可使用各期货公司的实盘地址。

暂不支持行权、组合等交易指令。

采用做市方式撮合成交，即高于叫卖价的多单立即成交，低于叫买价的空单立即成交，否则挂在队列中等行情符合条件的时候成交。

### **交易前置地址：**

- tcp://121.36.146.182:20002

### **行情前置地址：** 随便找的几个实盘地址，自己可以替换成其它的

- tcp://180.169.112.54:42213
- tcp://140.207.168.9:42213
- tcp://180.168.212.75:41313
- tcp://27.115.78.155:41313
- tcp://180.168.102.233:41168
- tcp://112.64.143.220:41168

### **用户：** 密码均为123456，初始资金为10000000

- 90001
- 90002
- 90003
- 90004
- 90005
- 90006

### **有其它需要的你懂的：**

99114024

### **特别说明：**

AuthCode、AppID认证信息任意填，不作校验

Broker任意填，填什么就回什么

<u>tradenow行情前置地址：tcp://121.36.146.182:20004，虽然也可以从tradenow接收实时行情，但是不建议这么做，除非玩TEST等自建合约，否则建议直接使用CTP数据源。从tradenow接收行情，同交易一样需要更换行情dll。</u>

**本平台为个人自建平台，希望大家手下留情，不要给太大的压力。**

<u>*本模拟平台没有像simnow那样严格遵循各交易所规则，如：不计持仓明细，因此平仓不存在先开先平等规则，只是对总持仓进行处理。如有较高测试要求的请连simnow或联系期货公司。*</u>
<u>*本模拟平台不对模拟结果作任何保证，依据本平台测试结果进行实盘交易的后果完全由使用者自己承担。*</u>
