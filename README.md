# YoYoung Shorts 优扬短剧

![YoYoung Shorts Logo](./assets/logo/logo-wordmark-horizontal.png)

> 由一名独立开发者持续构建。目前还在首尾打磨阶段，暂不开放相关源码；后续会在产品成熟后，考虑开放部分基础能力展示版。

从一句想法开始，自动组织分镜脚本、连续图片与视频结果。

YoYoung Shorts 优扬短剧不是单点模型入口，也不是把几个接口拼在一起的壳。它更像一套把角色、场景、道具、分镜脚本、图片和视频串成连续工作流的 AI 短剧工作台，让不会写复杂提示词的人也能更快开始创作。

如果你想看更完整的功能拆解，可以继续看 [FEATURES.md](./FEATURES.md)。  
如果你想看更聚焦的案例说明，可以继续看 [CASES.md](./CASES.md)。

## 下载本地体验包

想先在自己的电脑上看一看产品形态？可以下载 Docker/DACKER 本地体验包。

这个包适合用来快速体验优扬短剧的界面、创作入口和工作流结构：从一个想法开始，进入脚本、图片、视频相关流程，而不是一上来研究复杂提示词或接口配置。

- 下载入口：[v0.1.1 Docker/DACKER Thin 本地软件包](https://github.com/rolfie-han/yoyoung-shorts/releases/tag/v0.1.1-docker-thin-public-clean)
- 下载文件：`docker-local-package-thin-bundle.zip`
- 适合人群：想体验产品形态的创作者、技术用户、合作方或早期试用用户
- 当前定位：本地体验包 / 技术预览包，不是完整源码自部署版

### 小白怎么开始

1. 先安装并启动 Docker Desktop 或 DACKER。
2. 在 Release 页面下载 `docker-local-package-thin-bundle.zip`。
3. 解压后，把 `.env.example` 复制一份并改名为 `.env`。
4. 在 `.env` 里填写官方提供的 `CLOUD_BACKEND_ORIGIN`，必要时修改 `LOCAL_WEB_PORT`。
5. 在解压目录运行 `docker compose up -d --build`，然后打开 `http://127.0.0.1:<LOCAL_WEB_PORT>`。

如果你只是想先了解产品能力，可以直接看下面的截图、案例和演示视频；如果你想实际跑起来，请优先使用 Release 里的本地体验包。

## 为什么这个仓库值得关注

- 这不是“又一个套模型接口的壳”，而是一套围绕真实创作流程组织出来的短剧工作台
- 它的重点不是教用户写复杂提示词，而是让用户先说想法，再逐步推进成脚本、图片和视频
- 单图、多图叙事、分镜脚本、视频和历史记录之间是连着的，不是彼此割裂的几个页面
- 角色、场景、道具会持续参与生成流程，这让结果更像在“创作”，而不是在“抽卡”
- 这是一个独立开发者长期打磨的产品，后续还会继续公开更多案例和演进方向

## 核心价值

- 不是“填一段提示词出一张图”的单点工具，而是从一句想法继续推进到脚本、图片和视频的连续创作工作台
- 不会写复杂提示词也能开始：先说想法，再进入创作流程，而不是先做提示词工程
- 图片一致性不是单点偶然结果：单图、多图叙事、分镜脚本共用同一条连续创作链
- 资产中心不是摆设：角色、场景、道具会持续参与后续生成，而不是一次性描述
- 结果不是一次性的：图片和视频会沉淀到历史记录里，便于回看、比较和继续延展

## 它和常见同类工具的差别

- 很多工具更像模型入口，YoYoung Shorts 更像创作工作台
- 很多工具要求用户先写好提示词，这里更强调“先有想法，再逐步组织”
- 很多工具的图片是孤立结果，这里更强调角色、场景、道具和分镜的连续关系
- 很多工具停在图片层，这里会继续把脚本和图片推进到视频结果
- 很多工具的结果生成完就结束，这里会继续沉淀到历史记录里复用

## 它最适合谁

- 想做短剧、动画短片、故事化内容，但不会写复杂提示词的人
- 需要把一个灵感持续推进成多张连续画面，而不是只要一张封面图的人
- 希望角色、场景、道具在后续阶段还能继续被引用和延续的人
- 不满足于“出图即结束”，还想继续推进成视频结果的人

## Hero

![YoYoung Shorts overview](./assets/hero/hero-overview-main.png)

这张总览图本身就能说明：这不是单点工具，而是一条从多图叙事推进到视频结果的连续工作流。

## 功能区与能力说明

### Create：从一句想法开始

Create 更像创作入口，而不是提示词工程入口。用户先输入一个想法，再把它推进到图片、分镜脚本和视频流程里。

![Create with anchored assets](./assets/showcases/showcase-create-single-image-with-assets.png)

### Assets：角色、场景、道具作为锚点

资产中心不是装饰，而是工作流里的锚点系统。角色、场景、道具会在后续单图、多图、分镜脚本和视频阶段持续进入生成链。

![Assets as anchors across the workflow](./assets/showcases/showcase-assets-anchor-system.png)

### Story：多图叙事不是重复同一张图

多图叙事的重点不是多出几张图，而是把同一个剧情段落组织成连续画面，保留角色关系、场景氛围和动作推进感。

![Multi-frame story consistency](./assets/showcases/showcase-story-multi-frame-consistency.png)

### History：结果沉淀与复用

历史记录不仅是归档区，也是在公开展示里解释“连续创作”和“结果可复用”的最好证据。单角色一致性、同一主题的连续画面，都能在这里直接看出来。

![Single character consistency history](./assets/cases/case-single-character-consistency-history.png)

## 脚本与视频工作流

分镜脚本不是终点，它可以继续连接图片与视频，形成完整创作闭环。

### 1. 分镜脚本到视频结果

这张图最适合说明：脚本、镜头描述和视频结果是可以同屏衔接的，而不是写完脚本就结束。

![Storyboard to video workflow](./assets/showcases/showcase-script-to-video.png)

### 2. 视频生成功能区

这里展示的是视频功能区本身。它承接前面的图片和提示，把静态结果继续推进到视频阶段。

![Video generation workbench](./assets/showcases/showcase-video-workbench.png)

### 3. 脚本、视频与音频工作区

这一块更像“完整工作台”的证明图，说明产品不是只停留在单一结果页，而是有继续编辑和串联的空间。

![Storyboard, video, and audio workbench](./assets/showcases/showcase-script-video-audio-workbench.png)

### 4. 历史结果沉淀与复用

图片和视频结果都能沉淀进历史记录，方便回看、比较和继续延展。这也是为什么它更像一套创作系统，而不是一次性工具。

![History and reuse](./assets/cases/case-single-character-consistency-history.png)

## Demo Videos

相比 GIF，短视频更适合展示这类连续工作流，也更清楚。

GitHub 对仓库里的 mp4 内联预览支持并不总是理想，所以这里把视频当作“补充演示材料”，核心说明仍然放在截图和文字结构里。后续会考虑补更顺手的在线演示方式，让浏览体验更完整。

- [一句想法 -> 分镜脚本](./assets/videos/demo-idea-to-script.mp4)
- [资产中心 -> 多图叙事](./assets/videos/demo-assets-to-story.mp4)
- [分镜脚本 -> 视频结果](./assets/videos/demo-script-to-video.mp4)

## Built Independently

YoYoung Shorts 优扬短剧由独立开发者持续构建和迭代。重点不是堆模型数量，而是把真实创作过程组织成更顺畅的工作流。

> Built independently by a solo developer, and continuously refined around real creative workflows.
>
> The source code is not open at this stage. When the product is more mature, a limited basic edition may be opened for community showcase.

## Roadmap

- 持续强化图片一致性体验
- 持续优化分镜脚本组织能力
- 持续提升图片到视频的工作流闭环
- 持续打磨角色、场景、道具的资产化逻辑
- 在产品成熟后，视情况开放部分基础能力展示给社区

## 加入测试群

如果你已经下载了本地体验包，或者想先看看后续更新、反馈体验问题，可以扫码加入测试群。

群里会优先同步：

- 本地体验包更新
- 使用问题和排障说明
- 新功能演示和测试反馈
- 后续体验名额和交流信息

> 二维码 7 天内有效，过期后会更新。

<img src="./assets/community/wechat-test-group-2026-05-01.png" alt="优扬短剧测试群二维码" width="360" />
