# personalGpt

personalGpt 是一个基于 GPT-3.5-Turbo 模型的交互式网站项目，使用 Next.js 框架构建，使用 Vercel 云平台部署，是一个纯前端的轻量级应用，供自己使用chatGpt使。

Github 代码库: https://github.com/riwigefi/light-gpt

演示站点: https://wu-gpt.vercel.app/  (需要科学上网)

## 功能

1. 纯前端应用，基于 GPT-3.5-Turbo 模型，使用 API KEY 在前端请求 OpenAI 的对话接口，支持流式数据，页面以打字机效果显示机器人回复。
2. 部署后，用户在前端页面设置自己的 API KEY，科学上网的情况下，问答速度会很快。用户设置的 API KEY 将保存在客户端，完全没有泄漏风险。
3. 支持新的主题对话和查看历史主题对话。所有对话数据都存储在浏览器的 IndexedDB 中，也就是说对话数据记录是保存在本地的，不会有数据泄漏风险。
4. AI 回复支持多种语法高亮和一键复制代码功能，针对编程相关问题。对话支持图片和 PDF 导出。
5. 应用适配了 PC 和 Mobile 设备，方便使用。
6. 支持 DIY，支持设置用户头像和 AI 头像。
## 本地部署

要在本地部署 Light-GPT，按照以下步骤操作(需要 node16 及以上版本)：

1. 将项目下载到本地:

```bash
git clone https://github.com/riwigefi/light-gpt.git
```

2. 进入项目目录并安装依赖项:

```bash
cd light-gpt
pnpm install
```

3. 启动应用程序:

```bash
pnpm run dev
```

这样，项目就能在 http://localhost:3000 上预览了。在前端页面输入你的 API KEY，就可以愉快对话了。

## Vercel 线上部署

1. 注册一个 Vercel 云平台部署账号，访问 https://vercel.com
2. 登录 Vercel 平台，点击 "Add New"，选择 "Project"，将该项目进行部署

## 重要提示

**本地部署时，由于 OpenAi 风控政策，请务必保证你是科学上网环境，你可以正常访问 open ai 官网，如果不能，请不要设置 api key 进行调试，否则会有异常风险**
