# SyncABCPrinter
提供两种顺序循环打印ABC各10的方法
方法1：利用acquire和release函数对初始permit的修改和阻塞效果实现
方法2：不断修改允许打印的threadId，不满足的线程进入循环等待，每次打印结束后唤醒所有等待的线程