---
title: "Simulating Mechanical Control System With Matlab"
date: 2017-01-29T20:50:08-05:00
draft: true
toc: false
images:
tags:
  - simulink
---

仿真对于控制方向的研究和开发有多重要就不用强调了。不管是写paper还是开会做presentation，有个看起来很cool的仿真都是有帮助的。如果能快速的搭建仿真，还能帮着在研究的前期快速验证idea是否可行。

然而进行仿真总不是简单的事情。一方面可能要进行繁琐的公式推导和计算（而且特别容易出错，错了还不容易找出问题）。另一方面又需要写大量的程序（特别是要有视觉效果的时候）。今天我来介绍一种工作流程来绕开这两个麻烦，它特别适用于机械系统的控制和仿真。这里需要用到的是Simscape multibody (以前叫Simmechanics) 和 Simulink Control Design工具箱。

为了简单起见，起到抛砖引玉的作用，我们就制作一个最简单的机械系统 -- 倒立摆 -- 的仿真。特别注明我用的是MATLAB R2015b. 其它版本的MATLAB可能略有差异。

首先，打开一个新的Simulink模型，里面带有一些常用的Simmechanics模块。输入如下命令

>> smnew


你会看到两个弹出来的窗口。一个是空的模型，一个是Simmechanics的library.

我们现在来创建倒立摆的杆，为此，双击Solid模块，修改一下它的长宽高. 注意单位我用的是厘米。