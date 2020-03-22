## 分支处理原则
- 任何时间Master都保持最终线上状态，只有Release和Hotfix可以改变
- 任何新分支都从Master新建
- Feature，Fixbug分支用以自测或Smoke测试
- 上线使用Release分支，完毕后merge入Master
- Release分支只Merge该阶段准备上线的Feature和Bugfix任务
- Hotfix直接Merge入Master进行上线


## 各个场景对应流程
### 1 功能开发
从Master分支新建Feature分支
开发完成自测结束
等待Release时间确定合并至Release
UAT Release后上线

### 2 线上遗留BUG处理
从Master分支新建Bugfix分支
开发完成自测结束
等待Release时间确定合并至Release
UAT Release后上线

### 3 紧急修复
从Master分支新建Bugfix分支
UAT Bugfix后直接上线
