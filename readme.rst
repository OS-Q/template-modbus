
Modbus-RTU Poll
-------------------

基于Modbus-RTU Poll & Slave 实现数字IO控制

.. _modbus_app:

applications
~~~~~~~~~~~~~~~~~

.. _modbus_lib:

libraries
~~~~~~~~~~~~~~~~~


Standard
-----------------

* 双串口，至少一路支持RS485通信
* 串口波特率2400/4800/9600/19200/38400/57600/115200
* 至少一个数字输出IO，切换频率≥ 1KHz
* 至少一个数字输入IO，采样频率≥ 1KHz

.. _modbus_inf:

interface
~~~~~~~~~~~~~~~~~

output
~~~~~~~~~~~~~~~~~

input
~~~~~~~~~~~~~~~~~


Hardware
-----------------

满足模型的基本功能IO需要至少4个，在模型基础上构建，适配的MCU封装范围可选SON8到TSSOP20等一些列低成本 `L1R1控制器 <https://doc.soc.xin>`_


.. list-table::
    :header-rows:  1

    * - :ref:`modbus_bsp`
      - :ref:`modbus_app`
      - :ref:`modbus_lib`
      - :ref:`modbus_inf`
      - `chips <https://github.com/OS-Q/chips>`_
    * - E22
      - √
      - √
      - 4
      - `STM32G031 <https://doc.soc.xin/STM32G031>`_
    * - E30
      - √
      - √
      - 12
      - `MM32F031 <https://doc.soc.xin/mindmotion/MM32F031>`_


.. _modbus_bsp:

boards
~~~~~~~~~~~~~~~~~


