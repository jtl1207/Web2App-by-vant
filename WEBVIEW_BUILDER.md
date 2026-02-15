# 📱 WebView App Builder

> 将任何网站快速打包成 Android 应用 / Package any website as an Android app in minutes

## 🚀 快速开始 / Quick Start

### 只需三步！/ Just 3 Steps!

#### 1️⃣ 编辑配置 / Edit Config
```json
// app-config.json
{
  "appName": "我的应用",
  "packageId": "com.example.app",
  "appUrl": "https://example.com",
  "allowedDomains": ["example.com"]
}
```

#### 2️⃣ 运行构建 / Run Build
```bash
bun run build:app
```

#### 3️⃣ 获取 APK / Get APK
```
WebApkShell/app/build/outputs/apk/release/app_*.apk
```

## 📚 完整文档 / Documentation

| 文档 | 说明 | 适用场景 |
|------|------|----------|
| [**QUICKSTART.md**](./QUICKSTART.md) | 快速开始指南 | 第一次使用 |
| [**CONFIG_GUIDE.md**](./CONFIG_GUIDE.md) | 配置详细说明 | 了解配置选项 |
| [**WEBVIEW_APP_README.md**](./WEBVIEW_APP_README.md) | 完整使用文档 | 深入了解功能 |
| [**SUMMARY.md**](./SUMMARY.md) | 项目改进总结 | 了解项目价值 |
| [app-config.example.json](./app-config.example.json) | 配置示例 | 参考配置 |

## 🌟 核心特性 / Features

### ⚡ 极速上手
- 只需修改一个配置文件
- 一条命令完成构建
- 5分钟从网站到APP

### 🔒 安全可靠
- 自动拦截广告链接
- 防止恶意跳转
- 阻止XSS攻击
- 严格的域名验证

### 📦 功能完整
- 支持任何网站
- 动态域名配置
- 自动版本管理
- GitHub Actions集成

### 📖 文档完善
- 从入门到精通
- 详细配置说明
- 真实使用案例
- 常见问题解答

## 💡 使用案例 / Examples

### 个人博客
```json
{
  "appName": "我的博客",
  "packageId": "com.myblog.app",
  "appUrl": "https://myblog.com",
  "allowedDomains": ["myblog.com"]
}
```

### 企业官网
```json
{
  "appName": "公司官网",
  "packageId": "com.company.official",
  "appUrl": "https://www.company.com",
  "allowedDomains": ["company.com", "api.company.com"]
}
```

### GitHub Pages
```json
{
  "appName": "My Portfolio",
  "packageId": "com.github.user.portfolio",
  "appUrl": "https://user.github.io",
  "allowedDomains": ["github.io", "githubusercontent.com"]
}
```

## 🎯 工作流程 / Workflow

```
┌──────────────┐
│ 编辑配置文件 │ app-config.json
└──────┬───────┘
       │
       ▼
┌──────────────┐
│ 运行构建命令 │ bun run build:app
└──────┬───────┘
       │
       ▼
┌──────────────┐
│  获取 APK   │ 安装到手机
└──────────────┘
```

## 🔧 配置说明 / Configuration

### 必填字段

- **appName**: 应用名称（显示在手机上）
- **packageId**: 包名（唯一标识符，如 com.example.app）
- **appUrl**: 启动URL（应用加载的网址）
- **allowedDomains**: 允许的域名列表（其他域名会被拦截）

### 可选字段

- **versionName**: 版本号（留空自动生成）
- **icon**: 图标路径（留空使用默认图标）

详细说明请查看 [CONFIG_GUIDE.md](./CONFIG_GUIDE.md)

## 📋 系统要求 / Requirements

- [Bun](https://bun.sh) - JavaScript runtime
- JDK 11+ - Java开发工具包
- Android SDK - 通过Gradle自动下载

## 🤝 GitHub Actions

推送代码到 `main` 分支会自动触发构建：
- ✅ 自动构建APK
- ✅ 自动创建Release
- ✅ 自动上传APK文件

## ❓ 常见问题 / FAQ

### Q: 如何更改应用名称？
A: 修改 `app-config.json` 中的 `appName`，重新构建即可。

### Q: 如何允许多个域名？
A: 在 `allowedDomains` 数组中添加多个域名：
```json
"allowedDomains": ["example.com", "api.example.com", "cdn.example.com"]
```

### Q: 子域名需要单独添加吗？
A: 不需要。添加 `example.com` 会自动包含所有子域名。

### Q: 构建失败怎么办？
A: 检查：
1. 配置文件格式是否正确
2. 是否安装了所有依赖
3. 查看错误日志

更多问题请查看 [CONFIG_GUIDE.md](./CONFIG_GUIDE.md)

## 📊 项目统计 / Statistics

- ⚡ 配置步骤: **2步** (之前7步)
- 📝 需要修改的文件: **1个** (之前3+个)
- 🎯 代码量: **减少33%**
- ⏱️ 上手时间: **5分钟**

## 🎉 开始使用 / Get Started

1. 查看 [QUICKSTART.md](./QUICKSTART.md) 快速上手
2. 参考 [app-config.example.json](./app-config.example.json) 示例
3. 阅读 [CONFIG_GUIDE.md](./CONFIG_GUIDE.md) 了解详情
4. 运行 `bun run build:app` 构建应用

---

**5分钟从网站到APP！** 🚀

**From Website to App in 5 Minutes!** 🚀
