# Enterprise React Demo

一个小体量、企业后台风格的 React 学习项目。它不是空模板，而是把真实项目里常见的结构压缩成可读版本：登录态、受保护路由、后台布局、数据请求、查询表格、弹窗表单、状态管理和主题配置。

## 技术栈

- React 19.2.7
- Vite 8.0.16
- TypeScript
- Ant Design 6.4.3
- React Router 7.17.0
- TanStack Query 5.101.0
- Zustand 5.0.14
- Lucide React 1.17.0

## 启动

```bash
npm install
npm run dev
```

登录页账号密码可随意输入，默认值已经填好。

## 目录

```text
src/
  app/              应用入口、路由、Provider
  features/         业务模块：登录、总览、客户、订单、设置
  shared/
    api/            mock API、类型、数据
    auth/           登录态和路由守卫
    layout/         后台主布局
    ui/             通用展示组件
    utils/          格式化工具
  styles/           全局样式
```

## 学习建议

1. 先从 `src/app/router.tsx` 看页面如何组织。
2. 再看 `src/shared/auth/AuthGuard.tsx` 和 `authStore.ts`，理解登录态。
3. 然后看 `src/features/customers/CustomersPage.tsx`，里面有查询、表格、弹窗表单和缓存刷新。
4. 最后把 `src/shared/api/client.ts` 换成真实后端接口。
