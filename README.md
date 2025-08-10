# 🏆 提成系统

一个现代化的员工提成管理系统，支持提成计算、数据统计和炫酷排行榜功能。

## ✨ 功能亮点

### 📊 提成计算
- 基于ROI的智能提成计算
- 实时数据同步
- 历史数据查询和筛选
- 月度统计报告

### 🏆 排行榜系统
- 实时提成排行
- 炫酷的动效UI设计
- 专属称号系统
- 完美的移动端适配

### 📱 移动端优先
- 响应式设计
- 触摸友好的交互
- 60fps流畅动画

## 🚀 快速开始

### 前置条件
- Node.js 16+
- npm 或 yarn
- Supabase账户

### 安装和运行

```bash
# 1. 克隆仓库或下载代码
git clone https://github.com/你的用户名/commission-system.git
cd commission-system

# 2. 安装依赖
npm install

# 3. 启动开发服务器
npm run dev
```

访问 http://localhost:5173 开始使用！

## 🌐 Netlify 部署

### 方法一：自动部署（推荐）

1. **将代码推送到 GitHub**
2. **登录 Netlify** (https://netlify.com)
3. **连接 GitHub 仓库**：
   - 点击 "New site from Git"
   - 选择 GitHub
   - 选择你的仓库
4. **部署设置：**
   - Build command: `npm run build`
   - Publish directory: `dist`
   - 点击 "Deploy site"

### 方法二：CLI 部署

```bash
# 安装 Netlify CLI
npm install -g netlify-cli

# 登录 Netlify
netlify login

# 构建项目
npm run build

# 部署
netlify deploy --prod --dir=dist
```

### 自动配置
项目已包含 `netlify.toml` 配置文件，支持：
- ✅ 自动构建配置
- ✅ SPA 路由重定向
- ✅ 缓存优化
- ✅ Node.js 18 环境

## 📆 提成规则

| ROI范围 | 单价提成 | 显示状态 |
|---------|----------|----------|
| ROI ≥ 1.0 | 7元/单 | 🟢 正常 |
| 0.8 ≤ ROI < 1.0 | 5元/单 | 🟡 一般 |
| ROI < 0.8 | 0元/单 | 🔴 跑了个锤子 |

## 🏅 排行榜称号

| 排名 | 称号 | 特权 |
|------|------|------|
| 🥇 第一名 | 游艇会黑金卡 | 顶级会员待遇 |
| 🥈 第二名 | 阳光国会黑金卡 | 高级会员待遇 |
| 🥉 第三名 | 黑灯舞黑金卡 | 公司提供免费体检一次 |

## 📁 项目结构

```
src/
├── components/          # React组件
│   ├── CommissionRanking.jsx    # 排行榜组件
│   ├── CommissionSystem.jsx     # 提成系统
│   └── Navigation.jsx           # 导航组件
├── data/               # 数据服务
├── utils/              # 工具库
└── styles/             # 样式文件
```

## 🔧 技术栈

- **前端**: React 18 + Vite + Tailwind CSS
- **后端**: Supabase (PostgreSQL + Auth + Storage)
- **动画**: CSS3 + Framer Motion
- **部署**: Netlify

## 🔧 开发脚本

```bash
# 开发模式
npm run dev

# 构建生产版本
npm run build

# 预览构建结果
npm run preview

# 代码检查
npm run lint
```

## 🌟 特性展示

### 炫酷排行榜
- 奖牌闪烁效果
- 排名数字跳动动画
- 悬停光晕特效
- 称号渐变动画

### 数据实时同步
- 自动刷新机制
- 手动刷新按钮
- 数据更新时间显示

### 响应式设计
- 移动端优先
- 适配所有屏幕尺寸
- 触摸友好交互

## 📝 许可证

MIT License - 详情查看 [LICENSE](LICENSE) 文件

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📞 支持

如有问题，请创建 Issue 或联系开发团队。

---

⭐ 如果这个项目对你有帮助，请给个 Star！
