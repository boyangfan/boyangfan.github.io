# 兔了个兔（xlegex）

一个基于 **Vue 3 + TypeScript + Vite** 的轻量三消叠牌小游戏，灵感来自“羊了个羊”玩法。

## 项目简介

玩家需要从牌堆中点击卡片，将卡片放入底部槽位；当槽位中出现 3 张相同卡片时会自动消除。槽位满且无法继续消除时判定失败。

当前版本包含 3 个关卡，并提供：

- 卡片点击/落位交互
- 三张同类自动消除
- 回退功能
- “移出前三个”道具功能
- 关卡提示与胜负音效
- 完成最终关卡后的庆祝效果

## 技术栈

- Vue 3
- TypeScript
- Vite
- UnoCSS

## 本地开发

> 建议使用 `pnpm`。

```bash
pnpm install
pnpm dev
```

开发服务器启动后，按终端提示打开本地地址（通常为 `http://localhost:5173`）。

## 构建与预览

```bash
pnpm build
pnpm preview
```

## 常用脚本

- `pnpm dev`：启动开发环境
- `pnpm build`：类型检查并构建生产包
- `pnpm preview`：预览构建结果
- `pnpm lint`：运行 ESLint
- `pnpm lint:fix`：自动修复可修复的 lint 问题

## 目录结构（节选）

```text
src/
  App.vue              # 主界面与关卡逻辑挂载
  core/
    useGame.ts         # 游戏核心状态与操作逻辑
    utils.ts           # 动画/特效工具方法
  components/
    card.vue           # 单张卡片组件
public/audio/          # 音效资源
```

## 许可证

本项目采用仓库中的 [LICENSE](./LICENSE) 许可条款。
