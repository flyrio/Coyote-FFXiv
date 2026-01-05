# Coyote-FFXiv

通过 Dalamud 插件对接 Coyote 服务器，实现聊天/血量/状态触发等自动控制。

## 功能概览
- `/coyote` 打开主界面
- `/coyotefire <火力> <时间ms> <是否重置计时> [波形ID]`
- `/emoteid <emoteId>` 执行已解锁表情
- 触发器：聊天触发、血量触发、状态触发
- 状态图标大全与名称复制

## 快速开始
1. 确保 Coyote 服务器正常运行，记录 IP/端口 与 ClientID。
2. 游戏内输入 `/coyote`，填写 `CoyoteIP` 与 `ClientID`，点击“测试连通性”。
3. 在“触发”页面配置规则并开启总开关。

## 配置文件
以下文件会保存在 Dalamud 插件配置目录中：
- `chatTriggerRules.json`
- `hpTriggerRules.json`
- `BuffTriggerConfig.json`

默认路径示例：
`AppData\Roaming\XIVLauncherCN\pluginConfigs\Coyote-FFXiv\`

## 开发/编译
- 打开 `Coyote-FFXiv.sln`
- 项目文件：`Coyote-FFXiv/Coyote-FFXiv.csproj`
- 目标框架：`net10.0-windows7.0`（Dalamud.CN.NET.SDK/14.0.1）
- 资源：`Data/Coyote.png` 会复制到输出目录

## 许可
见 `LICENSE.md`。
