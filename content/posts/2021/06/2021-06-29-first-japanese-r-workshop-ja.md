---
layout: page
authors: ["Joel Nitta", "Tom Kelly", "Kozo Nishida", "Masami Yamaguchi"]
title: "ソフトウェアカーペントリーの初日本語ワークショップ"
date: 2021-06-29
time: "00:00:00"
category: ["Community", "Internationalisation", "Curriculum", "Japan", "Online Workshops"]
---

([Read this post in English](https://carpentries.org/blog/2021/06/first-japanese-r-workshop-en/))

この間、初めて日本語で[ソフトウェアカーペントリー（SWC）](https://software-carpentry.org/)のワークショップをオンラインで開催しました。今回のワークショップは、[東京大学](https://www.u-tokyo.ac.jp/)と[ソフトバンク](https://www.softbank.jp)が共同で立ち上げた[Beyond AI研究推進機構](https://beyondai.jp/)の中の研究グループ、[B'AI Global Forum](https://baiforum.jp/)との共同開催でした。[「Rによるデータ解析入門」](https://swcarpentry-ja.github.io/2021-04-02-todai-online-ja/)というタイトルで、[今まで翻訳してきたRレッスン](https://swcarpentry-ja.github.io/r-novice-gapminder/ja/)を元に行いました[^prev-blog]。以下、[カーペントリーズ形式](https://datacarpentry.org/blog/2017/06/minute-cards)で「緑付箋」（上手く行ったこと）と「赤付箋」（上手く行かなかったこと）に分けて感想をまとめました。

## 緑付箋（上手く行ったこと）

### 共同主催者と密接な連携

今回の共同主催者の[B'AI Global Forum](https://baiforum.jp/)には大変お世話になりました。B'AI Global Forumが参加者（主に東京大学文系大学院生）を募集して、重要な連絡をしてくれたので、ワークショップの準備に集中することが出来ました。対応がいつも丁寧かつプロフェッショナルでした。パートナーは大事です。　

### オンラインで行うワークショップの知識

今回のワークショップは新型コロナウイルスによってワークショップがオンラインに移り始めてからちょうど一年目というタイミングで行いました。その間に、カーペントリーズのコミュニティーからワークショップをオンラインで行う上でのヒント・アドバイスが色々挙げられました[^links]。インストラクターのためのオンラインで[ワークショップを行うワークショップもあります](https://carpentries.github.io/instructor-training-bonus-modules/01-online-workshops-module-1/index.html)！これらの資料は大いに参考になりました。そして、参加者もかなりすでにオンライン（zoom）に慣れていましたので、割とスムーズに行きました。

### 練習と準備

しかし、ヒントだけでは出来ません。ワークショップの前に２回ほど全員（インストラクター２人、ヘルパー４人）でミーティングをして、インストラクターだけでさらに数回練習会をしました。オンラインでワークショップを行うのは本当に複雑で、落とし穴だらけです。何回も練習したら、ブログポストを読むだけでは分からないことを色々に気付きました。そして、毎回セッションが終わった後にインストラクターやヘルパーで30分くらい反省点など話し合うことによって、次回の内容の調整ができました。

## 赤付箋（上手く行かなかったこと）

### 教える内容の変更による混乱

元々は唯一翻訳が完成したレッスンの[「R for Reproducible Scientific Analysis」](https://swcarpentry-ja.github.io/r-novice-gapminder/ja/)を教えることを予定していたのですが、参加者は主に文系の大学院生で、時間も短いものでした（全５回、２時間ずつ）。そう考えると、Rの基礎を丁寧に教えるSWC形式よりも、なるべく早く実際に応用できるデータ・カーペントリー（DC）の[「Data Analysis and Visualization with R for Social Scientists」](https://datacarpentry.org/r-socialsci/)の方がふさわしい、と思うようになりました。が、データ・カーペントリーのレッスンはまだ日本語訳が出来ていなかったので、最終的には翻訳済のR for Reproducible Scientific Analysisの用語を使いながら、教える内容をDCのレッスンのように教えることにしました（例えば、ベースRよりもtidyverseから使う、など）。ちょっと混乱しましたが、最終的はこのようにして良かったと思います。理想的にはいつか、他のレッスンも翻訳したいところです！

### オンラインで教える内容の選定

オンラインのワークショップだと、教えられる内容が大幅に減ることを予想しましたので、レッスンの内容はかなり軽く設定しました。それでも、４回目のレッスンでパイプ（`%>%`）、`dplyr::group_by()`、`dplyr::summarize()`を全部教えようとしたら、流石に多すぎました。この三つのコンセプトはどれも初心者にはかなり難しいので、もっと時間が必要だと反省しています。

## まとめ

初の日本語SWCワークショップは全体的に上手く行ったと思います。アンケートでは参加者から非常に高い評価をいただきました[^survey]。翻訳が完成したレッスンは今のところ一つしかないことで多少困りましたが、近い将来、他のレッスンもどんどん翻訳したいと思います。皆様から日本語カーペントリーズのコミュニティーのご参加をお待ちしています！

## 参加方法

- [SWC日本語チームのホームページ](https://swcarpentry-ja.github.io/)
- ツイッター： [@swcarpentry_ja](https://twitter.com/swcarpentry_ja)
- フェイスブック： [carpentries.ja](https://www.facebook.com/carpentries.ja)
- ギットハブ: [swcarpentry_ja](https://github.com/swcarpentry-ja)
 
スラックチャンネルもあります (日本語でも英語でも大丈夫です)。[ここ](https://carpentries-ja.herokuapp.com/)からご参加ができます。

どなたでもレッスンの翻訳に貢献できます。もしギットハブ上でのワークフローについてのご質問があったら、気軽に聞いてください。どうぞよろしくお願いします！

[^prev-blog]: レッスンの翻訳についてのブログポストは[こちらです](https://carpentries.org/blog/2021/02/complete-R-lesson-japanese/)（英語）。

[^links]: これらのブログポストは特に参考になりました：[Online Workshop Logistics and Screen Layouts](https://carpentries.org/blog/2020/06/online-workshop-logistics-and_screen-layouts/), [Recommendations for Teaching Carpentries Workshops Online](https://carpentries.org/online-workshop-recommendations/), [Mapping & Planning a Live Coding Workshop for Digital Delivery](https://carpentries.org/blog/2020/04/plan-map-live-coding-workshop/#my-personal-teaching-setup)

[^survey]: ワークショップに関するアンケートの解析結果は[こちらです](https://github.com/swcarpentry-ja/2021-04-02-todai-assessment/blob/main/survey_report_ja.md)（日本語のみ）。
