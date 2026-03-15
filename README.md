# 种子文件转磁力链接工具

一个简单易用的种子文件转磁力链接工具，直接在浏览器中运行，无需安装任何软件。

## 功能特性

- 📁 **拖放上传**：支持直接拖放种子文件到页面
- 📦 **批量处理**：可同时处理多个种子文件
- 🌐 **语言切换**：支持中文和英文界面
- 📊 **进度显示**：实时显示转换进度
- 📋 **一键复制**：支持复制单个或所有磁力链接
- 📱 **响应式设计**：适配不同屏幕尺寸（电脑、手机、平板）
- 🔒 **本地处理**：所有文件在浏览器本地解析，不会上传到服务器

## 如何使用

### 直接访问

访问已部署的网站：https://your-domain.vercel.app

### 本地运行

1. 克隆或下载项目
2. 直接在浏览器中打开 `index.html` 文件
3. 或者使用本地服务器：

```bash
python3 -m http.server 8000
# 然后访问 http://localhost:8000
```

### 部署到 Vercel

1. 安装 Vercel CLI：

```bash
npm i -g vercel
```

2. 部署项目：

```bash
cd vercel-deploy
vercel
```

## 技术说明

### 磁力链接格式

```
magnet:?xt=urn:btih:<INFO_HASH>&dn=<DISPLAY_NAME>&tr=<TRACKERS>&xl=<FILE_SIZE>
```

- `xt` - 实体类型（URN）
- `btih` - BitTorrent Info Hash（SHA-1 哈希）
- `dn` - 显示名称（URL 编码）
- `tr` - Tracker 地址（URL 编码）
- `xl` - 文件大小（字节）

### 浏览器兼容性

- Chrome 60+
- Firefox 55+
- Safari 11+
- Edge 79+

## 许可证

本项目仅供个人使用。如有商业用途，请遵守相关版权法律。
