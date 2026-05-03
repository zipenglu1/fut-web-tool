# FSU EAFC FUT Web PLUS

<p align="center">
  <strong>EA SPORTS FC Ultimate Team Web App userscript for SBC automation, player management, price tools, pack utilities, and enhanced card information.</strong>
</p>

<p align="center">
  <a href="#中文">中文</a> · <a href="#english">English</a>
</p>

<p align="center">
  <img alt="Version" src="https://img.shields.io/badge/version-26.08.1-blue">
  <img alt="Type" src="https://img.shields.io/badge/type-userscript-orange">
  <img alt="Runtime" src="https://img.shields.io/badge/runtime-Tampermonkey%20%2F%20Violentmonkey-green">
  <img alt="License" src="https://img.shields.io/badge/license-MIT-lightgrey">
</p>

---

<a id="中文"></a>

## 中文

### 项目简介

**FSU EAFC FUT Web PLUS** 是基于 FSU 的 EA SPORTS FC Ultimate Team Web App 增强脚本。  
本版本在原 FSU 功能基础上，面向 SBC、球员管理、价格查询、开包、FUT.GG / FUTBIN 辅助和球员信息展示做了扩展与优化。
与原版差异内容视频介绍：https://space.bilibili.com/80008515

脚本当前版本为 **26.08.1**，适用于 EA SPORTS FC Ultimate Team Web App。

> 本项目不是 EA 官方工具。请自行评估自动化操作风险，尤其是自动提交 SBC、批量开包、批量出售、自动购买等功能。

---

### 核心功能

#### SBC 自动化

- 高级混合联赛 / 指定 SBC 自动循环处理。
- 自动寻找未完成挑战。
- 自动读取并填充 SBC 方案。
- 自动替换假想球员。
- 满足条件后自动提交。
- 完成后自动刷新列表并继续下一项。
- 对无法完成的挑战进行临时跳过，避免循环卡死。
<img width="766" height="481" alt="image" src="https://github.com/user-attachments/assets/03242bdb-77ea-4448-85d1-abab9d5c9225" />

-点击开始循环进行自动化进程

#### SBC 方案与填充增强

- 支持 FUTBIN / FUT.GG 方案导入。
- 支持内置默认方案。
- 支持高级混合联赛默认方案。
- 支持英超 / 西甲默认方案。
- 支持一键填充、重复球员优先填充、阵容补全。
- 支持一键替换假想球员。
- 支持假想球员直接购买与批量购买。
- 支持根据评分范围、联赛、稀有度、可交易状态、进化状态等条件进行筛选。

#### SBC 仓库与重复球员处理

- 优先使用 SBC 仓库球员。
- 支持 SBC 仓库球员列表。
- 支持仓库球员批量发送回俱乐部。
- 支持未分配重复球员与俱乐部可交易版本批量交换。
- 支持重复球员快速完成可匹配 SBC。
- 支持提交前检测未分配不可交易版本，并尝试自动替换。

#### 开包与未分配管理

- 支持跳过开包动画。
- 支持快速开包入口。
- 支持批量打开球员包。
- 支持自动分配开包结果：
  - 非重复球员发送至俱乐部。
  - 符合条件的重复球员发送至 SBC 仓库。
  - 无法处理时停止并展示未分配列表。
- 支持按包回报价值排序。
- 支持未分配列表刷新。
- 支持一键领取并发送球员至俱乐部。
- 支持按评分阈值快速出售低评分物品，并可排除指定联赛。

#### 球员信息增强

- 显示球员价格、评分低价、购买价格。
- 显示额外位置、俱乐部拥有状态、重复状态、低价信息。
- 支持球员锁定 / 解锁。
- 支持球员加速类型计算。
- 支持体型、真实脸、动态升级、额外默契等信息展示。
- 支持球员元评分与排名。
- 支持 FG / FUT.GG 风格的角色评分查看。
- 支持查看可进化任务与进化收益信息。

#### 市场与价格工具

- 查询球员拍卖低价。
- 刷新拍卖低价。
- 快速按低价挂牌。
- 批量拍卖所选球员。
- 支持修改挂牌时间。
- 支持假想球员拍卖搜索优化。
- 支持球员自动购买测试功能。
- 支持 FUTBIN / FUT.GG 跳转与价格辅助。

#### 目标、SBC 与信息面板

- 首页显示新增目标、即将到期目标与奖励摘要。
- SBC 页面显示造价预估、阵容价值、点赞 / 点踩参考。
- 顶部 SBC 快捷入口。
- SBC 子任务筛选与完成状态展示。
- SBC 计数器，便于观察当日提交数量。
- 需求球员统计，辅助评估库存缺口。

---

### 安装方式

#### 1. 安装 userscript 管理器

推荐使用以下任意一个浏览器扩展：

- [Tampermonkey](https://www.tampermonkey.net/)
- [Violentmonkey](https://violentmonkey.github.io/)
- ScriptCat

#### 2. 安装脚本

将仓库中的脚本文件导入 userscript 管理器：

```text
【FSU】 EAFC FUT WEB增强器PLUS-26.08.user.js
```

或者新建脚本，复制文件内容并保存。

#### 3. 打开 Web App

访问 EA SPORTS FC Ultimate Team Web App，等待页面完全加载。  
脚本会在页面加载后自动初始化。

---

### 支持页面

脚本匹配以下页面类型：

- EA SPORTS FC Ultimate Team Web App
- easports.com 旧域名 Web App
- FUTBIN
- FUT.GG
- EasySBC Evolutions 页面

---

### 快速开始

#### 基础使用

1. 安装并启用脚本。
2. 打开 EA SPORTS FC Ultimate Team Web App。
3. 等待插件加载完成。
4. 进入 SBC、球员列表、商店或未分配页面。
5. 根据页面新增按钮使用对应功能。

#### 使用自动 SBC 循环

1. 进入目标 SBC 组的挑战列表页面。
2. 点击页面顶部或标题区域中的 **开始循环**。
3. 脚本会自动寻找未完成挑战。
4. 自动填充方案、替换假想球员并尝试提交。
5. 点击 **停止循环** 可中断流程。

#### 使用一键替换假想球员

1. 打开含有假想球员的 SBC 阵容。
2. 点击 **一键替换假想球员**。
3. 脚本会优先尝试满足 SBC 条件。
4. 根据设置优先使用 SBC 仓库球员或普通俱乐部球员。

---

### 推荐配置

根据使用习惯，可在插件设置中重点检查：

- 是否优先使用 SBC 仓库球员。
- 是否启用重复球员填充。
- 是否启用阵容补全。
- 是否排除可交易球员。
- 是否排除进化球员。
- 是否排除指定联赛。
- 是否允许使用特殊稀有度球员。
- 青铜 / 白银是否优先普通品质。
- 黄金球员评分范围。
- 批量开包低评分处理阈值。
- 是否显示球员元评分与排名。

---

### 使用建议

- 自动提交类功能建议适度使用。
- 不建议长时间无人值守运行自动循环。
- 运行自动流程时尽量保持页面可见，避免浏览器后台节流。
- 网络不稳定时不要连续触发自动操作。
- 自动购买、批量开包、快速 SBC 等功能请先小范围测试。
- 高价值球员较多时，建议开启锁定与提交前提示。

---

### 常见问题

#### 脚本没有加载

请检查：

- userscript 管理器是否启用。
- 脚本是否启用。
- 当前页面是否在脚本 `@match` 范围内。
- 页面是否已经完全加载。
- 浏览器控制台是否有报错。

#### 自动循环卡住

可以尝试：

- 点击停止循环。
- 刷新 Web App。
- 重新进入 SBC 页面。
- 检查挑战是否仍有可完成方案。
- 查看控制台错误信息。

#### 一键替换后仍有假想球员

可能原因：

- 俱乐部球员不足。
- SBC 仓库球员不足。
- 当前阵容条件过于严格。
- 排除联赛、排除可交易、排除进化、排除特殊卡等设置过严。
- 默契条件无法满足。

#### 批量开包停止

通常表示存在无法自动分配的未分配球员。  
请进入未分配列表手动处理，或使用脚本提供的交换、发送俱乐部、快速出售等功能。

#### 价格不显示或读取失败

可以尝试：

- 刷新页面。
- 检查网络连接。
- 检查 FUTBIN / FUT.GG 是否可访问。
- 检查 FUTGG 转发地址设置是否正确。
- 稍后重试。

---

### 开发与维护

#### 项目结构

当前项目以单 userscript 文件为主：

```text
【FSU】 EAFC FUT WEB增强器PLUS-26.08.user.js
```

#### 修改后建议检查

每次修改脚本后，建议至少验证：

- Web App 首页是否正常加载。
- 设置入口是否正常打开。
- SBC 页面按钮是否正常显示。
- 一键填充是否可用。
- 一键替换假想球员是否可用。
- 自动 SBC 循环是否能启动和停止。
- 仓库、重复、未分配标识是否正常。
- 控制台是否存在阻断性错误。

#### 建议的 Issue 模板

```text
## 问题描述

## 脚本版本

## 浏览器与脚本管理器

## 触发页面

## 复现步骤
1.
2.
3.

## 预期表现

## 实际表现

## 控制台报错

## 截图或录屏
```

---

### 版本说明

当前 README 基于 **FSU EAFC FUT Web Enhancer PLUS 26.08.1** 编写。

主要能力包括：

- 自动完成 / 循环处理 SBC。
- 高级混合联赛与部分默认方案增强。
- SBC 仓库优先与重复球员处理。
- 批量开包与自动分配。
- 球员元评分、FG 角色评分、体型与真实脸信息。
- FUTBIN / FUT.GG / EasySBC 相关辅助功能。
- 价格、拍卖、自动购买与球员管理工具。

---

### 免责声明

本项目仅供学习、研究和个人使用。  
本项目与 Electronic Arts、EA SPORTS、EA SPORTS FC、FIFA、Ultimate Team、FUTBIN、FUT.GG、EasySBC 等品牌或产品无官方关联。  
使用本脚本可能违反相关平台服务条款，或带来账号限制、功能限制、提交失败、数据异常、游戏内资产损失等风险。  
任何使用后果均由使用者自行承担。

---

<a id="english"></a>

## English

### Overview

**FSU EAFC FUT Web PLUS** is a userscript for the EA SPORTS FC Ultimate Team Web App, based on the original FSU enhancer and extended with additional automation, SBC workflow improvements, player management tools, price utilities, pack tools, and enhanced player-card information.

Current version: **26.08.1**.  
The script targets the EA SPORTS FC Ultimate Team Web App.
Different between originl FSU：https://space.bilibili.com/80008515
> This project is not affiliated with EA. Use automation features at your own risk, especially automatic SBC submission, bulk pack opening, quick selling, and auto-buying.

---

### Key Features

#### SBC Automation

- Automated SBC loop for selected SBC sets.
- Finds incomplete challenges automatically.
- Loads and fills SBC squad templates.
- Replaces concept players automatically.
- Submits the challenge when all requirements are met.
- Refreshes the challenge list and continues to the next challenge.
- Temporarily skips failed challenges to avoid blocking the loop.
<img width="766" height="481" alt="image" src="https://github.com/user-attachments/assets/08207f9f-b146-45d7-8775-483bae02f1f9" />

-Entering'开始循环'to star loop

#### SBC Template and Squad Building Enhancements

- Import SBC solutions from FUTBIN or FUT.GG.
- Built-in default templates.
- Premium Mixed Leagues default solutions.
- Premier League / LaLiga default solutions.
- One-click fill, duplicate-priority fill, and squad completion.
- One-click concept player replacement.
- Direct and batch purchase for concept players.
- Filters by rating range, league, rarity, tradeable status, Evolution status, and more.

#### SBC Storage and Duplicate Management

- Prioritize SBC Storage players.
- View SBC Storage player list.
- Bulk send SBC Storage players back to Club.
- Swap unassigned duplicates with tradeable Club versions.
- Use duplicate players to quickly complete supported SBCs.
- Detect unassigned untradeable versions before submission and attempt automatic replacement.

#### Pack and Unassigned Item Tools

- Skip pack animations.
- Quick pack opening entry.
- Bulk open player packs.
- Automatically assign pack results:
  - Send non-duplicates to Club.
  - Send eligible duplicates to SBC Storage.
  - Stop and show the unassigned list when manual handling is required.
- Sort packs by expected return value.
- Refresh the unassigned list.
- Claim and send players to Club.
- Quick sell low-rated items under a configurable threshold, with league exclusions.

#### Player Information Enhancements

- Display player price, rating floor price, and purchase price.
- Display extra positions, Club ownership, duplicate status, and low-price information.
- Lock and unlock players.
- Calculate acceleration type.
- Display body type, real-face status, dynamic upgrade status, and extra chemistry information.
- Display player meta rating and rank.
- View FG / FUT.GG-style role ratings.
- Show available Evolution tasks and Evolution upgrade information.

#### Market and Price Tools

- Search auction low price.
- Refresh auction price.
- Quick list at low price.
- Bulk auction selected players.
- Customize auction duration.
- Optimize concept-player auction search.
- Experimental player auto-buy module.
- FUTBIN / FUT.GG navigation and price helpers.

#### Objectives, SBC Panels, and Dashboards

- Show newly added Objectives, expiring Objectives, and reward summaries.
- Show SBC estimated cost, squad value, thumbs-up / thumbs-down references.
- Top SBC shortcut entry.
- SBC sub-challenge filters and completion states.
- SBC counter for daily submission awareness.
- Required-player statistics for inventory planning.

---

### Installation

#### 1. Install a userscript manager

Recommended options:

- [Tampermonkey](https://www.tampermonkey.net/)
- [Violentmonkey](https://violentmonkey.github.io/)
- ScriptCat

#### 2. Install the script

Import this userscript file into your userscript manager:

```text
【FSU】 EAFC FUT WEB增强器PLUS-26.08.user.js
```

Alternatively, create a new userscript, paste the file content, and save it.

#### 3. Open the Web App

Open the EA SPORTS FC Ultimate Team Web App and wait for the page and script to finish loading.

---

### Supported Pages

The script is designed to match:

- EA SPORTS FC Ultimate Team Web App
- Legacy easports.com Web App URLs
- FUTBIN
- FUT.GG
- EasySBC Evolutions pages

---

### Quick Start

#### Basic Usage

1. Install and enable the script.
2. Open the EA SPORTS FC Ultimate Team Web App.
3. Wait until the enhancer loads.
4. Navigate to SBC, player list, Store, or Unassigned pages.
5. Use the additional buttons injected by the script.

#### Auto SBC Loop

1. Open the target SBC set challenge list.
2. Click **Start Loop**.
3. The script will find the next incomplete challenge.
4. It will fill the squad, replace concept players, and attempt submission.
5. Click **Stop Loop** to interrupt the process.

#### Concept Player Replacement

1. Open an SBC squad containing concept players.
2. Click the one-click concept replacement button.
3. The script will search for valid replacements.
4. Depending on your settings, it can prioritize SBC Storage players or regular Club players.

---

### Recommended Settings

Check these settings based on your play style:

- Prioritize SBC Storage players.
- Enable duplicate-player fill.
- Enable squad completion.
- Exclude tradeable players.
- Exclude Evolution players.
- Exclude selected leagues.
- Allow or block special rarity players.
- Prioritize common Bronze / Silver players.
- Gold player rating range.
- Bulk pack quick-sell threshold.
- Player meta rating and rank display.

---

### Usage Tips

- Use automatic submission features moderately.
- Avoid long unattended auto loops.
- Keep the Web App tab visible while automation is running to reduce browser throttling.
- Avoid repeated automatic actions when the network is unstable.
- Test auto-buy, bulk pack opening, and quick SBC features on low-risk scenarios first.
- Lock valuable players before running automation.

---

### FAQ

#### The script does not load

Check:

- Your userscript manager is enabled.
- The script is enabled.
- The current URL matches the script rules.
- The Web App has fully loaded.
- The browser console does not show blocking errors.

#### Auto loop gets stuck

Try:

- Click Stop Loop.
- Refresh the Web App.
- Re-enter the SBC page.
- Check whether the challenge still has a valid solution.
- Inspect the browser console.

#### Concept players remain after replacement

Possible causes:

- Insufficient Club players.
- Insufficient SBC Storage players.
- SBC requirements are too strict.
- Exclusion settings are too restrictive.
- Chemistry requirements cannot be met.

#### Bulk pack opening stops

This usually means some unassigned items cannot be handled automatically.  
Open the unassigned list and resolve them manually, or use the script’s swap, send-to-club, and quick-sell tools.

#### Price data is missing

Try:

- Refresh the page.
- Check your network.
- Verify FUTBIN / FUT.GG availability.
- Check the FUTGG proxy setting.
- Retry later.

---

### Development and Maintenance

#### Project Structure

The project is primarily maintained as a single userscript:

```text
【FSU】 EAFC FUT WEB增强器PLUS-26.08.user.js
```

#### Suggested Checks After Changes

After editing the script, verify at least:

- Web App home page loads normally.
- Settings panel opens.
- SBC buttons appear.
- One-click fill works.
- Concept replacement works.
- Auto SBC loop can start and stop.
- Storage, duplicate, and unassigned markers display correctly.
- No blocking console errors are present.

#### Suggested Issue Template

```text
## Description

## Script Version

## Browser and Userscript Manager

## Page / Area

## Steps to Reproduce
1.
2.
3.

## Expected Behavior

## Actual Behavior

## Console Errors

## Screenshots or Recording
```

---

### Version Notes

This README is based on **FSU EAFC FUT Web Enhancer PLUS 26.08.1**.

Major capabilities include:

- Automated SBC completion and looping.
- Premium Mixed Leagues and default-template enhancements.
- SBC Storage priority and duplicate-player handling.
- Bulk pack opening and auto assignment.
- Player meta rating, FG role rating, body type, and real-face information.
- FUTBIN / FUT.GG / EasySBC helper features.
- Price, auction, auto-buy, and player-management tools.

---

### Disclaimer

This project is for learning, research, and personal use only.  
It is not affiliated with Electronic Arts, EA SPORTS, EA SPORTS FC, FIFA, Ultimate Team, FUTBIN, FUT.GG, or EasySBC.  
Using this script may violate platform terms of service or lead to account restrictions, feature restrictions, submission failures, data inconsistencies, or in-game asset loss.  
You are solely responsible for any consequences of using this script.
