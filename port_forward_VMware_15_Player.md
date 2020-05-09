# 设置 VMware Workstation 15 Player 端口转发
Setup port forward for VMware Workstation 15 Player

## 版本信息
* VMware-player-15.5.2-15785246
* vmnetcfg_15_5_1

## 方法
1. 将 vmnetcfg_15_5_1 解压并放置在 Player 安装目录 （C:\Program Files (x86)\VMware\VMware Player）
2. Player 进入虚拟机，Terminal， ifconfig， 记下虚拟机 ip
3. 打开刚解压完毕的 vmnetcfg.exe ， 点击右下角“更改设置”，选择上面唯一的NAT模式（通常是VMnet8），进入下面的NAT设置
4. 添加，主机端口和虚拟机端口均为4567，虚拟机ip地址用步骤2的ip地址，确定，应用
5. 如果ros已经在运行，重启ros