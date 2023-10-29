# skland-checkin-ghaction

利用 GitHub Action 自动完成森空岛签到，基于 ~~[Maojuan-lang](https://github.com/Maojuan-lang/SenKongDao)~~ [nonbot plugin](https://github.com/GuGuMur/nonebot-plugin-skland-arksign) 的实现包装。

~~只是一点微小的工作。~~

## How to
1. fork 本仓库
2. 点击顶部 Settings 选项卡进入仓库设置
3. 左侧栏找到 Security 一节，点击展开 Secrets and variables，点击 Actions
4. 在右侧点击 New repository secret 按钮，新建一个名为``UID``的 secret，内容为你的所有绑定游戏账号的UID（以``;;``分隔）
5. 同样的新建一个名为``CRED``的 secret，内容为[你的森空岛token](https://web-api.skland.com/account/info/hg)（需要登录账号）。
6. 编辑这个README（或者你懂怎么 commit），提交后立刻触发签到，或者等它自动启动<br>默认每日北京时间4:00启动，可自行修改workflow触发时间，注意 Action 使用的是 UTC +0 时区，你需要手动减去8个小时后再填入你的时间