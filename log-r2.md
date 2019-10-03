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

いろんなドキュメントを探したり読んだりに終始して、今日はあまり手を動かせず。  
DBに保存してある情報をActions on Googleから呼び出すことができるのか調べてる。

[ここ](https://techblog.gmo-ap.jp/2018/01/19/%E3%80%8C%E6%9C%AC%E6%B0%97%E3%81%AE%E3%81%97%E3%82%8A%E3%81%A8%E3%82%8A%E3%80%8Dgoogle-home%E3%82%A2%E3%83%97%E3%83%AA%E3%82%92%E4%BD%9C%E3%82%8A%E3%81%BE%E3%81%97%E3%81%9F%E3%80%82/)が参考になりそう？

成果物代わりに、読んだページを一言メモとともにリストアップして [ブログ](https://ontheneworbit.blogspot.com/2019/08/actions-on-googledatabase.html) に残しておきました。

あしたはとにかく何でもいいのでFirebase Realtime Databaseからデータを読み出すということをやってみようかな？

**Links to work:**  
- Blog: [読んだ物メモ (Actions on Googleの基本とDatabaseとの接続) - On the New Orbit](https://ontheneworbit.blogspot.com/2019/08/actions-on-googledatabase.html)


### Day 9: August 31, 2019

**Today's Progress:**  
- Actions on Google: Actions SDK　の使い方を調べる
  - Firebase Realtime Databaseからデータを読み出す

公式で提供されているサンプルにデータベースとの接続を付け加えて、なんとか値を読み出すことができた…！！！

けどPromiseとかCallbackの使い方がよくわかってなくて（昔理解したのに忘れてしまった…）DBからのレスポンスを待ってActions on Googleに渡すということができてない。

とりあえず、 `firebase deploy` したタイミングで読みだした値を格納しておいて後で使うということはできた。まずActions on GoogleとFirebase Realtime Databaseが接続できるということだけは確認できた！

**Links to work:**  
- GitHub: [Connect to Firebase Realtime Database · sidemt/actionssdk-say-number-nodejs@82f1fce](https://github.com/sidemt/actionssdk-say-number-nodejs/commit/82f1fcede9e0e3a760e671978ad74273e9e80a98)


### Day 10: September 1, 2019

**Today's Progress:**  
- Actions on Google: Actions SDK　の使い方を調べる
  - [Daily Updates & Push Notifications Sample](https://github.com/actions-on-google/dialogflow-updates-nodejs) を動かしてみる

あんなにずっとそもそもデータベースとの接続ができるのかどうか分からなくて調べてたのに、このサンプルであっさりできた…（苦笑）

Dialogflow と Cloud Firestore を組み合わせて使うバージョンのサンプル。  
良さそう。カテゴリ名で検索してる部分のコードとか参考になりそう。

私が作りたいアプリが、ユーザーが入力した名前（しかも芸名・ペンネームとかの一般的な名前っぽくない名前）をキーにして探したいので、難しそうだなと思ってたんだけど、音声入力でうまく聞き取ってもらえなくてもスマホなら最悪キーボード入力はできるよね、とこのサンプルを触ってて気づく。  
おそらく最初に使ってもらえそうな層はスマホの人達だし。

個人的な夢としてはやっぱり口頭で会話できるものが作りたいけれど！

**Links to work:**  
- なし


### Day 11: September 2, 2019

**Today's Progress:**  
- Actions on Google: Actions SDK　の使い方を調べる
  - [Daily Updates & Push Notifications Sample](https://github.com/actions-on-google/dialogflow-updates-nodejs) のコードを読んでみる

サンプルの index.js のコードを読んで、何をしているコードなのかコメントを細かく入れてみました。  
JavaScript多少勉強してきたおかげか、だいぶActions on Googleの知識が広く浅く集まってきたおかげか、かなり理解できた。

Fork したリポジトリにブランチ切ってコメント入れたファイルを公開してみました。（下記）

**Links to work:**  
- [Add comments to describe sample code · sidemt/dialogflow-updates-nodejs@32609cc](https://github.com/sidemt/dialogflow-updates-nodejs/commit/32609cc0021a0ed03dac3726ee8c6e13a42e9ea5)


### Day 12: September 3, 2019

**Today's Progress:**  
- Actions on Google 開発
  - セットアップ

昨日コードを読んでいたサンプルの真似をしながら、Actions on Googleコンソール、Dialogflow、Cloud Firestore等を設定。  
Firestoreからデータの取得もできている。

ところが、なぜか `where` メソッドで検索した結果を取得しようとすると、急にレスポンスが返ってこなくなり、エラーになる。調査中。

Actions on Google、2年前くらいから構想だけはあって調べていて、日本語の音声でお気に入りの声があったので絶対この子で作ろう！と思っていたのですが、バージョンアップされて声が変わってしまっていて悲しい…（笑）  
たしかに自然さはアップしてるんですが。好みの問題で…

**Links to work:**  
- なし（GitLab private repo）


### Day 13: September 4, 2019

**Today's Progress:**  
- Actions on Google 開発
  - ローカル実行環境セットアップ

[この記事](https://medium.com/voiceano/speed-up-actions-on-google-development-workflow-with-local-fulfilment-7de17d5f166f) を参考に、ローカルで Firebase Functions の代わりになるExpressサーバーを実行できるようにセットアップ。

JavaScriptの単純な文法にすら自信がない上にいろんなサービスを連携させて使わないといけないので、自分のコードが悪いのか何かの設定が上手くいってないのかの切り分けを繰り返すのに、少しコードを変える度に毎回 Firebase Functions にデプロイしないといけないのはかなり辛かったので。

セットアップはうまくいきました！DBにもアクセスできることを確認。これで開発がはかどりそう！

機能うまくいかなかったwhere句での絞り込みは同じように上手くいかず…明日からはこれを調査しようと思います。

**Links to work:**  
- なし


### Day 14: September 5, 2019

**Today's Progress:**  
- Actions on Google 開発
  - Cloud Firestore のデータの検索

できましたー！！！

`db.collection(FirestoreNames.NOTICES)` は取得できているのに `db.collection(FirestoreNames.NOTICES).where(FirestoreNames.KEYWORD, '==', keyword)` とするとMalformed responseというエラーが発生してデータが取得できない問題で悩んでいたのですが、Dialogflowのパラメータ名/Firestoreのフィールド名/変数名の `keyword` を全て `keyword0` に変更すると動くようになりました…原因はわかりません…

キーワード2つを組み合わせての検索もできました。

昨日セットアップしたローカルサーバー大活躍！確かにこれはいちいちFirebase Functionsにデプロイするよりずっと速いし手間がかからない。

**Links to work:**  
- なし


### Day 15: September 6, 2019

**Today's Progress:**  
- Actions on Google 開発
  - search_again intent の追加
  - 会話内容の改善

今日はちょっと内容軽め。でもフォローアップインテントについてドキュメントを読んだり触ってみたり、合言葉のキーワードが足りない時に訊き返す会話(Prompts)を追加したり（これはDialogflow ConsoleのUIから）

あまり複雑に作り込む前に、次はRailsアプリとFirestoreの接続方法を調べようかと思ってます。

**Links to work:**  
- なし


### Day 16: September 7, 2019

**Today's Progress:**  
- Pluralsight (Google Cloud Functions: Getting Started)視聴
- Actions on Google 開発
  - Rails Appの作成
  - PostgreSQL の再インストール

Pluralsightが今週末限定の無料キャンペーンをやっていたので、ちょっと手を出してみました。  
ところが微妙に体調が悪くて思ったように進まず…。全体像を掴むくらいしかできませんでしたが、役には立ったと思います。明日もう少しやりたい。

Actioins on Googleで利用するデータを登録するサイトをRailsで作ろうと思っていて、そのためのRails Appを作り始めました。
WSL上でPostgreSQLが起動できなくなっていたのですが、結局 `apt-get --purge remove postgresql\*` とやって全部アンインストールして、再インストール。その後Railsアプリの database.yml にポート番号を指定してあげることで `rails db:create` が成功し、 `rails s` できるようになりました。

**Links to work:**  
- なし


### Day 17: September 9, 2019

**Today's Progress:**  
- Pluralsight視聴
  - Firebase Functions: Fundamentals
  - Firebase Firestore: Getting Started
  - Firbase Hosting: Fundamentals
  - Architecting Scalable Web Applications with Firebase

無料キャンペーン中に…と思って1.5倍速ぐらいで一気に視聴（笑）

動画の講座って私の場合はあまり頭に入ってこなくて、かつ後で振り返りにくくて苦手なのですが、短時間でざっと概要を掴むという使い方には良いなと思いました。

Pluralsight今回初めて使ったのですが、YouTube等で公開されている無料の動画よりは音声や動画のクオリティも高い感じがして内容もまとまっていて、良かったと思います。  
全文のTranscript（文字起こし）が見れるページがあるのも、後で内容を振り返って探すのに役立ちそう。  

講座のジャンルも豊富で、Firebase関連の講座があったのも予想外だったので良い勉強になりました。

**Links to work:**  
- なし


### Day 18: September 10, 2019

**Today's Progress:**  
- Actions on Google 開発
  - Firebase Hostingのセットアップ

Pluralsightで学習した内容から、そもそもRailsアプリにしなくていいのでは…と気が付いてFirebaseHostingで作ってみることに。
セットアップ。 `firebase deploy` も `firebase serve` も上手くいきました。

Hostingの追加にあたって、既存のプロジェクトに対して `firebase init` して大丈夫なの…？と不安になりましたが、大丈夫でした。その辺ブログに残しておきました。

**Links to work:**  
- Blog: [既存のFirebase Projectにサービスを追加する - On the New Orbit](https://ontheneworbit.blogspot.com/2019/09/firebase-project.html)


### Day 19: September 11, 2019

**Today's Progress:**  
- Actions on Google 開発
  - Firebase Hosting と Cloud Firestore の接続

Cloud Firestore のスタートガイドとそこにあった動画を参考に、Firebase Hosting に置いたウェブページ から Cloud Firestore のデータを操作できることを確認。

HTMLでシンプルな input フォームを設置して、JavaScriptにCloud Firestoreに `docRef.set({ notice: "something" })` みたいなコードを書いて、Submitボタンのonclickで実行されるようにする感じ。とりあえずできました。

参考： [Cloud Firestore を使ってみる  |  Firebase](https://firebase.google.com/docs/firestore/quickstart?hl=ja)

**Links to work:**  
- なし


### Day 20: September 12, 2019

**Today's Progress:**  
- Actions on Google 開発
  - Updatesメソッドでドキュメントの一部を更新

昨日 `set` メソッドでFirestoreにデータを登録できることを試した時に、指定したドキュメントにすでに他のフィールドが存在しても、 `set` で渡したフィールドのみの状態に上書きされてしまうことが分かったので、部分的に更新する方法を調査。

`update` メソッド、または `set` メソッドに `{ merge: true }` を付けてあげることで実現できるようでした。

```
var setWithMerge = cityRef.set({
    capital: true
}, { merge: true });
```

明日試すのはここら辺かなあ。  
[ウェブサイトで Firebase Authentication を使ってみる  |  Firebase](https://firebase.google.com/docs/auth/web/start?hl=ja)

**Links to work:**  
- なし


### Day 21: September 13, 2019

**Today's Progress:**  
- Actions on Google 開発
  - Firebase Authentication

下記を読んで、
- [ウェブサイトで Firebase Authentication を使ってみる  |  Firebase](https://firebase.google.com/docs/auth/web/start?hl=ja)
- [JavaScript で Google ログインを使用して認証する  |  Firebase](https://firebase.google.com/docs/auth/web/google-signin?hl=ja)

ここら辺からコピペして、とりあえず動くことを確認。
- [quickstart-js/email-password.html at 691a9f51ea1849c76e09f46f1e4c83e82672da7a · firebase/quickstart-js](https://github.com/firebase/quickstart-js/blob/691a9f51ea1849c76e09f46f1e4c83e82672da7a/auth/email-password.html#L95-L107)
- [quickstart-js/google-redirect.html at 691a9f51ea1849c76e09f46f1e4c83e82672da7a · firebase/quickstart-js](https://github.com/firebase/quickstart-js/blob/691a9f51ea1849c76e09f46f1e4c83e82672da7a/auth/google-redirect.html)


ログイン・ログアウト機能が作れるのは分かった。GoogleでもEmailでもできた。

ではそれで取得したトークン？とかをどうやって権限管理に使ったらいいのか分からない…？

**Links to work:**  
- なし


### Day 22: September 14, 2019

**Today's Progress:**  
- Actions on Google 開発
  - Firebase Authentication

サンプルを動かしてみる？  
[FirebaseExtended/firechat: Real-time Chat powered by Firebase](https://github.com/FirebaseExtended/firechat)

と思ったけど、なんか違う感じがする…？firechatというもう出来上がってるプロダクト（Firebase authとかRealtime Databaseとかを使ってる）を導入する方法の説明みたいな気がする。

FirebaseUI というのが用意されていて、ログインUIはこれを使うのがよさそう。  
https://github.com/firebase/firebaseui-web

YouTubeのFirecastもあった。  
[Using FirebaseUI Auth, on the Web - Firecasts - YouTube](https://www.youtube.com/watch?v=hb85pYZSJaI)

ちょっとまだ情報を探して迷走中。

**Links to work:**  
- なし


### Day 23: September 15, 2019

**Today's Progress:**  
- CSSでfloatで動かした要素がクリックできない問題
- Fontawesomeのアイコンを重ねる方法

最近一緒に勉強してくれてるリアル友人のコードでうまくいかないと聞いた所を調査。  
自分の発想になかったことを調べるきっかけになってとても勉強になった…！  
そして私CSS苦手なんだなと実感（笑）

クリックできない問題は `z-index` の指定で解決。

見せてもらったページで FontAwesome のアイコンに文字を重ねてかわいいボタンを作っていて、何これどうやってるの…！？と調べた。私にはその発想自体が無かった…！

参考：  
- [Font Awesomeのファイルアイコンの中にテキストを追加する - Qiita](https://qiita.com/nyu/items/eed05030975bd625911c)
- [Stacking Icons | Font Awesome](https://fontawesome.com/how-to-use/on-the-web/styling/stacking-icons)

**Links to work:**  
- なし


### Day 24: September 16, 2019

**Today's Progress:**  
- Firebase Auth について勉強

下記の動画を見て、

[Controlling Data Access Using Firebase Auth Custom Claims (Firecasts) - YouTube](https://www.youtube.com/watch?v=3hj_r_N0qMs)  
[Security Rules! 🔑 | Get to Know Cloud Firestore #6 - YouTube](https://www.youtube.com/watch?v=eW5MdE3ZcAw)

こちらのCodelabに手を付け始めましたが、ちょっと行き詰まってる感。

[Firebase Admin SDK Codelab](https://codelabs.developers.google.com/codelabs/firebase-admin/#0)

CodelabのサンプルがNode.js のバージョンが古い物にしか対応していなかったので、nvmでバージョンを切り替えるのに挑戦。それはうまくいきました。

**Links to work:**  
- なし


### Day 25-27: September 17-19, 2019

**Today's Progress:**  
- 既存サイトのURL移転

昨年作って公開したサイトのドメインの更新時期が迫ってきたのですが、対してアクセスもないので他で使っているドメインに統合しようと移転作業。
まるっと複製して、301リダイレクトを設定して、Googleアドレス変更申請。

明日からまたGoogle Assistantの作業に戻ろうと思います～。

**Links to work:**  
- 自作ツール: https://tools.charonworks.com/


### Day 28: September 20, 2019

**Today's Progress:**  
- Codelabの続き

[Firebase Admin SDK Codelab](https://codelabs.developers.google.com/codelabs/firebase-admin/#0) の続きを進めていたのですが、 `npm run dev` でどうもNode.jsにうまくPathが通ってないような感じのエラーが発生する。

元々開発に手を付けていたバージョンでは `firebase serve` もうまく動いていたので、このエラーの解消の調査は今学習したいことから逸れていきそうだな…と思ったので、ドキュメントを読んで進める方向に方向転換しようと思います。なかなか迷走している…

**Links to work:**  
- なし


### Day 29: September 21, 2019

**Today's Progress:**  
- [Cloud Firestore セキュリティ ルールを使ってみる  |  Firebase](https://firebase.google.com/docs/firestore/security/get-started)

こちらの動画 [Security Rules! 🔑 | Get to Know Cloud Firestore #6 - YouTube](https://www.youtube.com/watch?v=eW5MdE3ZcAw) の内容をおさらい。だいぶ理解できてきた。

Cloud Firestoreの firestore.rules には、認証情報によるルールだけでなく、リクエストのデータの内容・DBにあるデータの内容を参照してバリデーションのようなルールも設定できるとか。使い方少しずつイメージできてきた気がします。

**Links to work:**  
- Blog: [Firebase Auth、Cloud Firestoreのセキュリティルールについてメモ - On the New Orbit](https://ontheneworbit.blogspot.com/2019/09/firebase-authcloud-firestore.html)


### Day 30: September 22, 2019

**Today's Progress:**  
- 自分のプロジェクトにFirebase Authを使用したルールを設定してみる

Firebase CLI を使用してルールをデプロイしたり、JavaScriptのコード内で `firebase.auth().currentUser.uid` でuidを取得してその値をCloud Firestore のDBに保存したりするやり方を試しました。

参考にしたドキュメント
- [ルールのデプロイ > Firebase CLI を使用する](https://firebase.google.com/docs/firestore/security/get-started#use_the_firebase_cli) 
- [Firebase のユーザーを管理する](https://firebase.google.com/docs/auth/web/manage-users?hl=ja#get_the_currently_signed-in_user)

Visual Studio Code に Firestore の .rules ファイル用の拡張機能があるのを発見。  
- [Firestore Rules - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=ChFlick.firecode)

**Links to work:**  
- [Set up Firebase auth · sidemt/kokuchitant@5081251](https://github.com/sidemt/kokuchitant/commit/5081251c0d7f06922457d93b444414080424cff3) (Private Repo)


### Day 31: September 23, 2019

**Today's Progress:**  
- Hostingにデプロイして同じ操作ができることを確認
- ログイン中のユーザーの告知を取得する

Loadボタンを押したタイミングで、ログインしているユーザーのuidを `firebase.auth().currentUser;` で取得し、それを元にクエリを作成して読み出すことに成功。

document ID を指定すると1件の `.get()` でdocumentだけが取得されるけど、 collectionに対してクエリを実行すると `.get()` で得られるのが複数件のdocumentの集合なのでforEachで回して読み取らないといけないのが、前にも同じところで躓いた気がする。

参考  
[コレクションから複数のドキュメントを取得する](https://firebase.google.com/docs/firestore/query-data/get-data?hl=ja#get_multiple_documents_from_a_collection)

JavaScript難しい…何度理解したと思っても少し書かない期間が空くと全部忘れてしまう…。

**Links to work:**  
- なし


### Day 32: September 24, 2019

**Today's Progress:**  
- Firebaseのプロジェクトを新しく立て直す

今使用しているプロジェクトが1年ほどまえに試作していたものをそのまま使っていて、Location(Region)がUSが選択されていたのですが、現在はTokyoが選べるようになっていて、後々使い続けるとしたら今のうちにTokyoに変更しておいた方が良さそうだったので、プロジェクトを新しく立て直すことにしました。  
（Locationだけ変更はできなかった）

ここまで対応した内容。まだ途中です。

- Firebase console から新しい名前のプロジェクトを取得
- Cloud Firestoreの使用開始→なぜかエラーになる（「不明なエラーが発生しました」）→タイムラグがあるのか、10分程度時間が経つとエラーが解消された。
- Google Cloud Platform consoleにもFirebase Consoleから登録した新しいプロジェクト名が表示されなかったが、同じくらいのタイミングで表示されるようになった。
- `.firebaserc` で指定されているデフォルトプロジェクト名を、新しいプロジェクト名に書き換えてから `firebase init`

**Links to work:**  
- なし


### Day 33: September 25, 2019

**Today's Progress:**  
- Firebaseのプロジェクトを新しく立て直す(完了)

元々動いていた機能を一通りコピーできました。

対応内容↓

- Dialogflowプロジェクトの作り直し、Restore
- Actions API の認証情報（サービスアカウントキー）の再設定
- Firebase Functions のデプロイ
- Function URLをDialogflowに設定し直し
- Firebase構成情報の設定し直し
- Firebase Authenticationを有効化

あとは Function の Region も設定しなおさなければ。

**Links to work:**  
- なし


### Day 34: September 26, 2019

**Today's Progress:**  
- Firebase FunctionのRegionの変更

変更できました。今日は仕事関係を結構がんばってしまってあまりこちらは進められずという感じですが…。
結構会話の応答が遅い感じするので、Region変えたら速くなるかなとちょっと期待していたのですが、体感で分かるほどは速くならなかったです（笑）

ひとまず新プロジェクトへの移行作業は完了！

**Links to work:**  
- [Change project by sidemt · Pull Request #3 · sidemt/kokuchitant](https://github.com/sidemt/kokuchitant/pull/3)


### Day 35-36: September 27-28, 2019

**Today's Progress:**  
- `<script>` タグに書いていたコードを `.js` ファイルに分離
- サインイン後、新しい告知を保存後のタイミングで保存されている情報を画面に表示するようにした
- ESLintの導入

`<script>` タグでHTMLファイルに直書きすれば動くのに、.jsファイルに分離すると動かない、という状況によく陥るのですが、おそらく `$(document).ready` を入れるべきなのに入れてない、という状況が多いのかなと…。

下記の記事の、

> `</body>` タグの直前にscriptを入れる場合、$(docment).readyは必要ない

という部分で理解できました。

[JavaScript・jQueryの改修・高速化のためのメモ - Qiita](https://qiita.com/redamoon/items/1c38ee93834588e3c4ff#documentready%E3%82%92%E5%88%A9%E7%94%A8%E3%81%99%E3%82%8B)

またしばらく経つと忘れてしまいそう…！

**Links to work:**  
- なし


### Day 37-38: September 29-30, 2019

**Today's Progress:**  
- FirebaseUIの導入
- ログイン後、他のページに遷移させてみる
- 他のページでもログイン後の情報を利用してみる

JavaScriptの読み込み順、実行順でとにかく引っかかっているなと思います。  
ドキュメントを上から順に読んでその通りに並べても動かなくて、どこでinitializeしたインスタンスをどこで使って…というのを意識して読み込み順を整理すると動くようになりました。

ログイン後別のページにリダイレクトさせた際、 `firebase.auth()` の情報はどうやって引き継いだら…？と思ったのですが、普通に別ページにもfirebaseをinitializeするコードを入れて `firebase` が使えるようにすると、引き継ぐことができました。

どこまで引き継がれるかはここら辺で設定できるのかな？  
[認証状態の永続性](https://firebase.google.com/docs/auth/web/auth-state-persistence?hl=ja)

Google, Twitter, Email+Password でログインフローが動作することを確認。

**Links to work:**  
- [Create login flow by sidemt · Pull Request #4 · sidemt/kokuchitant](https://github.com/sidemt/kokuchitant/pull/4)


### Day 39-40: October 1-2, 2019

**Today's Progress:**  
- Firebase Functions ローカル開発環境の構築方法をブログに
- nodemon が起動できないエラーの調査

やってみてすごく便利！と思ったのでブログに書こう書こうと思っていた、 Firebase Functions のローカル環境の作り方をブログにまとめました。
最初に設定したときから1か月くらい経ってしまっていたので、色々バージョンアップしたせいかサーバーが起動できなくなっており…。

結局エラーメッセージからは全然予想しなかった設定で解決しました。だいぶ悩みました…。解決してよかった！

**Links to work:**  
- Blog: [Actions on Googleで使うFirebase Functionsの開発用ローカルサーバーを作る - On the New Orbit](https://ontheneworbit.blogspot.com/2019/10/actions-on-googlefirebase-functions.html)
