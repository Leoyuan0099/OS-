# OS-
操作系统复习笔记


作业调度算法：
  1.先来先服务：
    FCFS：按照作业(JOB)的 等待时间 处理。 等待时间越短，越先处理
    
    
  2.短作业优先：
    SJF：按照 作业的 运行时间 来处理。运行时间越短，越先处理
    
    
  3.高响应比优先：
    HRRN：既考虑 运行时间 又考虑 等待时间
     优先权Rp= 等待时间 + 运行时间 / 运行时间  = 响应时间 / 运行时间

    
交换：
•	交换操作系统将一个进程的整个地址空间的内容保存到外存中（换出swap out），而将外存中的某个进程的地址空间读入到内存中（换入swap in）。换入换出内容的大小为整个程序的地址空间。

•	粒度：一个程序。

•	交换实现的几个问题：
  o	何时需要发生交换？只有当内存空间不够或有不够的危险时换出
  
  o	交换区的大小：
  
  o	程序换入时的重定位：换出后再换入的内存位置一定要在原来的位置上吗？不是，最好采用动态地址映射的方法。
  
•	交换和覆盖的区别

  o	粒度：交换在以程序为单位的。覆盖在程序之内。
  
