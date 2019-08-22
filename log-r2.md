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

**Link to work:**  
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

**Link to work:**  
- paiza: [Webセキュリティ入門編1 修了証](https://paiza.jp/works/lesson_certifications/nCzszE-gJUFIFQ)
- Blog: [GitHub から Security Alert が来たので package.json をアップデートする - On the New Orbit](https://ontheneworbit.blogspot.com/2019/08/github-security-alert-packagejson.html)  
- GitHub: [sidemt/pomcal: Pomodoro timer integrated with Google Calendar](https://github.com/sidemt/pomcal)
