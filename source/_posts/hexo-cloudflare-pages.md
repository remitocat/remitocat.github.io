---
title: Hexo & Cloudflare Pagesでブログを立ち上げました
date: 2021-05-23 11:47:23
category: tech
tags:
 - [Node.js]
 - [Hexo]
 - [Cloudflare]
cover_img: /images/hexo-cloudflare-pages-thumbnail.png
summary: 文章をストックしておく場として活用する予定です
---

これまでMastodonに文章を書き留めていましたが、1000文字 (Chillout Chatの投稿文字数制限) を超える長文や、毎年恒例のAdvent Calender用に書く記事をストックしておく場として、新たにブログを立ち上げました。
私は学生であるため、安定した収入がないことから、これ以上サーバーに資金を費やすことができません。そのため、静的サイトジェネレータである [Hexo](https://hexo.io) を使用し [Cloudflare Pages](https://pages.dev) にデプロイすることで、無料で運用できるようにしました。

## Cloudflare Pagesのメリット

Cloudflare Pagesの他にも、静的サイトジェネレータの生成物をホスティングするサービスとして [GitHub Pages](https://pages.github.com)・[Netlify](https://www.netlify.com)・[Vercel](https://vercel.com) などが有名です。どのサービスにもそれぞれ利点がありますが、ここではCloudflare Pagesのメリットをいくつか紹介したいと思います。

### HTTP/3に対応
2019年にGoogle Chromeでもサポートされた、新しい通信規格であるHTTP/3に対応しているため、HTTP/3に対応した環境からはサイトと効率的に通信することができます。

### データ転送量が無制限

他のサービスでは100GB/月などの制限がありますが、Cloudflare Pagesは無料プランから無制限となっています。個人運用のレベルで転送量が100GB/月を超すことは考えにくいですが、アクセス数の多い企業運営のサイト等を運用するにあたっては大きなアドバンテージとなるかもしれません。

### アクセス制限が無料

他のサービスでは有料プランにアップグレードしなければアクセス制限を使用することができませんが、Cloudflare Pagesなら50人までのチームでの運用であれば無料でアクセス制限をかけることができます。

## 設定のポイント

Cloudflare Pagesには、簡単にビルドの設定を行うためにフレームワーク プリセットが用意されていますが、残念ながらHexoのプリセットは (2021.05.23現在) 用意されていません。そのため、ビルドコマンドとビルド出力ディレクトリを自分で設定する必要があります。
ビルドに関する設定を `_config.yml` で変更していなければ、以下の設定で動作するはずです。

> ビルドコマンド: `hexo generate`
> ビルド出力ディレクトリ: `public`
