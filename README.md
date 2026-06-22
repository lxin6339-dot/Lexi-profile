# -Lexi-s-profile
曾参与多项节目，担任导演、策划、撰稿等职务。具备直播、晚会、短视频等多类型内容执行经验。 注重创意与落地的结合，擅长在项目中承担多重角色。
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>个人作品集 | 你的名字</title>
    <!-- 字体图标库 Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
    <style>
        /* ===== 全局重置 & 基础 ===== */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Roboto, system-ui, -apple-system, sans-serif;
            background: #0f0f1a;
            color: #eaeef2;
            line-height: 1.6;
            padding: 2rem 1rem;
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
        }

        /* ===== 卡片通用 ===== */
        .card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(8px);
            -webkit-backdrop-filter: blur(8px);
            border: 1px solid rgba(255, 255, 255, 0.08);
            border-radius: 28px;
            padding: 2rem 2.2rem;
            box-shadow: 0 20px 40px -12px rgba(0, 0, 0, 0.6);
            transition: transform 0.2s ease, border-color 0.2s;
        }

        .card:hover {
            border-color: rgba(255, 255, 255, 0.18);
            transform: translateY(-2px);
        }

        /* ===== 头部 / 头像区 ===== */
        .hero {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            gap: 2.5rem;
            margin-bottom: 3.5rem;
        }

        .avatar {
            width: 130px;
            height: 130px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid rgba(255, 255, 255, 0.15);
            box-shadow: 0 12px 28px -8px rgba(0, 0, 0, 0.5);
            background: #2a2a3e;
            flex-shrink: 0;
        }

        .hero-text h1 {
            font-size: 2.8rem;
            font-weight: 700;
            letter-spacing: -0.02em;
            background: linear-gradient(135deg, #f0e9ff, #b7a9ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .hero-text p {
            font-size: 1.2rem;
            color: #b0b8c8;
            margin-top: 0.3rem;
        }

        .hero-text .tagline {
            display: inline-block;
            margin-top: 0.6rem;
            background: rgba(255, 255, 255, 0.06);
            padding: 0.3rem 1.2rem;
            border-radius: 40px;
            font-size: 0.9rem;
            color: #c8d0e0;
            border: 1px solid rgba(255, 255, 255, 0.06);
        }

        /* ===== 社交链接 ===== */
        .social-links {
            display: flex;
            gap: 1.2rem;
            margin-top: 1.2rem;
            flex-wrap: wrap;
        }

        .social-links a {
            color: #b0b8c8;
            font-size: 1.5rem;
            transition: color 0.2s, transform 0.15s;
            display: inline-block;
        }

        .social-links a:hover {
            color: #b7a9ff;
            transform: scale(1.1);
        }

        /* ===== 网格布局 ===== */
        .grid-2 {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 2rem;
            margin: 2.5rem 0;
        }

        /* ===== 项目卡片 ===== */
        .project-item {
            background: rgba(255, 255, 255, 0.03);
            border-radius: 18px;
            padding: 1.5rem 1.8rem;
            border-left: 3px solid #7c6df0;
            transition: background 0.2s;
        }

        .project-item:hover {
            background: rgba(255, 255, 255, 0.06);
        }

        .project-item h3 {
            font-size: 1.3rem;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 0.6rem;
        }

        .project-item h3 i {
            color: #7c6df0;
            font-size: 1.1rem;
        }

        .project-item p {
            color: #b8c0d0;
            margin: 0.5rem 0 0.8rem;
            font-size: 0.98rem;
        }

        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-top: 0.6rem;
        }

        .project-tags span {
            background: rgba(124, 109, 240, 0.15);
            color: #c8c0f0;
            font-size: 0.75rem;
            padding: 0.2rem 0.9rem;
            border-radius: 30px;
            border: 1px solid rgba(124, 109, 240, 0.15);
        }

        .project-link {
            display: inline-block;
            margin-top: 0.9rem;
            color: #b7a9ff;
            text-decoration: none;
            font-weight: 500;
            font-size: 0.9rem;
            transition: color 0.2s;
        }

        .project-link i {
            font-size: 0.8rem;
            margin-left: 0.3rem;
            transition: transform 0.2s;
        }

        .project-link:hover {
            color: #d4caff;
        }
        .project-link:hover i {
            transform: translateX(4px);
        }

        /* ===== 技能标签 ===== */
        .skills-wrap {
            display: flex;
            flex-wrap: wrap;
            gap: 0.8rem;
            margin-top: 0.5rem;
        }

        .skills-wrap span {
            background: rgba(255, 255, 255, 0.06);
            padding: 0.4rem 1.2rem;
            border-radius: 40px;
            font-size: 0.9rem;
            border: 1px solid rgba(255, 255, 255, 0.04);
            color: #d0d8e8;
        }

        /* ===== 关于我 ===== */
        .about-text {
            color: #c8d0e0;
            font-size: 1.02rem;
            margin-top: 0.3rem;
        }

        /* ===== 联系区 ===== */
        .contact-row {
            display: flex;
            flex-wrap: wrap;
            gap: 1.5rem 3rem;
            margin-top: 0.8rem;
        }

        .contact-row a {
            color: #b7a9ff;
            text-decoration: none;
            font-size: 1rem;
            display: inline-flex;
            align-items: center;
            gap: 0.6rem;
            transition: color 0.2s;
        }

        .contact-row a:hover {
            color: #d4caff;
        }

        .contact-row i {
            font-size: 1.2rem;
            width: 1.6rem;
            text-align: center;
        }

        /* ===== 页脚 ===== */
        .footer {
            text-align: center;
            margin-top: 3.5rem;
            color: #5a6278;
            font-size: 0.9rem;
            border-top: 1px solid rgba(255, 255, 255, 0.04);
            padding-top: 2rem;
        }

        .footer a {
            color: #7c6df0;
            text-decoration: none;
        }

        /* ===== 响应式 ===== */
        @media (max-width: 760px) {
            .grid-2 {
                grid-template-columns: 1fr;
                gap: 1.5rem;
            }

            .hero {
                flex-direction: column;
                align-items: flex-start;
                gap: 1.2rem;
            }

            .hero-text h1 {
                font-size: 2.2rem;
            }

            .card {
                padding: 1.5rem 1.2rem;
            }

            .contact-row {
                flex-direction: column;
                gap: 0.8rem;
            }

            body {
                padding: 1rem 0.8rem;
            }
        }

        @media (max-width: 420px) {
            .hero-text h1 {
                font-size: 1.8rem;
            }
            .avatar {
                width: 100px;
                height: 100px;
            }
        }
    </style>
</head>
<body>

    <div class="container">

        <!-- ===== 头部 ===== -->
        <header class="hero">
            <!-- 头像：替换 src 为你自己的图片链接 -->
            <img class="avatar" src="https://api.dicebear.com/7.x/avataaars/svg?seed=Felix" alt="头像" />
            <div class="hero-text">
                <h1>你好，我是 Felix</h1>
                <p>全栈开发 · 创意编程 · 设计爱好者</p>
                <span class="tagline"><i class="fas fa-map-pin" style="margin-right: 6px;"></i>基于 GitHub Pages 的作品集</span>

                <div class="social-links">
                    <a href="#" aria-label="GitHub"><i class="fab fa-github"></i></a>
                    <a href="#" aria-label="掘金"><i class="fab fa-js-square"></i></a>
                    <a href="#" aria-label="Twitter"><i class="fab fa-twitter"></i></a>
                    <a href="#" aria-label="LinkedIn"><i class="fab fa-linkedin-in"></i></a>
                    <a href="#" aria-label="邮箱"><i class="fas fa-envelope"></i></a>
                </div>
            </div>
        </header>

        <!-- ===== 网格：关于 + 技能 ===== -->
        <div class="grid-2">
            <!-- 关于我 -->
            <section class="card">
                <h2 style="font-weight: 600; font-size: 1.5rem; margin-bottom: 0.8rem;">
                    <i class="fas fa-user-astronaut" style="color: #7c6df0; margin-right: 10px;"></i>关于我
                </h2>
                <div class="about-text">
                    <p>热爱将创意转化为代码，喜欢探索前沿技术并构建实用的产品。</p>
                    <p style="margin-top: 0.8rem;">目前专注于 <strong style="color: #e0e8f8;">React</strong>、<strong style="color: #e0e8f8;">Node.js</strong> 和 <strong style="color: #e0e8f8;">TypeScript</strong>，同时保持对 UI/UX 的敏锐感知。</p>
                    <p style="margin-top: 0.8rem;">✨ 相信好的设计能让技术更有温度。</p>
                </div>
            </section>

            <!-- 技能 -->
            <section class="card">
                <h2 style="font-weight: 600; font-size: 1.5rem; margin-bottom: 0.8rem;">
                    <i class="fas fa-code" style="color: #7c6df0; margin-right: 10px;"></i>技术栈
                </h2>
                <div class="skills-wrap">
                    <span>React</span>
                    <span>Vue</span>
                    <span>TypeScript</span>
                    <span>Node.js</span>
                    <span>Python</span>
                    <span>Tailwind</span>
                    <span>Figma</span>
                    <span>Git</span>
                    <span>Docker</span>
                    <span>MongoDB</span>
                </div>
                <p style="color: #8a92a8; margin-top: 1rem; font-size: 0.9rem;">
                    <i class="fas fa-rocket" style="margin-right: 6px;"></i>持续学习，不断迭代
                </p>
            </section>
        </div>

        <!-- ===== 项目展示 ===== -->
        <section class="card" style="margin: 2rem 0;">
            <h2 style="font-weight: 600; font-size: 1.6rem; margin-bottom: 1.8rem;">
                <i class="fas fa-folder-open" style="color: #7c6df0; margin-right: 12px;"></i>精选项目
            </h2>

            <div class="grid-2" style="margin-top: 0;">
                <!-- 项目 1 -->
                <div class="project-item">
                    <h3><i class="fas fa-cloud-moon"></i> 天气可视化</h3>
                    <p>基于 OpenWeatherMap API 的实时天气仪表板，包含动态图表和 7 日预报。</p>
                    <div class="project-tags">
                        <span>React</span>
                        <span>Chart.js</span>
                        <span>REST API</span>
                    </div>
                    <a href="#" class="project-link">查看项目 <i class="fas fa-arrow-right"></i></a>
                </div>

                <!-- 项目 2 -->
                <div class="project-item">
                    <h3><i class="fas fa-robot"></i> 智能助手 Bot</h3>
                    <p>基于 GPT 的 Telegram 机器人，支持多轮对话、任务提醒和趣味问答。</p>
                    <div class="project-tags">
                        <span>Node.js</span>
                        <span>OpenAI</span>
                        <span>Telegram API</span>
                    </div>
                    <a href="#" class="project-link">查看项目 <i class="fas fa-arrow-right"></i></a>
                </div>

                <!-- 项目 3 -->
                <div class="project-item">
                    <h3><i class="fas fa-palette"></i> 设计系统库</h3>
                    <p>可复用的 UI 组件库，包含 30+ 原子组件，支持暗色模式和主题定制。</p>
                    <div class="project-tags">
                        <span>Vue</span>
                        <span>Storybook</span>
                        <span>CSS Variables</span>
                    </div>
                    <a href="#" class="project-link">查看项目 <i class="fas fa-arrow-right"></i></a>
                </div>

                <!-- 项目 4 -->
                <div class="project-item">
                    <h3><i class="fas fa-chart-line"></i> 个人看板</h3>
                    <p>极简风格的任务管理面板，支持拖拽、标签过滤和进度追踪。</p>
                    <div class="project-tags">
                        <span>React</span>
                        <span>DnD</span>
                        <span>LocalStorage</span>
                    </div>
                    <a href="#" class="project-link">查看项目 <i class="fas fa-arrow-right"></i></a>
                </div>
            </div>

            <!-- 更多项目链接 -->
            <div style="text-align: center; margin-top: 0.8rem;">
                <a href="#" style="color: #7c6df0; text-decoration: none; font-weight: 500;">
                    <i class="fas fa-arrow-right" style="margin-right: 6px;"></i>在 GitHub 上查看更多
                </a>
            </div>
        </section>

        <!-- ===== 联系 ===== -->
        <section class="card">
            <h2 style="font-weight: 600; font-size: 1.5rem; margin-bottom: 0.8rem;">
                <i class="fas fa-paper-plane" style="color: #7c6df0; margin-right: 12px;"></i>联系我
            </h2>
            <div class="contact-row">
                <a href="mailto:your.email@example.com"><i class="fas fa-envelope"></i> your.email@example.com</a>
                <a href="#"><i class="fab fa-github"></i> github.com/yourname</a>
                <a href="#"><i class="fab fa-twitter"></i> @yourhandle</a>
                <a href="#"><i class="fab fa-linkedin"></i> linkedin.com/in/yourname</a>
            </div>
            <p style="color: #7a8298; margin-top: 1.2rem; font-size: 0.95rem;">
                <i class="fas fa-comment-dots" style="margin-right: 8px;"></i>欢迎交流，一起创造有趣的东西！
            </p>
        </section>

        <!-- ===== 页脚 ===== -->
        <footer class="footer">
            <p>
                &copy; 2026 Felix · 用 <i class="fas fa-heart" style="color: #7c6df0; margin: 0 4px;"></i> 构建 ·
                托管于 <a href="https://pages.github.com/" target="_blank">GitHub Pages</a>
            </p>
            <p style="margin-top: 0.3rem; font-size: 0.8rem;">
                <i class="fas fa-code-branch"></i> 新手友好 · 快速定制
            </p>
        </footer>

    </div>

</body>
</html>
