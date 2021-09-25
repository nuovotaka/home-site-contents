---
title: 'Next.jsとTailwind CSSの構成図を作ってみました'
description: Nextjs Tailwind css Github Netlify Typescript Eslint
date: '2021-09-25'
modified_date: '2021-09-25'
image: /assets/images/posts/nextjs-starter-banner.png
---

## Nextjs,Tailwind CSS,Netlify,Githubの構成図

![構成図](@@baseUrl@@/assets/images/posts/nextjs-chart.png)

記事の管理をマークダウンで記述して管理したかったのと記事とAppを分離したかったのでこのような構成になりました。

Appの変更があった場合はそちらだけで更新が可能です。
記事のみを投稿するときはNetlifyのBuild HookとGithubのWeb Hooksを利用しています。

ユーザーはNetlifyがホストするサーバーを閲覧しにいくことになります。
Githubでは記事とAppのソースの管理を行います。

この構成ではGithubのパーソナルアクセストークンを利用しています。
