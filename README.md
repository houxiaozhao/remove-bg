# AI 图片背景移除工具

一个基于 Vue 3 + Vite 开发的在线图片背景移除工具，使用 AI 模型实现快速、高质量的背景移除。

## 主要功能

### 图片处理

- 支持单张或批量上传图片
- 使用 AI 模型自动移除图片背景
- 实时预览对比效果，支持滑动对比原图和处理后的图片
- 支持拖拽上传图片

### 图片管理

- 图片列表显示，包含文件名和大小信息
- 支持删除单张图片
- 一键清空所有图片
- 支持一键导出所有处理完成的图片
- 处理状态实时显示

## 技术特点

- 使用 Vue 3 + Vite 构建，提供现代化的开发体验
- 采用 Web Worker 处理图片，保证主线程流畅运行
- 使用 HuggingFace 的 RMBG-1.4 模型进行背景移除
- 响应式设计，支持各种屏幕尺寸

## 使用说明

1. 上传图片：

   - 点击上传区域选择图片
   - 或直接拖拽图片到上传区域

2. 图片处理：

   - 上传后自动开始处理
   - 处理过程中显示加载动画
   - 完成后可在预览区查看效果

3. 图片管理：
   - 点击图片列表中的图片可切换预览
   - 点击图片右侧的删除按钮可删除单张图片
   - 使用顶部的"清空"按钮可删除所有图片
   - 使用"导出全部"按钮可下载所有处理完成的图片

## 开发环境设置

```bash
# 安装依赖
npm install

# 启动开发服务器
npm run dev

# 构建生产版本
npm run build
```

## 注意事项

- 首次加载需要下载 AI 模型，请耐心等待
- 模型加载完成前无法选择和处理图片
