# 🏠 Loan Calculator Suite - 贷款计算器套件

专业的房贷计算工具 - 苹果风格设计

## ✨ 功能特性

### 5 大核心计算器

1. **🏡 买卖房地产计算器 (Buy/Sell)**
   - 支持 6 种贷款类型：Conventional、Non-QM、DSCR、Bank Statement、FHA、VA
   - 计算月供、LTV、DTI 等关键指标
   - DSCR 投资房产租金计算
   - FHA 贷款限额查询（56 州 + 领地完整数据）
   - VA 贷款资格判断与对比

2. **💰 重贷计算器 (Refinance)**
   - Rate and Term 模式
   - Cash Out 模式
   - 计算每月节省和回本时间

3. **💵 收入计算器 (Income)**
   - W2 工资收入（多种支付周期）
   - 小时工收入
   - 自雇收入（DU/LP 两种计算方式）
   - 租金收入（75% 计算）
   - 其他收入（儿童抚养、社会福利等）

4. **📋 Closing Cost 计算器**
   - Lender Fees（贷款机构费用）
   - Third Party + Title（第三方 + 产权费用）
   - Prepaid（预付费用）
   - Credits（抵免）

5. **ℹ️ About**
   - 多语言支持（中文、English、Español）
   - 使用说明
   - 版本历史
   - 免责声明

## 🎨 设计特点

- **苹果风格设计**：简洁、现代、大圆角
- **毛玻璃效果**：`backdrop-filter: blur(20px)`
- **柔和阴影**：舒适的视觉层次
- **渐变按钮**：Apple Blue 配色
- **响应式布局**：完美适配手机和桌面

## 🌐 多语言支持

- 🇨🇳 中文
- 🇺🇸 English
- 🇪🇸 Español

## 📁 文件结构

```
mortgage-calculators/
├── index.html      # 主页面（包含所有 CSS 和 JavaScript）
├── README.md       # 项目说明
└── CHANGES.md      # 变更日志
```

## 🚀 部署

### Vercel 部署

1. 访问 [vercel.com](https://vercel.com)
2. 登录 GitHub 账号
3. 点击 "New Project"
4. 选择 `mortgage-calculator` 仓库
5. 点击 "Deploy"
6. 获取预览链接

### GitHub Pages 部署

1. 进入仓库 Settings
2. 选择 Pages
3. Source 选择 `main` branch
4. 保存后获取链接

## 📊 技术栈

- HTML5
- CSS3（CSS Variables、Flexbox、Grid、Animations）
- 原生 JavaScript（ES6+）
- 无需后端，所有计算在浏览器完成

## 📱 测试重点

- ✅ 手机界面响应式
- ✅ 所有计算器功能
- ✅ 多语言切换
- ✅ 表单输入和计算结果

## 📧 联系方式

- 邮件：daviddairealty@gmail.com

## 📄 许可证

MIT License

## 🔄 版本历史

### v1.0.1 (2026-03-21)
- 添加 DSCR 租金收入计算
- 添加 VA 贷款对比功能
- 重构收入计算逻辑
- 支持多份工作收入

### v1.0.0 (2026-03-21)
- 初始版本
- 5 大核心功能上线
- 苹果风格 UI 设计

---

© 2026 Loan Calculator Suite. All rights reserved.
