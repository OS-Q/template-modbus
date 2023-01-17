.. _modbus_tcp:

Template-Modbus
-------------------

.. image:: https://github.com/OS-Q/template-modbus/workflows/sdk/badge.svg
    :target: https://github.com/OS-Q/template-modbus/actions

本模板基于Modbus RTU/TCP双协议栈，主从机双模式。

Modbus TCP 通信主站为client，主动建立连接；从站为server端，等待连接。IANA（Internet Assigned Numbers Authority，互联网编号分配管理机构）给Modbus协议赋予TCP端口号为502，这是目前在仪表与自动化行业中唯一分配到的端口号。

ModbusTCP的数据帧可分为两部分：MBAP+PDU。简单的理解，就是去掉了modbus协议本身的CRC校验，增加了MBAP报文头。

MBAP为报文头，长度为7字节，组成如下：

* 事务元标识符（2个字节）：用于事务处理配对。在响应中，MODBUS服务器复制请求的事务处理标识符。这里在以太网传输中存在一个问题，就是先发后至，我们可以利用这个事务处理标识符做一个TCP序列号，来防止这种情况所造成的数据收发错乱（这里我们先不讨论这种情况，这个事务处理标识符我们统一使用0x00，0x01）
* 协议标识符（2个字节）：modbus协议标识符为0x00，0x00
* 长度（2个字节）：长度域是下一个域的字节数，包括单元标识符和数据域。
* 单元标识符（1个字节）：该设备的编号。（可以使用PLC的IP地址标识）。


.. contents::
    :local:
    :depth: 1

.. _modbus_app:

applications
~~~~~~~~~~~~~~~~~


.. _modbus_std:

standard
~~~~~~~~~~~~~~~~~

* 双串口，至少一路支持RS485通信
* 串口波特率2400/4800/9600/19200/38400/57600/115200
* 至少一个数字输出IO，切换频率≥ 1KHz
* 至少一个数字输入IO，采样频率≥ 1KHz


.. _modbus_lib:

libraries
~~~~~~~~~~~~~~~~~

.. _modbus_if:

interface
~~~~~~~~~~~~~~~~~

.. _modbus_hw:

hardware
~~~~~~~~~~~~~~~~~



