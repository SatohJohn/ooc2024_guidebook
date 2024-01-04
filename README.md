# About

## このリポジトリの説明

このリポジトリは、Object-Oriented Conference 2024（OOC2024）の参加者に無料配布する「公式ガイドブック（仮称）」の執筆用データを格納するために作られています。
公式ガイドブックには、カンファレンスの概要や見どころなど参加者に向けたご案内のほか、カンファレンス参加を予定されている方であれば立場を問わずどなたでも「オブジェクト指向に関する技術記事」を寄稿いただけます。
たとえば、スピーカーによる登壇内容の増補や解説、スポンサーによる組織内のオブジェクト指向な取り組み事例、参加者による技術解説など、さまざまな記事をお寄せください。
OOC2024に関わる皆さまで、カンファレンスオリジナルの技術書を1冊作り上げましょう！

寄稿に際して、以下の条件を設けます。

1. カンファレンスの趣旨に沿った記事であること
    - どなたでも：技術的な記事
    - スポンサー：プロダクト紹介、組織紹介、人材募集、など
    - スタッフ：スタッフの裏話、担当範囲の紹介、など
3. すべての方に公開可能な内容であること
4. 他者の著作権を侵害しないこと
5. （スポンサー以外の方のみ）営業行為や求人をおもな目的にしないこと
6. その他、OOCが定める行動規範に反しないこと

登壇だけがアウトプットではありません！本という形で、あなたの知識をアウトプットしてみませんか？
OOC実行委員会では、あなたの寄稿をお待ちしています。ぜひご参加ください。

## 執筆要綱

本READMEと一部重複しますが、執筆に際して執筆要綱をご一読ください。

- [一般向け募集要項(スピーカーやスタッフを含む)](https://esa-pages.io/p/sharing/20260/posts/86/ea5cb758351fd3d32a4c.html)
- [スポンサー向け募集要項](https://esa-pages.io/p/sharing/20260/posts/91/b543c2a5dda510d3a93a.html)

### 寄稿手順

1. 寄稿する原稿をMarkdown形式で執筆してください
2. 原稿を `/markdown` ディレクトリ内に配置し、プルリクエストしてください
3. OOC実行委員会にて内容を確認し、必要に応じてコメントを戻します
4. 内容がマージされたらOOC実行委員会にて印刷用レイアウトを整備します

### スケジュール

日程 | 内容
---|---
2024年1月31日　| 新規寄稿の受付締め切り（以降は修正期間になります）
2024年2月20日　| 寄稿内容の校了（以降は印刷内容を変更できません）
2024年3月初旬 | 印刷入稿予定日
2024年3月24日　| カンファレンス当日

上記日程は目安になります。
詳細状況はDiscordスペースにて共有しますので、そちらの案内をご覧ください。

### 執筆にあたってのお願い

個別のご相談はDiscordにて受け付けます。

- コンフリクトが解消できない場合は、実行委員会　@oyakata2438 @ar1ak1 までご相談ください
- その他、困ったことがあれば、お気軽にご相談ください

## Re:VIEWの書き方

[Re:VIEWチートシート](https://gist.github.com/erukiti/c4e3189dda179a0f0b73299fb5787838) を作ってみたので、参考にしてみてください。

## 原稿を確認したい
自分が書いた原稿がどんな感じになるかを見たいときは、

* 自分でコンパイルする。
* 編集にPDF送付を依頼する
* 定期的にDiscordに上がるPDFを確認する

のいずれかが可能です。

以下、自分でPDFをビルドする方法です。

### Dockerを使う方法

Dockerを使うのが一番手軽です。

```sh
$ docker run --rm -v `pwd`:/work vvakame/review /bin/sh -c "cd /work/articles ; review-pdfmaker config.yml"
```

### bat/shでビルド
ローカルにDockerがあれば、
build-print.batを叩くと/src内にpdfができるよ！

## 権利

ベースには、[TechBooster/ReVIEW\-Template: TechBoosterで利用しているRe:VIEWのテンプレート（B5/A5/電子書籍）](https://github.com/TechBooster/ReVIEW-Template) を使っています。

* 設定ファイル、テンプレートなど制作環境（techbooster-doujin.styなど）はMITライセンスです
* 再配布などMITライセンスで定める範囲で権利者表記をおねがいします
