# skland-checkin-ghaction

利用 GitHub Action 自动完成森空岛签到，基于[Maojuan-lang](https://github.com/Maojuan-lang/SenKongDao)的实现包装。

## How to
1. fork 本仓库
2. 点击顶部 Settings 选项卡进入仓库设置
3. 左侧栏找到 Security 一节，点击展开 Secrets and variables，点击 Actions
4. 在右侧点击 New repository secret 按钮，新建一个名为``UID``的 secret，内容为你的所有绑定游戏账号的UID（以``&``分隔）
5. 同样的新建一个名为``CRED``的 secret，内容为你的cred（可通过登录网页端森空岛后，打开开发工具→应用→本地存储空间查看）
6. 编辑这个README（或者你懂怎么 commit），提交后立刻触发签到，或者等它自动启动
