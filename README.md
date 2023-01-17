# [template-modbus](https://github.com/OS-Q/template-modbus)

[template-modbus](https://github.com/OS-Q/template-modbus) 以量产为主的标准模板，基于Modbus RTU协议通信，IO输入输出

## 关键参数

* 串口通信支持波特率2400/4800/9600/19200/38400/57600/115200
* 至少一个数字输出IO，切换频率≥ 1KHz
* 至少一个数字输入IO，采样频率≥ 1KHz

## 底层框架

标准模板不关心底层的实现机制，只需要满足特定的性能基线，使用的开发框架和SDK都是由硬件层实现和打包。



## 适配硬件

| chips | [![Build Status](https://github.com/OS-Q/template-modbus/workflows/sdk/badge.svg)](https://github.com/OS-Q/template-modbus/actions/workflows/sdk.yml) | [![Build Status](https://github.com/OS-Q/template-modbus/workflows/arduino/badge.svg)](https://github.com/OS-Q/template-modbus/actions/workflows/arduino.yml) | [![Build Status](https://github.com/OS-Q/template-modbus/workflows/cmsis/badge.svg)](https://github.com/OS-Q/template-modbus/actions/workflows/cmsis.yml) | [![Build Status](https://github.com/OS-Q/template-modbus/workflows/cmsis/badge.svg)](https://github.com/OS-Q/template-modbus/actions/workflows/cmsis.yml) | [![Build Status](https://github.com/OS-Q/template-modbus/workflows/libopencm3/badge.svg)](https://github.com/OS-Q/template-modbus/actions/workflows/libopencm3.yml) |
| ------- | ------- | ------ | --------- | --------- | --------- |
| [STM32G031](https://doc.soc.xin/STM32G031) |  √  |  √  |  √  |  √  |  √  |
| [MM32F031](https://doc.soc.xin/mindmotion/MM32F031) |    |    |    |     |


