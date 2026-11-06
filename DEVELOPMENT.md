# site-status · 开发与部署

## 环境要求
- Node.js、pnpm 9.12.2（见 `packageManager`）
- UptimeRobot API Key（或其它监控数据源）

## 配置
```bash
cp .env.example .env
```
按 `README.md` / `README.zh-CN.md` 填入 API Key 与站点列表。

## 本地开发（Nuxt 3）
```bash
pnpm install --frozen-lockfile
pnpm dev
```

## 构建
```bash
pnpm build        # SSR 构建
pnpm generate     # 静态生成
pnpm pwa          # PWA 产物
pnpm preview      # 本地预览
```

## 部署
```bash
pnpm vercel       # 部署到 Vercel
```
也可托管 `pnpm generate` 产出的静态目录；配置见 `nuxt.config.ts`。
