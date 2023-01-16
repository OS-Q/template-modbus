# [template-modbus](https://github.com/OS-Q/template-modbus)

[template-modbus](https://github.com/OS-Q/template-modbus) 以量产为主的标准模板，基于Modbus RTU协议通信，IO输入输出

## 关键参数

* 串口通信支持波特率2400/4800/9600/19200/38400/57600/115200
* 至少一个数字输出IO，切换频率≥ 1KHz
* 至少一个数字输入IO，采样频率≥ 1KHz


## 适配信息

满足模型的基本功能IO需要至少4个，在模型基础上构建，适配的MCU封装范围可选SON8到TSSOP20等一些列低成本  [L1R1控制器](https://doc.soc.xin/list/low)

| [chips](https://github.com/OS-Q/chips) | [templates](https://github.com/OS-Q/qio) | [applications](https://github.com/OS-Q/applications) | [libraries](https://github.com/OS-Q/libraries) | [boards](https://github.com/OS-Q/boards) |
| ------- | ------- | ------ | --------- | --------- |
| [STM32G031](https://doc.soc.xin/STM32G031) |  √  |  √  |  √  |  √  |
| [MM32F031](https://doc.soc.xin/mindmotion/MM32F031) |  √  |  √  |  √  |  √  |

