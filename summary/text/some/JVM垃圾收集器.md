# JVM
## 垃圾收集算法
   * 标记-清除:
        * 优点:简单
        * 不足:1、标记和清除效率不高；2、容易产生碎片，内存不连续，分配大内存触发FULL GC
   * 复制算法
        * 优点:实现简单、运行高效
        * 缺点:所需内存翻倍 
   * 标记-整理
        * 优点:没有碎片，内存连续
        * 缺点:内存对象一端移动，耗时一点 
## 新生代收集器
  * Serial收集器
        * 单线程、复制算法 
  * ParNews收集器
        * 多线程并行、复制算法；Serial的多线程版本
  * Parallel Scanenge收集器
        * 多线程并行、复制算法；更关注吞吐量      
  * G1收集器
        * 多线程并发、标记整理算法 
## 老年代收集器
  * CMS收集器
        * 多线程并发、标记清除算法 
  * Serial Old收集器
        * 单线程、标记整理算法
  * Parallel Old收集器
        * 多线程并行、标记整理算法
  * G1收集器
        * 多线程并发、标记整理算法 
## 名词
* 引用计数
* 可达性
* GCRoots
* SafePoint
* OopMap
* 并行
* 并发 