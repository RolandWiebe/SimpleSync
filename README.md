# SimpleSync
Simple synchronization protocol between two microcontrollers using FreeRTOS

It is designed to synchonize single variables as also complex structures through an pheripheral interface to another microcontroller. It is working in Master-Slave configuration and the master can be configured to synchronize the configured items cyclic or just once. The data is directly put to the linked variable, so there is no need for additional activities. Just configure it and have your data synchornized on both controllers. Optionally a callback function can be set in Master and Slave to react on the event of data update. 

SimpleSync relies on FreeRTOS for creation of Task, Queues and Events. For mor information see www.FreeRTOS.org.

SimpleSync is designed to be portable to use it on different microcontrollers and also different pheripherals. The current ports include the following controllers and pheripherals:
- STM32F030
  - USART
- STM32F373
  - USART

More ST Cortex-M controllers will follow but if you find this code useful, share your port and I will include it here.
