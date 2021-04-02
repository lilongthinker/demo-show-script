## from cilium 
https://github.com/cilium/cilium/tree/2decaf1d7596f202f4c50ad85d0464141f781d14/contrib/shell

## 安装步骤
### 基础环境与能力演示

1. 基于linux环境（centos or aliyunlinux2）
2. 安装pv
```bash
yum -y install pv
```
3. git clone https://github.com/lilongthinker/demo-show-script.git
4. ./show_demo.sh

### 其他优化展示工具
1. jq https://stedolan.github.io/jq/manual/
2. jtab https://github.com/wlezzar/jtab
3. 阿里云命令行工具 arc

### 一些脚本演示
如下是demo里面的演示，可以一次打印，可以逐字打印，可以执行命令行，而命令行配合一些环境信息可以和jq/jtab/arc-cli 配合可以展现自动化的脚本展示

```bash
. ./bin/util.sh
desc "一次打印出来的提示信息"
desc_rate "逐字打印，类似手打效果"

run "date"
```