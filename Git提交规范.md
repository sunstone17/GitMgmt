# Branch 规则
  
 **格式 前缀_任务ID_时间戳** 其中时间戳为可选  
 **前缀**  
 Feature: 新功能[使用的Feature任务ID]  
 Bugfix: 线上BUG修复[使用子任务Task或者BUG的ID]   
 Hotfix: 紧急修复[修复后需马上Merge到主分支]   
 Release: 上线分支[确定上线节点后开启，所有Feature和Bugfix分支都需要Merge到Release分支，没有任务ID
  
**示例**  
Feature_10_20191016  
Bugfix_15_20191016  
Hotfix_20_20191016  
Release_20191016/Release_V180  



# Commit 规则  

**前缀使用以下标识开头**  
**前缀**  
Dev：开发  
Fix：修补bug  
Docs：文档（documentation）  
Style： 格式（不影响代码运行的变动）  
Refactor：重构（即不是新增功能，也不是修改bug的代码变动）  
Test：增加测试或单元测试  
Chore：构建过程或辅助工具的变动  

**示例**  
Dev: 新增读取医生信息字段XX  
Fix: 修复标题长度限制BUG  
Style: XX列表样式增加背景颜色  
