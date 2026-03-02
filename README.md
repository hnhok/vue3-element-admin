# Vue3-Element-Admin (PC Admin Template)

[![Vue](https://img.shields.io/badge/vue-3.5.x-brightgreen.svg)](https://vuejs.org/)
[![Vite](https://img.shields.io/badge/vite-6.0.x-646cff.svg)](https://vitejs.dev/)
[![Element Plus](https://img.shields.io/badge/element--plus-2.9.x-409eff.svg)](https://element-plus.org/)
[![TypeScript](https://img.shields.io/badge/typescript-5.7.x-blue.svg)](https://www.typescriptlang.org/)

这是一个基于 **Vue 3** + **Vite 6** + **Element Plus** 搭建的现代化后台管理系统。

## 🚀 特性

- ⚡ **现代化技术栈**：Vue 3.5+, Vite 6, TypeScript 5.7+。
- 🏢 **专业后台布局**：内置基于 Element Plus 的侧边栏、中后台常用组件。
- 📦 **组件按需加载**：自动导入 Element Plus 组件及 Vue/Router/Pinia 常用的组合式 API。
- 🎨 **原子化 CSS**：使用 UnoCSS 引擎，支持属性化模式（Attributify）。
- 🏪 **状态管理**：Pinia + 状态持久化插件（`pinia-plugin-persistedstate`）。
- 🚦 **规范开发**：
  - **ESLint 9** + **Prettier** 代码标准校验。
  - **Husky** + **lint-staged** 实现 Git 提交前检查。
  - **Commitlint** 强制 Angular 风格提交信息规范。

## 📂 目录结构

```text
src/
├── api/            # 接口请求
├── router/         # 路由配置
├── store/          # Pinia 状态管理
├── utils/          # 工具函数
├── views/          # 视图页面
│   ├── HomeView.vue         # 首页
│   ├── OrderDetail/         # 订单详情模块
│   └── UserProfile/         # 用户中心模块
├── App.vue         # 根组件
└── main.ts         # 入口文件
```

## 🛠️ 快速开始

### 安装依赖
```bash
npm install
```

### 启动开发环境
```bash
npm run dev
```

### 构建生产环境
```bash
npm run build
```

### 代码检查与格式化
```bash
npm run lint    # 运行 ESLint
npm run format  # 运行 Prettier 格式化
```

## 📝 Git 提交规范

项目强制执行规范化的提交信息，格式如下：
`<type>(<scope>): <subject>`

- `feat`: 新功能
- `fix`: 修复 bug
- `docs`: 文档变更
- `style`: 代码格式（不影响功能）
- `refactor`: 重构
- `perf`: 性能优化
- `test`: 测试
- `chore`: 构建过程或辅助工具的变动

## ⚠️ 注意事项

1. **项目名称与框架**：本项目命名为 `vue3-element-admin` 但实际主要使用 **Vant 4** 框架进行 H5 开发。
2. **PostCSS 适配**：基准设计稿宽度设为 `375px`。如果设计稿是 `750px`，请前往 `postcss.config.cjs` 修改 `viewportWidth`。
