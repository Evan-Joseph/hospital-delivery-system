# Hospital Delivery System (MediOrder)

一个专为医院场景设计的便捷订餐系统，为患者和医院用户提供简单、快速的订餐体验。

## 📋 项目概览

MediOrder 是一个创新的医院订餐解决方案，通过现代化的技术栈提供无缝的用户体验。

### 🎯 核心功能

- **二维码扫码下单**：通过扫描床头二维码自动填写配送信息
- **餐馆浏览**：展示附近合作餐馆及其菜单
- **智能支付**：支持多种支付方式，生成订单验证码
- **实时订单跟踪**：全程追踪订单状态
- **用户角色管理**：支持患者、商户、管理员多角色

## 🛠 技术架构

### 前端技术栈
- **框架**：Next.js 15 (App Router)
- **语言**：TypeScript
- **样式**：Tailwind CSS
- **UI组件**：Radix UI + shadcn/ui
- **图标库**：Lucide React
- **状态管理**：React Context API
- **表单处理**：React Hook Form
- **数据获取**：TanStack Query (React Query)

### 后端服务
- **当前**：Firebase (Firestore, Authentication, Storage)
- **计划迁移**：Supabase (PostgreSQL, Auth, Storage)

### AI集成
- **Genkit**：Google AI集成，提供智能功能

## 🚀 快速开始

### 环境要求
- Node.js 18+
- npm 或 yarn

### 安装依赖
```bash
npm install
```

### 开发环境运行
```bash
npm run dev
```

应用将在 http://localhost:9002 启动

### AI功能开发
```bash
npm run genkit:dev
```

## 📁 项目结构

```
src/
├── app/                 # 页面路由 (App Router)
│   ├── admin/          # 管理员功能模块
│   ├── merchant/       # 商户功能模块
│   ├── scan/           # 二维码扫描功能
│   ├── restaurants/    # 餐馆浏览功能
│   ├── checkout/       # 结账支付流程
│   ├── orders/         # 订单管理
│   └── cart/           # 购物车功能
├── components/         # 可复用UI组件
│   ├── ui/             # 基础UI组件 (shadcn/ui)
│   ├── layout/         # 布局组件
│   ├── cart/           # 购物车组件
│   ├── checkout/       # 结账组件
│   ├── merchant/       # 商户组件
│   ├── orders/         # 订单组件
│   └── restaurants/    # 餐馆组件
├── contexts/           # React Context状态管理
├── hooks/              # 自定义React Hooks
├── lib/                # 工具库和配置
├── types/              # TypeScript类型定义
└── ai/                 # AI功能集成
```

## 🎨 主要功能模块

### 👤 用户端
- 扫码订餐
- 餐馆浏览
- 菜单选择
- 购物车管理
- 订单支付
- 订单追踪
- 收藏功能

### 🏪 商户端
- 菜单管理
- 订单处理
- 促销活动
- 营业设置
- 数据统计

### 👨‍💼 管理员端
- 商户管理
- 二维码生成
- 系统监控
- 数据分析

## 🔧 配置说明

### 环境变量
创建 `.env.local` 文件：
```env
# Firebase配置
NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_auth_domain
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_storage_bucket
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id

# Genkit AI配置
GOOGLE_AI_API_KEY=your_google_ai_api_key
```

## 📱 屏幕截图

<!-- 这里可以添加应用截图 -->

## 🤝 贡献指南

1. Fork 本仓库
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开 Pull Request

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 📞 联系我们

- 项目链接：[https://github.com/Evan-Joseph/hospital-delivery-system](https://github.com/Evan-Joseph/hospital-delivery-system)
- 问题反馈：[Issues](https://github.com/Evan-Joseph/hospital-delivery-system/issues)

## 🙏 致谢

- [Next.js](https://nextjs.org/) - React框架
- [Tailwind CSS](https://tailwindcss.com/) - CSS框架
- [Radix UI](https://www.radix-ui.com/) - UI组件库
- [shadcn/ui](https://ui.shadcn.com/) - UI组件集合
- [Firebase](https://firebase.google.com/) - 后端服务
- [Genkit](https://firebase.google.com/docs/genkit) - AI集成框架
