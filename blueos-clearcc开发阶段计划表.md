# 操作系统开发计划
## 第一阶段改造：（让系统更符合预期）
1. 改造窗口样式与鼠标指针(已废弃)
2. 改造内存分配函数(已废弃)
3. 为命令行增加更多功能支持
## 第二阶段改造：（改进系统表层结构）
* 阶段涉及少量汇编语言
1. 改造任务调度算法，舍弃cpu级别的任务调度
2. 支持浮点部件的使用，将浮点部件加入任务调度控制
3. 增加磁盘读写能力
4. 加入中文字库支持
## 第三阶段改造：（改进系统底层结构）
* 阶段涉及大量汇编语言，处理器底层知识（需要另外的书籍或知识辅助）
1. 为系统开启分页内存管理（需要另外的书籍辅助或知识）
2. 改进系统启动流程，优化启动阶段
3. 增加apic中断控制器的支持，舍弃8259控制芯片（需要另外的书籍辅助或知识）
4. 增加多处理器（多核心）的支持（需要另外的书籍辅助或知识）
## 第四阶段改造：（最终改造使得这个系统成为自己的东西）
* 阶段涉及相关文档、代码的阅读
1. 支持64位模式（需要另外的书籍辅助或知识）
2. 增加处理器虚拟化技术支持，操作系统由虚拟环境启动（需要另外的书籍或知识辅助）
3. 改进系统结构，实现类unix的根目录结构文件体系
4. 移植tek压缩格式，自此操作系统将自带文件压缩功能（需要阅读相关文档和代码）
5. 系统关键部分汇编化以加速执行（此项在所有阶段都顺带执行）
6. 操作系统将由一个启动器（blue-bootstrap）启动
## 扩展阶段改造：（更多新特性的加入）
* 阶段涉及大量文档阅读和相关标准学习
1. 增加UEFI启动支持
2. 移植标准库<std>环境的支持
3. 增加对网卡的支持
4. 操作系统安全设计

#实际进度表
1. 2022-8-20 成功使用io-apic代替8259A