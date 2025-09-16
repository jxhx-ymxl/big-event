<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <title>大事件 (Big Event) - 项目说明</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <style>
        body {
            background: #f8f8fb;
            font-family: 'Segoe UI', 'PingFang SC', 'Hiragino Sans GB', Arial, sans-serif;
            color: #222;
            margin: 0;
        }
        .container {
            max-width: 800px;
            margin: 40px auto 40px auto;
            padding: 32px 28px 28px 28px;
            background: #fff;
            border-radius: 18px;
            box-shadow: 0 4px 32px 0 rgba(60, 60, 110, 0.08);
        }
        h1 {
            text-align: center;
            margin-bottom: 8px;
            font-size: 2.5rem;
            color: #2563eb;
            letter-spacing: 2px;
        }
        h2 {
            margin-top: 38px;
            font-size: 1.5rem;
            color: #084fa1;
            border-bottom: 2px solid #e7eaf3;
            padding-bottom: 6px;
        }
        h3 {
            margin-top: 22px;
            color: #2d3748;
            font-size: 1.15rem;
        }
        ul, ol {
            margin-left: 22px;
            margin-bottom: 16px;
        }
        ul li {
            margin-bottom: 7px;
            list-style: disc;
        }
        pre, code {
            background-color: #f3f6fa;
            color: #2563eb;
            border-radius: 6px;
            padding: 6px 10px;
            font-size: 1em;
            word-break: break-all;
            font-family: 'Fira Mono', 'Consolas', monospace;
        }
        pre {
            overflow-x: auto;
        }
        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 16px;
            margin: 15px 0 0 0;
        }
        .tech-item {
            background: #f1f5fa;
            color: #2563eb;
            font-weight: 500;
            border-radius: 7px;
            padding: 7px 16px;
            font-size: 1em;
            margin-bottom: 7px;
            border: 1px solid #e6eefc;
        }
        .env-setup, .repo-info {
            margin-top: 12px;
        }
        a {
            color: #2563eb;
            text-decoration: none;
            border-bottom: 1px dotted #2563eb;
            transition: color 0.15s;
        }
        a:hover {
            color: #1741a7;
            border-bottom: 1px solid #1741a7;
        }
        .btn {
            display: inline-block;
            padding: 7px 18px;
            background: #2563eb;
            color: #fff;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 600;
            margin: 6px 0;
            transition: background 0.18s;
        }
        .btn:hover {
            background: #1741a7;
        }
        .divider {
            border-bottom: 1px dashed #eee;
            margin: 28px 0 18px 0;
        }
        @media (max-width: 600px) {
            .container {
                padding: 12px 5vw;
                max-width: 98vw;
            }
            h1 { font-size: 1.5rem; }
            h2 { font-size: 1.1rem; }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>大事件 (Big Event)</h1>
        <p style="text-align:center; color:#5b6477; margin-bottom:30px;">专业的文章内容管理系统 | 前后端分离 | Vue + Java + Redis</p>

        <h2>项目简介</h2>
        <p><strong>大事件</strong>是一个专业的文章管理系统，致力于提供文章内容的创建、编辑、发布和管理等功能。本项目采用前后端分离架构，旨在打造高效、灵活的内容平台。</p>

        <div class="divider"></div>

        <h2>技术栈</h2>
        <div class="tech-stack">
            <span class="tech-item">前端: Vue</span>
            <span class="tech-item">后端: Java</span>
            <span class="tech-item">运行环境: Redis</span>
            <span class="tech-item">云仓库: GitHub</span>
        </div>

        <div class="divider"></div>

        <h2>安装与运行</h2>
        <div class="env-setup">
            <h3>前提条件</h3>
            <ul>
                <li>Node.js <span style="color:#8b8b8b;">(用于运行 Vue 前端)</span></li>
                <li>Java JDK <span style="color:#8b8b8b;">(用于编译和运行 Java 后端)</span></li>
                <li>Redis Server <span style="color:#8b8b8b;">(作为项目的运行环境)</span></li>
                <li>Git <span style="color:#8b8b8b;">(用于版本控制和克隆仓库)</span></li>
            </ul>
            <h3>获取项目代码</h3>
            <ol>
                <li>克隆本项目到您的本地机器：
                    <pre>git clone &lt;您的-GitHub-仓库地址&gt;</pre>
                </li>
                <li>进入项目目录：
                    <pre>cd big-event</pre>
                </li>
            </ol>
            <h3>后端 (Java) 设置与运行</h3>
            <ol>
                <li>进入后端项目目录。</li>
                <li>使用 <strong>Maven</strong> 或 <strong>Gradle</strong> 编译项目（根据您的项目配置选择）。</li>
                <li>运行后端应用程序。</li>
            </ol>
            <h3>前端 (Vue) 设置与运行</h3>
            <ol>
                <li>进入前端项目目录。</li>
                <li>安装项目所需的 npm 包：
                    <pre>npm install</pre>
                </li>
                <li>启动开发服务器：
                    <pre>npm run serve</pre>
                </li>
                <li>
                    前端应用通常会在
                    <code>http://localhost:8080</code>
                    启动（具体端口请参考终端输出）。
                </li>
            </ol>
            <h3>运行环境 (Redis) 配置</h3>
            <ul>
                <li>确保 Redis 服务器已在您的机器上安装并运行（默认 <code>localhost:6379</code>）。</li>
                <li>如有需要，在后端应用的配置文件中指定 Redis 连接信息（主机、端口、密码等）。</li>
            </ul>
        </div>

        <div class="divider"></div>

        <h2>云仓库说明</h2>
        <div class="repo-info">
            <p>本项目使用 <strong>GitHub</strong> 作为代码托管和版本控制的云仓库。</p>
            <ul>
                <li><strong>主仓库</strong>: 用于存放项目的主要源代码。</li>
                <li><strong>uploads 仓库</strong>: 用于管理上传文件（如图片、文档等）。</li>
            </ul>
        </div>

        <div class="divider"></div>

        <h2>如何贡献</h2>
        <ol>
            <li><strong>Fork</strong> 本仓库。</li>
            <li>创建功能分支：
                <pre>git checkout -b feature/YourAmazingFeature</pre>
            </li>
            <li>提交更改：
                <pre>git commit -m 'Add some YourAmazingFeature'</pre>
            </li>
            <li>推送到分支：
                <pre>git push origin feature/YourAmazingFeature</pre>
            </li>
            <li>发起 <strong>Pull Request</strong>。</li>
        </ol>

        <div class="divider"></div>

        <h2>许可证</h2>
        <p>本项目采用 MIT 许可证。详情请查看
            <a href="LICENSE" target="_blank">LICENSE</a> 文件。
        </p>

        <div class="divider"></div>

        <h2>联系方式</h2>
        <p>如有任何问题或建议，请通过以下方式联系我们：</p>
        <ul>
            <li>在 GitHub 仓库中提交 <a href="#">Issue</a></li>
        </ul>
    </div>
</body>
</html>
