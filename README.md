# OpenShortVideo - AI短视频生成平台

## 代码近期会开源，有想法的可以进行交流

## 📖 项目概述

**OpenShortVideo** 是一个基于AI的短视频智能制作平台，集成了剧本创作、角色管理、场景生成、镜头制作等完整的工作流，帮助创作者快速生成高质量的短视频内容。
## demo
[openshortvideo.mp4](assert/openshortvideo.mp4)
## ✨ 核心功能

### 🎬 智能视频制作
- **一键生成**：输入简单描述，AI自动生成完整短视频
- **分步生成**：按剧本→角色→场景→镜头的流程精细化制作
- **实时预览**：生成过程中实时查看进度和预览效果

### 👥 角色管理
- **AI角色生成**：自动生成角色形象和特征
- **多角度肖像**：支持正面、侧面、背面全方位展示
- **批量管理**：支持批量导入、编辑和删除角色

### 🎨 场景与镜头
- **智能分镜**：AI分析剧本自动分镜
- **场景管理**：多场景切换和配置
- **镜头预览**：实时查看镜头效果和描述

### 🤖 AI助手
- **灵犀Agent**：智能对话助手，辅助创意构思
- **Prompt优化**：智能提示词生成和优化
- **内容扩展**：基于输入内容自动扩展创意

## 🛠️ 技术栈

### 后端 (Backend)
- **框架**：Python Flask
- **数据库**：SQLAlchemy + SQLite
- **AI集成**：大语言模型API集成
- **文件存储**：本地文件系统 + 上传管理
- **API设计**：RESTful API架构

### 前端 (Frontend)
- **基础框架**：HTML5 + CSS3 + JavaScript
- **UI组件**：自定义CSS + Font Awesome图标
- **交互框架**：jQuery + 原生JavaScript
- **布局系统**：Flexbox + CSS Grid
- **响应式设计**：移动端适配

## 📂 项目结构

```
OpenShortVideo_V3/
├── backend/                 # 后端代码
│   ├── api_v1.py           # API路由定义
│   ├── models.py           # 数据模型
│   ├── routes/             # 路由模块
│   │   ├── characters.py   # 角色管理路由
│   │   └── ...             # 其他路由
│   └── utils/              # 工具函数
│
├── frontend/               # 前端代码
│   ├── templates/          # HTML模板
│   │   ├── layout.html     # 基础布局
│   │   ├── dashboard.html  # 首页仪表板
│   │   ├── projects.html   # 项目管理
│   │   ├── project_detail.html # 项目详情
│   │   ├── episode_generate.html # 视频生成页面
│   │   ├── create_project.html  # 创建项目
│   │   ├── ai_dialogue_demo2.html # AI助手页面
│   │   └── ...             # 其他模板
│   │
│   ├── static/             # 静态资源
│   │   ├── css/            # 样式文件
│   │   ├── js/             # JavaScript文件
│   │   └── images/         # 图片资源
│   │
│   └── uploads/            # 用户上传文件
│
├── assert/                 # 项目示例图片
│   ├── QQ.png             # 联系QQ
│   ├── 一键生成页面.jpg    # 一键生成界面示例
│   ├── 发现页面.jpg       # 发现页面示例
│   ├── 教程.jpg          # 教程页面示例
│   ├── 新建项目.jpg       # 新建项目界面示例
│   ├── 项目详情.jpg       # 项目详情界面示例
│   └── 首页.jpg          # 首页仪表板示例
│
├── requirements.txt        # Python依赖包
├── config.py              # 配置文件
└── README.md              # 项目文档
```

## 🚀 快速开始

### 环境要求
- Python 3.8+
- Node.js (可选，用于前端开发)
- 现代浏览器 (Chrome 90+, Firefox 88+, Edge 90+)

### 安装步骤

1. **克隆项目**
   ```bash
   git clone <repository-url>
   cd openshortvideo_v3
   ```

2. **安装Python依赖**
   ```bash
   pip install -r requirements.txt
   ```

3. **配置环境变量**
   ```bash
   cp config.example.py config.py
   # 编辑config.py，配置数据库和API密钥
   ```

4. **初始化数据库**
   ```bash
   python -c "from backend.models import db; db.create_all()"
   ```

5. **启动后端服务**
   ```bash
   cd backend
   python app_service.py
   或
   start_service.bat
   ```

6. **访问前端**
   ```bash
   cd fronten
   python app_webui.py
   或
   start_ui.bat
   ```
   打开浏览器访问 `http://localhost:5000`

## 📱 界面展示

### 🏠 首页仪表板 (`assert/home.jpg`)
![home](assert/home.jpg)
- 项目概览和快速访问
- 最近项目展示
- 数据统计和进度跟踪

### 📁 项目管理 (`assert/project_details.jpg`)
![project_details](assert/project_details.jpg)
- 项目列表和筛选
- 封面图片展示和缩放
- 项目状态管理（草稿/进行中/已完成）

### 🎬 一键生成 (`assert/One_click_page_generation.jpg`)
![One_click_page_generation](assert/One_click_page_generation.jpg)
- 智能视频生成工作流
- 实时生成进度监控
- 镜头预览和编辑

### 🤖 AI助手 (`assert/agent.jpg`)
- 智能对话界面
- 创意灵感激发
- 多模态输入支持（文本、图片等）

### 📝 新建项目 (`assert/NewProject.jpg`)
- 项目基本信息配置
- 封面图片上传
- 角色生成选项设置

### 🌐 发现页面 (`assert/DiscoveryPage.jpg`)
- 社区作品展示
- 热门模板推荐
- 趋势分析

### 📚 教程页面 (`assert/教程.jpg`)
- 使用指南和教程
- 最佳实践案例
- 常见问题解答

## 🔧 配置文件

### 数据库配置
```python
# config.py
SQLALCHEMY_DATABASE_URI = 'sqlite:///openshortvideo.db'
SQLALCHEMY_TRACK_MODIFICATIONS = False
```

### API配置
```python
# AI服务配置
AI_API_KEY = 'your-api-key-here'
AI_BASE_URL = 'https://api.example.com'
```

### 上传配置
```python
UPLOAD_FOLDER = 'frontend/uploads'
MAX_CONTENT_LENGTH = 16 * 1024 * 1024  # 16MB
```

## 📊 数据模型

### 主要数据表
1. **User** - 用户信息
2. **Project** - 项目信息
3. **Character** - 角色信息
4. **Episode** - 分集信息
5. **Scene** - 场景信息
6. **Shot** - 镜头信息

## 🔌 API接口

### 项目管理
- `GET /api/projects` - 获取项目列表
- `POST /api/projects` - 创建新项目
- `GET /api/projects/{id}` - 获取项目详情
- `PUT /api/projects/{id}` - 更新项目
- `DELETE /api/projects/{id}` - 删除项目

### 视频生成
- `POST /api/episodes/{id}/generate` - 开始生成视频
- `GET /api/episodes/{id}/status` - 获取生成状态
- `POST /api/episodes/{id}/stop` - 停止生成

### 角色管理
- `GET /api/characters` - 获取角色列表
- `POST /api/characters` - 创建角色
- `DELETE /api/characters/{id}` - 删除角色

### 文件管理
- `GET /api/v1/generate/files` - 获取文件列表
- `GET /api/v1/generate/file` - 获取文件内容

## 🎨 前端特性

### 响应式布局
- 桌面端优化布局
- 移动端适配设计
- 多种屏幕尺寸支持

### 交互体验
- 图片预览和缩放
- 实时状态更新
- 拖拽上传支持
- 模态框和提示

### 视觉效果
- 渐变背景和阴影
- 动画过渡效果
- 图标字体集成
- 自定义滚动条

## 🤝 贡献指南

1. Fork 本项目
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 📞 联系方式

- **邮箱**: 854197093@qq.com
- **技术交流群**: 1029629549

## 🙏 致谢

感谢以下开源项目和服务的支持：
- Flask - Python Web框架
- SQLAlchemy - ORM工具
- Font Awesome - 图标库
- 各大AI服务提供商

---

**注意**: 本项目正在积极开发中，部分功能可能还在完善中。欢迎反馈和建议！