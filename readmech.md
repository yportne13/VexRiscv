以下配置的结果为1.44 DMIPS / MHz：
5级：F-> D-> E-> M-> WB。
单周期ADD / SUB /按位/移位ALU。
在E阶段完成分支/跳转。
WB阶段将绕过内存加载值（结果延迟）。
在M阶段绕过33个循环分割（结果较晚）。
在WB阶段进行旁路的单周期乘法（结果较晚）。
动态分支预测是在F阶段使用直接映射的目标缓冲区高速缓存完成的（对正确的预测没有损失）。
请注意，最近，增加了删除Fetch / Memory / WriteBack阶段的功能，以减少CPU的面积，最终为较小的配置提供了较小的CPU和更好的DMIPS / Mhz。
 依存关系