## 问题
Hype-V中创建的虚拟机，只分配了系统盘，C盘，想安装软件，但是不想放C盘，所以想给虚拟机添加一块逻辑盘，D盘。

## 测试环境
- Windows 10 Enterprise 1903
- Hype-V Manager 10.0.18362.1

## 步骤

1. 先把虚拟机关机（shut down）
2. 打开Hype-V，选择要扩展逻辑盘的虚拟机，Actions里选择Edit Disk...
3. 根据向导，选择你的虚拟硬盘文件存放位置
4. 选择下一步后，选择Expand
5. 选择下一步后，根据实际磁盘空间，设置新的大小
6. 下一步后，完成
7. 打开虚拟机
8. 在搜索框敲diskmgmt
9. 选择Create and format hard disk partitions
10. 你会发现多了一块没有格式化的分区
11. 这块就可以用做你的D盘了
