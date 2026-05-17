# AI Restaurant Demo - Smart Dining Assistant

一个展示 AI 智能点餐能力的演示应用，专为传音控股海外国家 CEO 面试准备。

## 功能亮点

- 🤖 **AI 智能推荐** - 基于场景化对话推荐菜品（预算、口味、人数、宗教禁忌）
- 🎙️ **语音点餐** - 中英双语语音识别与合成
- 📱 **移动端适配** - 完美适配手机屏幕，像真实小程序
- 🌍 **非洲本地化** - 尼日利亚拉各斯餐厅场景，清真、辣味、传统菜品
- 🛒 **完整购物车** - 添加、修改数量、结算流程

## 技术栈

- 纯前端 HTML/CSS/JS
- Tailwind CSS (CDN)
- Web Speech API (免费语音)
- Moonshot AI API (智能推荐，可选)

## 部署方式

### 方式一：Vercel 部署（推荐）

1. 将本项目推送到 GitHub
2. 登录 [vercel.com](https://vercel.com)，用 GitHub 账号登录
3. 点击 "New Project"，选择本仓库
4. 点击 "Deploy"，等待 1-2 分钟
5. 获得 `https://your-project.vercel.app` 链接

### 方式二：静态托管

将 `index.html` 上传到任何静态托管服务：
- GitHub Pages
- Netlify
- Cloudflare Pages

### 方式三：本地预览

双击 `index.html` 用浏览器打开即可。

## 配置 AI 功能（可选）

默认使用规则引擎推荐，无需 API Key 即可运行。

如需接入 Moonshot AI 获得更智能的推荐：

1. 访问 [platform.moonshot.cn](https://platform.moonshot.cn) 注册账号
2. 创建 API Key
3. 编辑 `index.html`，找到 `CONFIG` 对象，填入：
   ```javascript
   const CONFIG = {
       API_KEY: 'your-api-key-here',
       // ...
   };
   ```

## 演示场景

1. **预算推荐** - "我预算有限，推荐便宜的"
2. **口味推荐** - "我想吃辣的"
3. **宗教禁忌** - "我需要清真食品"
4. **多人聚餐** - "我们三个人，推荐适合聚餐的"
5. **语音点餐** - 长按麦克风按钮说话

## 项目结构

```
ai-restaurant-demo-static/
├── index.html      # 主应用（单文件）
└── README.md       # 说明文档
```

## 面试展示建议

1. 开场介绍定位："这是一个面向非洲市场的 AI 点餐助手 Demo"
2. 展示语音点餐：体现多语言、低识字率场景价值
3. 展示智能推荐：体现 AI 对本地需求的理解
4. 强调本地化：清真、辣味、传统非洲菜品
5. 提及可扩展性：可接入真实餐厅 API、支付系统
