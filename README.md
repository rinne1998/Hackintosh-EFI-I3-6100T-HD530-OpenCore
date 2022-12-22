# Hackintosh-EFI-I3-6100T-HD530-OpenCore

## 硬件
* CPU：Intel(R) Core(TM) i3-6100T CPU @ 3.20GHz
* iGPU：Intel HD Graphics 530
* 主板：ASUS H110M-K
* 硬盘：WD SN570 500G

## 系统
* macOS Big Sur 版本11.7.2（版号20G1020）


## 引导工具
* OpenCore 0.8.2

## 启用的内核拓展
* Apple ALC 1.7.3
* CPUFriend 1.2.6
* HibernationFixup 1.4.7
* Lilu 1.6.1
* RTCMemoryFixup 1.0.7
* RealtekRTL8111 2.4.2
* VirtualSMC 1.3.0
* VoodooPS2Controller 2.3.2
* VoodooTSCSync 1.5.0
* WhateverGreen 1.6.0

## 使用i3-6098P/HD510
只需将 DevicesProperties > PciRoot(0x0)/Pci(0x2,0x0) 中的选项做以下改动：
* AAPL,ig-platform-id : 00001B19 
* device-id : 02190000

**注意：当使用VGA接口连接显示器会黑屏，请使用DVI或者其他接口；此法虽然可以让核显工作，但使用Safari、Firefox等软件会Crash（能让核显驱动起来已经不容易了）**


## 无法工作
* 休眠
