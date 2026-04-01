## If you like this project, please give it a star ⭐  
A JavaScript userscript for automating repetitive tasks on websites
## 新增了 高级混合联赛SBC 挑战自动循环功能，可在挑战列表页一键启动自动处理流程。
<img width="746" height="490" alt="image" src="https://github.com/user-attachments/assets/d7d28b9d-fef6-4ae8-a151-fd765b7ec120" />


点击“开始循环”则开始自动循环完成SBC
自动流程为：

1. 自动寻找当前未完成挑战
2. 进入挑战
3. 执行 `SBC方案填充`
4. 执行 `一键替换所有假想球员`
5. 满足条件时自动提交
6. 返回并继续处理下一个挑战

## 优化一键填充的逻辑处理方式

现在的一键替换整体可以概括为：

1. 先循环替换假想球员。
2. 如果当前已替换上的真人球员提供的有效默契还不够，就尝试进行一次位置重排。
3. 一旦默契已达标，后续替换优先走省资源。
4. 当场上已经没有假想球员后，再做一次最终降分复检。
5. 如果降分后仍满足全部 SBC 条件，就保存更省的阵容。 

## Tips
因为浏览器本身的功能限制，最好不要完全挂在后台运行，这样运行的时间会被极大拉长。
