---
title: "鯖缶年報 '21"
slug: annual-report-2021
image: 
author: "Remito"
date: 2021-12-23T16:00:00+09:00
draft: false
categories: [fediverse]
tags: [Advent Calendar 2021]
---

**[Fediverse Advent Calendar 2021](https://adventar.org/calendars/6230) 23日目**

こんばんは。三条れみと ([@remito@chillout.chat](https://chillout.chat/@remito)) です。この記事では，技術系同人サークル「桜ヶ丘電信」が運営するサーバーのうち，私が管理に携わっている4つのサーバーを紹介するとともに，2021年に起こったサーバーに関する主な出来事を振り返っていきたいと思います。

## Chillout Chat

- URL: [chillout.chat](https://chillout.chat)
- GitHub: [sakura-tel/mastodon](https://github.com/sakura-tel/mastodon)

Chillout Chatは，3月5日にオープンしたMastodonサーバーです。私とやなぎぃ氏 ([@YanagieIsHere@chillout.chat](https://chillout.chat/@YanagieIsHere)) が中心となって運営していますが，モデレーションは桜ヶ丘電信のメンバー全員で行っています。

### コンセプト

Chillout Chatには，2つのコンセプトがあります。

1つ目のコンセプトは，**音楽を聴くのが好きな人が集まり，くつろげるようなサーバー** です。 サーバー名の由来となった chill out という言葉は，落ち着くことを表すだけでなく，スローテンポでリラックスさせるような音楽を形容することもあります。chill outな音楽に限らず，様々なジャンルの音楽を愛好する人が交流できるような空間であってほしいと思っています。

2つ目のコンセプトは，**安心して過ごせる居場所となるようなサーバー** です。Fediverseには様々なサーバー・インスタンスがありますが，その中でも特に居心地が良いと思ってもらえるような環境づくりを心がけています。

桜ヶ丘電信では，このコンセプトを実現するために，ユーザーを守るためのモデレーションを重要視しています。先述したように，モデレーションに取り掛かかる人員を増やしているのは，トラブルが起こった際に，迅速で公正な措置がとれるようにするためです。一方で，ユーザーが自由に利用できるような空間をつくることも重要です。そのため，利用規約に反しない限り，管理者がユーザーの行動に対して一切干渉しないことをモデレーションの大原則としています。

### 独自機能

Chillout Chatに導入されている主な独自機能を紹介します。

#### Koruriフォント

デフォルトのフォントとして，M+ OUTLINE FONTSとOpen Sansを合成させたKoruriフォントを導入しています。[koruri.chillout.chat](https://koruri.chillout.chat) からGoogle Fontsと同じ要領で読み込んでいます。

#### トロピカルテーマ
![](https://uma.milkey.homes/files/d8c99fe0-7fc3-4878-ab68-51b4f707b0b4/d8c99fe0-7fc3-4878-ab68-51b4f707b0b4.png)

みねむ氏 ([@Minemu483K@machikadon.online](https://machikadon.online/@Minemu483K)) がデザインしたサイトテーマです。

> 本来はグラデーション使った面白いテーマにするつもりだったのですが，思いの外ダサくなってしまい，ダサくて南国っぽいテーマとして方向転換したのが「トロピカルばれいしょテーマ」です。「ばれいしょ」は我々が崇めている2年前に失踪したMastodonユーザーのハンドルネームが由来となっています。
> 
> (みねむ氏の紹介)

#### Cat機能
![](https://uma.milkey.homes/files/2505fb9f-6ca2-4fa9-9cca-a4a71923e6f4/2505fb9f-6ca2-4fa9-9cca-a4a71923e6f4.gif)

Misskeyの機能をMastodonに移植したものです。[小田急丼の実装](https://github.com/accelforce/mastodon/tree/custom/cat) をベースとして，アイコンに猫耳が生えるように改良を加えました。猫耳が生えると幸せになれますね。

### 姉妹サーバー・Chillroma

- URL: [pleroma.chillout.chat](https://pleroma.chillout.chat)

Chillout Chat の避難所として開設されたPleromaサーバーです。桜ヶ丘電信のサーバーとしては珍しく，何もカスタマイズをしていないバニラで運用しています。周知もあまりしなかったため，過疎状態となってしまいました。VPSへの負荷はあまりかからないため，過疎状態であっても運用を継続することはできますが，管理者としては盛り上げたいところです。

## Milkey

![](https://uma.milkey.homes/files/77be7701-a53f-47f9-8316-fa7c1213e6e0/77be7701-a53f-47f9-8316-fa7c1213e6e0.png)

- URL: [milkey.homes](https://milkey.homes)
- GitHub: [sakura-tel/groundpolis](https://github.com/sakura-tel/groundpolis)

Milkeyは，3月30日にChillout Chatのリソースを活用して生まれたインスタンスです。インスタンス名はメディアミックスプロジェクト「Project MILKY HOLMES」にちなんでいます。

開設した当初はMisskeyサーバーとして運用していましたが，夏に私のミスが原因でデータベースが破壊され，休止せざるを得ない状況となりました。そのまま閉鎖することも考えていましたが，10月には「データベースをリセットし，過去に使用していたユーザー名で登録できないようにする」という，Misskey.ioと同様の方法で復旧させることができました。

復旧後はGroundpolisサーバーとして再始動し，Groundpolisの新機能実装に貢献しています。また，VPSをChillout Chatと共用のものから，ConoHaの東京リージョンに移転して運用しているため，Chillout Chatが使えない時の避難所としての役割も期待されています。

### 姉妹インスタンス・umaMilkey

![](https://uma.milkey.homes/files/a4d2c250-e996-43d3-9f84-b19796300af6/a4d2c250-e996-43d3-9f84-b19796300af6.png)

- URL: [uma.milkey.homes](https://uma.milkey.homes)
- GitHub: [sakura-tel/misskey-v11](https://github.com/sakura-tel/misskey-v11)

Milkeyが休止している間の代替インスタンスとして生まれたのがumaMilkeyです。サーバー名の"uma"には，今年流行したスマホゲームの「ウマ娘 プリティーダービー」や，「突然作られた未確認生物のような存在」という，インスタンスが誕生した経緯にちなんでいます。

ソフトウェアにはumaMilkey向けにカスタマイズされたMisskey v11を使用しています。umaMilkeyのヘビーユーザーである，ｺﾓﾊﾁｰﾖこと藤敷菰八氏 ([@FS5@misskey.io](https://misskey.io/@FS5)) も開発に携わっており，様々な独自機能が実装されています。

Milkeyが復旧してからは，代替サーバーとしての役割を失いましたが，競馬やウマ娘の話題を取り扱うサーバーとして盛り上がっています。有馬記念が楽しみですね。

## 2022年に向けて

2021年は，Milkeyの長期間休止をはじめとした，多くのインシデントを発生させてしまった1年でした。2022年はより手堅い運用を心がけ，サーバーの安定稼働に努めていきたいと思います。また，桜ヶ丘電信のメンバーが受験勉強や就職活動を終えるため，Fediverseに関する新しいプロジェクトに取り組んでいきたいと思います。具体的には，桜ヶ丘電信 Advent Calendar 25日目の記事で紹介する予定であるMetaFediverse構想の実現や，Chillout Chatの大改修に向けて動く予定です。2022年もどうぞよろしくお願いします。