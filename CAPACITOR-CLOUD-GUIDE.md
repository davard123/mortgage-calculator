# 📱 Capacitor Cloud 构建指南

## 快速开始

### 第 1 步：访问 Capacitor Cloud

**网址**：https://cloud.capacitorjs.com

### 第 2 步：登录

1. 点击 **"Sign In"** 或 **"Get Started"**
2. 选择 **"Continue with GitHub"**
3. 授权访问您的 GitHub 账号

### 第 3 步：创建项目

1. 点击 **"Create Project"**
2. 选择 **"Import from GitHub"**
3. 找到并选择 `davard123/mortgage-calculator` 仓库
4. 点击 **"Import"**

### 第 4 步：配置构建

**项目名称**：`mortgage-calculator`（自动填充）

**构建配置**（通常自动检测）：
- **Framework**: Capacitor
- **Node Version**: 18.x
- **Build Command**: `npm ci && npx cap sync`

### 第 5 步：构建 Android

1. 在项目页面，点击 **"Android"** 标签
2. 点击 **"Build Now"**
3. 等待构建完成（约 5-10 分钟）
4. 构建成功后，点击 **"Download"** 下载 APK/AAB

**下载的文件**：
- `app-release.apk` - 可直接安装
- `app-release.aab` - 上传到 Google Play（推荐）

### 第 6 步：构建 iOS（需要 Apple Developer 账号）

1. 点击 **"iOS"** 标签
2. 上传 Apple 证书：
   - **Distribution Certificate** (.p12)
   - **Provisioning Profile** (.mobileprovision)
3. 点击 **"Build Now"**
4. 下载 IPA 文件

---

## 🔑 获取 Apple 证书（仅 iOS 需要）

### 方法 1：在 Mac 上导出

1. 打开 **Xcode** → **Preferences** → **Accounts**
2. 选择您的 Apple ID
3. 管理证书
4. 导出 .p12 文件

### 方法 2：使用 Codemagic（无需 Mac）

如果无法获取 Apple 证书，可以使用 **Codemagic**：

1. 访问 https://codemagic.io
2. 用 GitHub 登录
3. 添加项目
4. 选择 "iOS" 平台
5. Codemagic 会引导您配置证书

---

## 📦 上传到应用商店

### Google Play Store

1. 访问 https://play.google.com/console
2. 创建新应用
3. 填写应用信息：
   - **应用名称**：贷款计算器
   - **简短描述**：专业的房贷计算工具
   - **分类**：财务
4. 上传 `app-release.aab` 文件
5. 填写内容评级问卷
6. 提交审核

**审核时间**：通常 1-3 天

### Apple App Store

1. 访问 https://appstoreconnect.apple.com
2. 创建新 App
3. 填写应用信息
4. 上传 IPA 文件（使用 Xcode 或 Transporter）
5. 填写隐私政策
6. 提交审核

**审核时间**：通常 1-2 天

---

## 💰 费用

| 平台 | 费用 | 支付周期 |
|------|------|----------|
| Google Play | $25 | 一次性 |
| Apple App Store | $99 | 每年 |
| Capacitor Cloud | 免费 | 每月 5 次构建 |

---

## 🔗 有用链接

- **Capacitor Cloud**: https://cloud.capacitorjs.com
- **Capacitor 文档**: https://capacitorjs.com
- **Google Play Console**: https://play.google.com/console
- **App Store Connect**: https://appstoreconnect.apple.com
- **Codemagic**（备选）: https://codemagic.io

---

## ❓ 常见问题

### Q: 构建失败怎么办？
A: 检查构建日志，通常是依赖问题。可以尝试：
```bash
npm ci
npx cap sync
```

### Q: 需要上传 node_modules 吗？
A: 不需要！云构建会自动安装依赖。

### Q: 可以自定义应用图标吗？
A: 可以！替换 `android/app/src/main/res/mipmap-*` 和 `ios/App/App/Assets.xcassets/AppIcon.appiconset/` 中的图片。

### Q: 如何更新应用？
A: 修改代码后，推送新的 commit 到 GitHub，然后重新构建即可。
