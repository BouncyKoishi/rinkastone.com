---
title: "网站迁移说明"
date: 2026-05-06T12:00:00
lastmod: 2026-05-06T12:00:00
author: "小石子"
categories: ["公告"]
tags: []
description: "本站已从 WordPress 迁移至 Hugo，文章内容、URL、图片资源均保持不变，托管平台改为 GitHub Pages。"
draft: false
---

<p>本站已从 WordPress 迁移至 Hugo，以下是迁移相关说明。</p>



<h2 class="wp-block-heading">为什么要迁移</h2>



<p>最近在整理服务器资源，想优化掉一些不必要的开支。这个个人博客没有动态页面的需求，完全可以转到 GitHub Pages 托管，于是就开始了这次迁移。</p>



<p>静态站点生成器的选型上，我选择了 Hugo。</p>



<h2 class="wp-block-heading">迁移保留了什么</h2>



<p></p>



<h3 class="wp-block-heading">文章内容</h3>



<p>所有历史文章均已迁移，内容保持不变。文章 URL 也保持了与 WordPress 时期相同的格式：</p>



<p><code>/{年}/{月}/{日}/archives/{文章ID}</code></p>



<p>例如 <url>https://rinkastone.com/2021/09/13/archives/51</url> 仍然可以访问。</p>



<h3 class="wp-block-heading">图片资源</h3>



<p>文章中的图片已从 WordPress 媒体库迁移至本站 <code>static/images/wp/</code> 目录，图片链接保持有效。</p>



<h3 class="wp-block-heading">友链页面</h3>



<p>友链页面保持不变，地址为 <a href="/links/">https://rinkastone.com/links/</a>。</p>



<h2 class="wp-block-heading">迁移后的变化</h2>



<p></p>



<h3 class="wp-block-heading">用户系统</h3>



<p>WordPress 自带的用户体系不再可用。本网站存在站长以外的用户，现在这些用户无法直接在本网站上传文章了。历史上由其它用户上传的文章会保留用户名显示，如果其它用户需要上传新文章可通过其它途径联系站长代发，或直接在 Github 仓库中提 pr 上传你的 md 文件。</p>



<h3 class="wp-block-heading">评论系统</h3>



<p>WordPress 自带的评论功能和文章点赞功能不再可用。如有需要联系作者，可通过友链页面中的联系方式。</p>



<h3 class="wp-block-heading">搜索功能</h3>



<p>暂未实现站内搜索功能。如有需要，可使用搜索引擎的 <code>site:</code> 语法，例如：</p>



<p><code>site:rinkastone.com 关键词</code></p>



<h2 class="wp-block-heading">技术细节</h2>



<p>本站当前使用：</p>



<ul class="wp-block-list">
<li><strong>站点生成器</strong>：Hugo</li>
<li><strong>主题</strong>：<a href="https://github.com/Tokinx/Adams">Adams</a>（基于原 WordPress 主题移植）</li>
<li><strong>托管平台</strong>：GitHub Pages</li>
<li><strong>CI/CD</strong>：GitHub Actions（推送后自动构建部署）</li>
</ul>



<p>所有源文件托管在 GitHub 仓库中，每次推送到主分支后，GitHub Actions 会自动运行 <code>hugo</code> 命令构建站点并部署到 GitHub Pages。</p>



<hr>



<p><em>如有任何问题或建议，欢迎通过友链页面中的联系方式与我交流。</em></p>
