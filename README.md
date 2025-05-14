# proj322-Efficient-SMP-scheduler
# 基于小米澎湃OS(Vela OS)的高效SMP调度器

## 项目描述

关于Vela OS：Vela是小米公司基于开源实时操作系统NuttX打造的物联网嵌入式软件平台，Vela在各种物联网硬件平台上提供统一的软件服务，支持丰富的组件和易用的框架，用于打通碎片化的物联网应用场景。

在RTOS领域，SMP多核系统下的任务调度策略是操作系统优化的重要主题，任务调度作为OS中最常发生的几个事件，提升调度系统的效率能够有效地提升系统的整体运行效率。 POSIX规范中给出了多核调度器的实现要求。本项目的目标是基于NuttX已有的多核支持，实现一个符合POSIX规范的多核调度器，进一步优化NuttX在SMP系统上的工作效率。

## 预期目标

- 符合POSIX规范，支持FIFO、RR、Sporadic调度策略
- 对称式调度器（每个核心维护自己的task list）or 其他更优的无锁实现
- 适配K210板卡，并考虑多平台的可扩展（ARM、Xtensa）

## 难度：
中高

## 所属赛道
2025全国大学生操作系统比赛的“OS功能挑战”赛道

## 参考资料
- https://nuttx.apache.org

## 赛题分类
内核完善

## 项目导师
- 黄齐，Bytecode Alliance RC / WAMR TSC Member , huangqi3@xiaomi.com
- 小米公司Vela研发团队（含NuttX社区主要代码提交人）

## 对参赛队提供的支持
- NuttX的内核实现和动态加载器
- 针对NuttX实时操作系统业界最专业和权威的技术支持
