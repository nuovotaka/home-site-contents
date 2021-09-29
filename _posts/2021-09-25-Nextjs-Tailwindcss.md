---
title: 'Next.jsとTailwind CSSの構成図を作ってみました'
description: Nextjs Tailwind css Github Vercel Netlify Typescript Eslint
date: '2021-09-25'
modified_date: '2021-09-29'
image: /assets/images/posts/nextjs-starter-banner.png
---

## Nextjs,Tailwind CSS,Vercel,Githubの構成図

![構成図](@@baseUrl@@/assets/images/posts/nextjs-chart.png)

記事の管理をマークダウンで記述して管理したかったのと記事とAppを分離したかったのでこのような構成になりました。

Appの変更があった場合はそちらだけで更新が可能です。
記事のみを投稿するときはVercelのBuild HookとGithubのWeb Hooksを利用しています。

ユーザーはVercelがホストするサーバーを閲覧しにいくことになります。
Githubでは記事とAppのソースの管理を行います。

この構成ではGithubのパーソナルアクセストークンを利用しています。

###　追記

構成図にある通りビルド、デプロイサーバーをNetlifyからVercelに変更しました。
カスタムドメインも変更しています。

HugoのサイトもVercelのサーバーへ移行しました。
少し改善されたような気がします。
