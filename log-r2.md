# 100 Days Of Code **R2** - Log

ちょっとさぼり気味だったので勉強する習慣をつけたくて、また100DaysOfCodeでもやろうかな～、と思ってふと気づいたら昨年1周目を始めた日の数日前でした。  
せっかくなので同じ日、今日から、やります！

去年やったときは結構ガチガチに公式ルールにのっとってやったのですが、今回はちょっとゆるめに行こうと思います…。

- チュートリアルを受講するだけでもOKとする（昨年、途中でインプット不足になっていくのを感じたので）
- Twitterでなく個人ブログでやる。ソーシャルメディアで他の人にリアクションする数・頻度は重視しない（コミュ障なのでストレスになってしまった…）


### Day 1: August 22, 2019

**Today's Progress:**  
- paiza Webセキュリティ入門編1: ウェブサイトの攻撃手法と対策の実践 チャプター04, 05

セキュリティ系は大事なのは分かるけどよくわからない、という状態がずっと続いているので、無料で公開されていたこの講座に手をだしてみました。  
SQLインジェクションやXSSを言葉としては知っていましたが、実際の攻撃手法の例と対策方法をセットで試せるというのは印象に残って良かったです。  
phpがほぼ分からないので、それで無駄に時間使ってしまった感はありつつ…。  
（例の通りに書いてるはずなのにうまくいかなくてすごい悩んだ結果「保存」ボタンを押してなくて変更が反映されてないってオチだったんですが）

**Links to work:**  
- なし


### Day 2: August 23, 2019

**Today's Progress:**  
- paiza Webセキュリティ入門編1: ウェブサイトの攻撃手法と対策の実践 チャプター06 →完了
- 自作ツール(Pom-Cal)のパッケージのアップデート

自分が欲しくて作った [Googleカレンダーに連携できるポモドーロタイマー](https://toolsiwant.net/pom-cal/) 、使ってみて色々改善したいところが出ているのでそれをやろうかなと思って、そういえばGitHubからセキュリティアラートが来ていたのでまずそれに対応。  
(ひょっとしてdependenciesに入れてるパッケージ全部devdependenciesなのではと思いつつ…)  

手順を[ブログに残しておきました。](https://ontheneworbit.blogspot.com/2019/08/github-security-alert-packagejson.html)

ついでにMinificationもかけてみた。そしたらたしかに速くなった！  
何日か前にMarkdown変換ツールの方もMinifyしてそっちはほとんど違いが分からなかったのですが、このくらいの規模になると違いが出るものなのか、と実感。

**Links to work:**  
- paiza: [Webセキュリティ入門編1 修了証](https://paiza.jp/works/lesson_certifications/nCzszE-gJUFIFQ)
- Blog: [GitHub から Security Alert が来たので package.json をアップデートする - On the New Orbit](https://ontheneworbit.blogspot.com/2019/08/github-security-alert-packagejson.html)  
- GitHub: [sidemt/pomcal: Pomodoro timer integrated with Google Calendar](https://github.com/sidemt/pomcal)


### Day 3: August 24, 2019

**Today's Progress:**  
- Pom-Cal: Long Break機能の作成
  - Long Break Length の増減ボタン
  - Long Break After の増減ボタン

ポモドーロタイマーにLong Break機能をつけたい。思い出しもかねて、まず増減ボタンを作成。  
Session/Breakの増減ボタンからほぼコピペ（ということは共通化とかすべきなんだろうな…）  
CSSでGridを設定してたこととかすっかり忘れてた。  
`npx babel --watch ...` で変換したファイルをプレビューして確認するために、index.htmlの中で.min.jsを読み込むようにしたところを.jsに戻して作業してるんだけど、公開するときにまた.min.jsにするのを忘れそう。これはどうやるのが普通なんだろ？

**Links to work:**  
- GitHub: [Create buttons for long break length and cycle counts · sidemt/pomcal@abf9bf6](https://github.com/sidemt/pomcal/commit/abf9bf60e69d99185ff3ba72f1eb2867adb9e0e8)


### Day 4: August 26, 2019

**Today's Progress:**  
- Pom-Cal: Long Break機能の作成
  - Long Break の処理を作成、完了

Long Break機能作りました。いろんな機能をつけ足しているのでだんだん画面のレイアウトがぐちゃぐちゃになってきた。

**Links to work:**  
- GitHub: [Add logic for long break · sidemt/pomcal@cd10353](https://github.com/sidemt/pomcal/commit/cd103532ba5af5a3825dc4a3bbd1673b988cf84b)


### Day 5: August 27, 2019

**Today's Progress:**  
- Pom-Cal: レイアウトの調整

友達に見てもらって、各部品の高さや幅が揃うように調整。（特にモバイルレイアウトがガタガタだった…）  
PCレイアウトは画面の幅を活かしたかったので3列の配置にしました。

marginを設定していると、 `width: 100%;` にすると思ってる幅よりはみ出してしまったりする。 `width: auto;` にすると直る。難しい…

`grid-template-columns` でGridの幅を指定できる。 `grid-gap` でGridの間隔を指定できる。この辺覚えておきたい。いつも `space-between` とかでむりやりやろうとしてうまくいかないなーと思ってる気がする。

**Links to work:**  
- GitHub: [Adjust grid width and layout by sidemt · Pull Request #16 · sidemt/pomcal · GitHub](https://github.com/sidemt/pomcal/pull/16/files)


### Day 6: August 28, 2019

**Today's Progress:**  
- Actions on Google: Actions SDK　の使い方を調べる
  - gactions CLI のインストール
  - action.json の作成

やっぱりGoogle HomeのActionが作りたいのでやってみよう。  
以前調べた時はDialogFlowを使う方法を調べてたけど、下記の記事を読んでいてActions SDKの方がひょっとして自分のやりたいことに合ってるのではと思ったのでまずはActions SDKの使い方を調べる。

[Actions On Googleなんちゃって中級編 - Qiita](https://qiita.com/odetarou/items/3bb06de7276fa104236f)

>特にDIalogFlowを使わないでも照明を消すや単純なコマンドであればActions SDKのほうが最初からjsで書けてシンプルではあるので問題はなさそうです。今後はActions SDKのほうが流行るかも？

まずこちらの手順書に沿って進めてみて概要を掴もうとしてます。  
[Actions SDK Basics  |  Actions on Google  |  Google Developers](https://developers.google.com/actions/sdk/)

今日のところは情報を探すのに色々手間取ってしまったので、とりあえず [Create a Project and Action Package](https://developers.google.com/actions/sdk/create-a-project) の最後、action.jsonを作成したところまで。

**Links to work:**  
- なし


### Day 7: August 29, 2019

**Today's Progress:**  
- Actions on Google: Actions SDK　の使い方を調べる
  - Deploy Fulfillment の終わりまで

こちらの手順書  
[Actions SDK Basics  |  Actions on Google  |  Google Developers](https://developers.google.com/actions/sdk/)  
読み進めたものの、このコードはどこに書けばいいの？とかいくつか分からない点があってこれだけではうまくいかず。

下記のサンプルのREADMEに沿って、まずこのサンプルをテストできる状態にするのがわかりやすかったです。

[actions-on-google/actionssdk-say-number-nodejs: Say a number Actions SDK sample for Actions on Google](https://github.com/actions-on-google/actionssdk-say-number-nodejs)

**Links to work:**  
- なし


### Day 8: August 30, 2019

**Today's Progress:**  
- Actions on Google: Actions SDK　の使い方を調べる
  - Submit Your Action の終わりまで
  -

いろんなドキュメントを探したり読んだりに終始して、今日はあまり手を動かせず。  
DBに保存してある情報をActions on Googleから呼び出すことができるのか調べてる。

[ここ](https://techblog.gmo-ap.jp/2018/01/19/%E3%80%8C%E6%9C%AC%E6%B0%97%E3%81%AE%E3%81%97%E3%82%8A%E3%81%A8%E3%82%8A%E3%80%8Dgoogle-home%E3%82%A2%E3%83%97%E3%83%AA%E3%82%92%E4%BD%9C%E3%82%8A%E3%81%BE%E3%81%97%E3%81%9F%E3%80%82/)が参考になりそう？

成果物代わりに、読んだページを一言メモとともにリストアップして [ブログ](https://ontheneworbit.blogspot.com/2019/08/actions-on-googledatabase.html) に残しておきました。

あしたはとにかく何でもいいのでFirebase Realtime Databaseからデータを読み出すということをやってみようかな？

**Links to work:**  
- Blog: [読んだ物メモ (Actions on Googleの基本とDatabaseとの接続) - On the New Orbit](https://ontheneworbit.blogspot.com/2019/08/actions-on-googledatabase.html)
