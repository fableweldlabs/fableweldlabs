# Shops, Crafting & Economy — 简体中文

1. 下载可选的 Lumen Vale 可编辑示例，用 Godot 4.7.2 打开 `project.godot` 并按 F5。选择简体中文，然后打开经济工坊。若要单独运行组件场景，请打开 `demo/economy_quick_start.tscn` 并按 F6。必需的插件下载不包含示例项目。
2. 在“制作”中选择药水，批次数保持为 1，然后制作。初始的 12 株药草中会消耗 2 株，获得 1 瓶药水；可在“背包”查看。在“商店”选择物品和数量后购买或出售。预览会显示价格或无法交易的原因。
3. 在“保存和读取”中保存经济数据。关闭并重新打开示例，然后读取。文件为 `user://economy-workshop.json`；读取会替换当前经济会话。任务、生命值和世界位置需要由游戏自己的存档系统保存。
4. 只安装插件时，将 `addons/fableweld_inventory` 复制到项目，在 Project Settings > Plugins 中启用 Fableweld Shops, Crafting & Economy。自建目录资源和生成的场景应保存在 `addons` 之外。保存前验证目录；在设置页使用尚不存在的 `res://` 路径生成经济场景。
5. 更新前保留项目和存档，禁用插件并关闭 Godot，只替换供应商的插件目录，再重新打开并验证目录资源和存档的副本。保持物品和会话 ID 稳定。迁移旧 Inventory 存档时，先预览，再写入不同的经济存档文件；原文件不变。此迁移不支持包含时钟的组合存档。
6. 基本交易和制作不需要时钟插件。缺少翻译时显示原始文本。在商贩练习中，先点击练习区域或用 Tab 聚焦，再用方向键移动。本文说明适用于 Shops, Crafting & Economy 1.0.0。许可条款及例外见 `LICENSE-ECONOMY.txt`、`LICENSE-COMPONENTS.txt` 和 `LICENSE-MIT.txt`。
