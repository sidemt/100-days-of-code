# 100 Days Of Code - Log

### Day 1: August 22, 2018

**Today's Progress:**  
- Created Users controller and User model

I'm creating a web app to test clear cache function of a web browser.  
Something like this: https://enigmatic-anchorage-96854.herokuapp.com/

It intentionally caches the image for testing purpose.  
I'm thinking this app can be used to test whether a browser's clear cache function is working or not.  
(My current job is a tester and I have been testing a web browser app recently. That's why I got interested in building this.)

I created the page above by modifying the toy_app sample in Rails Tutorial, so it has many unnecessary functions/codes.

Now I'm trying to develop it while going through the tutorial from Chapter 3, but this time trying to understand "which code does what" more clearly, and customize it to suit my purpose.

**Link to work:** [Image Cache Test App](https://github.com/sidemt/image_cache_test)


### Day 2: August 23, 2018

**Today's Progress:**  
- Enable SSL
- Add settings to use Puma on prod (heroku) environment
- Create show/create user actions


**Link to work:** [Image Cache Test App](https://github.com/sidemt/image_cache_test)


### Day 3: August 24, 2018

**Today's Progress:**  
- Create login/logout function

**Link to work:** [Image Cache Test App](https://github.com/sidemt/image_cache_test)


### Day 4: August 25, 2018

**Today's Progress:**  
- Create edit/delete user functions
- Create functions related to admin user

**Thoughts:**  
I decided to join #100DaysOfCode challenge!  
I'm a 三日坊主 person, but it is now Day 4 and Github contributions graph is showing 8 Days streak (thanks to timezone difference) I started feeling like I can do it.

**Link to work:** [Image Cache Test App](https://github.com/sidemt/image_cache_test)


### Day 5: August 26, 2018

**Today's Progress:**  
- Implement Micropost
- Disable User & Login features

**Thoughts:**  
I realized that I might not need the User & Login features for my purpose... So I disabled them.
I might remove unnecessary codes later, but I learned a lot from implementing them. Deeper understanding helped me implementing Micropost feature.

**Link to work:** [Image Cache Test App](https://github.com/sidemt/image_cache_test)I know it is a simple app, and it is not perfect at all, but I believe I have made a progress by making my work public.


### Day 6: August 27, 2018

**Today's Progress:**  
- Image upload function
- Force cache the uploaded image so that the user needs to hard refresh the browser to see the new image

**Thoughts:**  
I completed implementing all the features I wanted.  
I will do some more layout work tomorrow, and then I will make it public.

It is very inspiring to see everyone tweeting using #100DaysOfCode . 自分がチャレンジに参加するまではそんなに感じなかったのですが、急に身近にというか、当事者の気持ちになるものですね。

**Link to work:** [Image Cache Test App](https://github.com/sidemt/image_cache_test)  


### Day 7: August 28, 2018

**Today's Progress:**  
- Completed the development and deployed it to Heroku

**Thoughts:**  
Deployed my first product in this challenge!  
I know it is a simple app, and it is not perfect at all, but I believe I have made progress by making my work public.  

**Links to work:**  
[Clear Cache Test App](https://clear-cache-test.herokuapp.com/)  
[GitHub Repo](https://github.com/sidemt/image_cache_test)  


### Day 8: August 29, 2018

**Today's Progress:**  
- Submitted a pull request to 100-days-of-code repo

**Thoughts:**  
I'm not sure if working on Markdown can be counted as coding, but I wanted to experience the workflow of submitting a pull request to forked repo.  
Now I have gained some confidence and understanding in it.

Reference on how to submit a pull request to forked repo (Japanese):  
[GitHubを使った開発フロー(初心者用) - Qiita](https://qiita.com/naogify/items/a5d1dccc89c5e96abed6)

**Link to work:**  
[Improve Japanese translation by sidemt · Pull Request #193 · kallaway/100-days-of-code](https://github.com/kallaway/100-days-of-code/pull/193)


### Day 9: August 30, 2018

**Today's Progress:**  
- Found out where the width is set
- Installed some packages to customize Sublime Text

**Thoughts:**  
I didn't have much progress today.  
I'm trying to improve the mobile view of my blog. The template is complicated and I spend long time to understand how it is working.

**Link to work:**  
[GitHub](https://github.com/sidemt/blogger-template/tree/responsive-design)


### Day 10: August 31, 2018

**Today's Progress:**  
- Learned about viewport
- Made the grid work

**Thoughts:**  
It is now Day 10!  
Blogger のテンプレートのカスタマイズは思った以上に難しくて、やめた方がいいのかなという気がしてます。  
メニューの配置とかは変えられたのですが、謎のpadding, margin, widthがあるのか、変はみ出してしまうところがどこから指定されてるのかわからず…。

他に作りたいものも出て来たので、明日以降どうするかちょっと考えます。

ただ、media query を指定して、PCブラウザのサイズを変更したときは効くのに開発者ツールや実機でスマホ画面にすると効かないときは、viewportの設定が必要ということがわかったのは収穫でした。  
Bloggerのテンプレートだと、if文で、Blogger側の「モバイルテーマを表示する」設定がOFFになっているとViewportがレスポンシブ用に設定されないようになってるっぽかったです。

**Link to work:**  
[GitHub](https://github.com/sidemt/blogger-template/tree/responsive-design)


### Day 11: September 1, 2018

**Today's Progress:**  
- Feasibility study on next project

**Thoughts:**  
I leave the blogger template as for now, and work on next project.  
I want to create a web app which searches for #100DaysOfCode tweets of users who are on the same day as you.  
So I did some research on how to use Twitter API. It looks like using Ruby on Rails is good for this app too.  

ちょっと不眠の波が来ていて2,3時間睡眠が続いているのですが、逆に言うとそのおかげで時間がとれているというか…。

**Link to work:**  
[Blog](https://ontheneworbit.blogspot.com/2018/09/twitter-api.html)


### Day 12: September 2, 2018

**Today's Progress:**  
- Research on Twitter API
- Tried 'twurl' and 'twitter' gem

**Thoughts:**  
Still doing a research on Twitter API, not having much progress.  
It seems the embedding search timeline is disabled recently. I'm not sure if I can find a way to implement a function similar to it.  
Found a gem called 'twitter', and it seems I can get Tweet id of the tweets I want to display on my web page. I need to find out how I can generate embedded tweet from the Tweet id.

**Link to work:**  
[Blog](https://ontheneworbit.blogspot.com/2018/09/twitter-api-2.html)


### Day 13: September 3, 2018

**Today's Progress:**  
- Research on Twitter API
- Found out how to:
  - Search tweets using twitter gem
  - Generate a snippet to embed a tweet using oEmbed API
  - Call oEmbed API using rest-client gem
  - Display embedded tweet using widgets.js

**Thoughts:**  
I think I found a way out. 昨日まで行き詰まってたところが乗り越えられた気がします。  
明日から少しずつ実際に組み立て始められたらいいな。

**Link to work:**  
[Blog](https://ontheneworbit.blogspot.com/2018/09/twitter-api-3.html)


### Day 14: September 4, 2018

**Today's Progress:**  
- Found out how to:
  - Display html code retrieved from JSON (.html_safe) 
  - Store secret keys in environment variables

**Thoughts:**  
I think now I have figured out everything I needed, so I want to start building actual app tomorrow.

**Link to work:**  
[Gist](https://gist.github.com/sidemt/abec0436d7bc03f54bd9334f6eae9209)


### Day 15: September 5, 2018

**Today's Progress:**  
- Applied for a developer account of Twitter (And accepted successfully)
- Setup for a new rails project and started creating the first static pages
- Installed RuboCop
- Installed Guard

**Thoughts:**  
The application process for a developer account of Twitter was way easier than I thought. (審査とかあるのかと思ってましたが、おそらく入力項目が増えただけで、アカウント自体はすぐ作れました。個人アカウントだからかもしれませんが。)  

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)
[Study With Me live stream](https://youtu.be/G8OMWuY3kK8)


### Day 16: September 6, 2018

**Today's Progress:**  
- Search and get tweet IDs

**Thoughts:**  
I'm still confused where to write codes under model/controller/helper.  
This page ([Plain Old Ruby Objects](https://www.learnhowtoprogram.com/rails/building-an-e-commerce-site-with-ajax-and-apis/plain-old-ruby-objects)) is helping me a lot, but I'm afraid I have some misunderstanding.

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 17: September 7, 2018

**Today's Progress:**  
- Embed tweets of search results

**Thoughts:**  
I always forget how to get a value from a form... struggling with it now.

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 18: September 8, 2018

**Today's Progress:**  
- Add a function to allow the user to select the Day

**Thoughts:**  
I tried to use Ajax for the form but it didn't work with the Twitter widgets.js. So I created a separate page to show the search results.

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)

### Day 19: September 9, 2018

**Today's Progress:**  
- Apply Bootstrap
- Adjust page design and layout

**Thoughts:**  
I'm trying to think mobile-first, but it's still difficult for me.

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 20: September 10, 2018

**Today's Progress:**  
- Set environment variables on Heroku
- Deploy to Heroku as phase 1
- Start inplementing User feature
  - Implement Twitter sign up/sign in using Devise

**Thoughts:**  
It's Day 20!! I didn't think I could do this.

I implemented Twitter sign up with help of the page below. This is the most simple and easy to understand guide for me.  
[認証機能(Devise/Twitter) | Rails Training](https://sadah.github.io/rails-training/ja/003_devise.html)

こちらのページを参考に1年前（初めてRailsを触った頃）にもTwitter認証の実装をやったのですが、今回他のサイトを参考にしてうまくいかなくて、ブックマークしてなかったものでどこだったっけと探し回ってなんとか見つけられたおかげで今回もうまくいきました！

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 21: September 11, 2018

**Today's Progress:**  
- Add "day" column to User model
- Resolve an error in tests

**Thoughts:**  
I got an error saying "ActiveRecord::RecordNotUnique:" in all tests after I created User model using Devise. The default fixture file was causing it.

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)  
[Blog](https://ontheneworbit.blogspot.com/2018/09/devise-activerecordrecordnotunique.html#links)


### Day 22: September 12, 2018

**Today's Progress:**  
- Research how to write tests for the user created with Devise
- Write login/logout tests

**Thoughts:**  
There are a lot of questions coming up!

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 23: September 13, 2018

**Today's Progress:**  
- Created "My Page" for logged in users
- Wrote tests for it

**Thoughts:**  
Rails Tutorialで見たな、という内容と、実装中の内容に合わせて自分が書いたテストと、RuboCopの設定とか、これまでちまちまと集めて来た知識がうまいことはまってつながった感覚があった。  
before_action の追加を忘れかけてたのをうまいことテストで検出できた。

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 24: September 14, 2018

**Today's Progress:**  
- Created a form to change the "Day" of the user

**Thoughts:**  
Form がまだ苦手だ…。POSTする先とかの理解がふんわりしているせいだとは思うんですが。

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 25: September 15, 2018

**Today's Progress:**  
- Added tests for user model
- Created a button to count up by 1 day

**Thoughts:**  
Now it's Day 25!! Quarter of 100!  
I took long time to figure out how to implement this button to count up by 1. hidden_field solved it.

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 26: September 16, 2018

**Today's Progress:** 
- Layout Improvements
  - Nav bar
  - Added progress bar
- Changed to redirect to my page after sign in
- Some research on how to test sign in behavior of devise

**Thoughts:**  
Deviseのログイン時の挙動を自動テストでテストしたいけれど、方法がわからない。  
調べてばかりで前に進まない気配がしたので、一旦置いておく。  
本家のREADMEをちゃんと読んでなかったばっかりにひっかかってたところがあったので（Rails5で書き方が変わっていた）気を付けたい！  

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 27: September 17, 2018

**Today's Progress:** 
- Layout Improvements
  - Remove unnecessary spacing
  - Refactor the code to display the flash message
- Another project (create a landing page sample)

**Thoughts:**  
いつものRailsのプロジェクトは1時間くらいやって、ちょっと他に作りたいものがでてきてそちらに時間を割いてたり。  
そっちに気を取られて未完成で放り出したりしないようにだけ気を付けねば！

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 28: September 18, 2018

**Today's Progress:** 
- Added some codes to handle the cases of Day0, 100, nil
- Added a celebration message for Day100
- Added a guide message for first time users
- Disabled unused action and devise modules
- Added validation to day value
- Done all these things while writing tests for them
- Deployed to Heroku as phase 2


**Thoughts:**  
Deployed, with features to login and track the Day. Check out if you are interested!  
[On The Day](https://on-the-day.herokuapp.com/)

There are still many things I want to improve, but I want to do another project too. So I decided to deploy it as phase 2 now.  
In the future I want to implement a function to tweet from the app, and as you tweet it counts up the Day automatically.  

And also it has a bug I cannot find how to solve it yet, I filed a issue for it not to forget it.  
[Sometimes embedded tweets are not rendered using widgetjs · Issue #6 · sidemt/on_the_day](https://github.com/sidemt/on_the_day/issues/6)

**Link to work:**  
[On The Day](https://on-the-day.herokuapp.com/)  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 29: September 19, 2018

**Today's Progress:** 
- Created a simple landing page with Bootstrap carousel

**Thoughts:**  
Created a simple page. Back to basics.  
I always think "justify-content" and "align-items" of flexbox in wrong way and get stuck...  

**Link to work:**  
[Tweet (with screenshot of the page)](https://twitter.com/siideemt/status/1042168457012248576)


### Day 30: September 20, 2018

**Today's Progress:** 
- Created another landing page with Bootstrap grid system

**Thoughts:**  
Now it's Day 30!!  
I'm trying to create some variations of simple landing pages.  
I think I understand the Grid system better than before.

**Link to work:**  
[Tweet (with screenshot of the page)](https://twitter.com/siideemt/status/1042550852232208384)


### Day 31: September 21, 2018

**Today's Progress:** 
- Created another landing page with Bootstrap grid system, using order class

**Thoughts:**  
Now I have created 3 different design in 3 days! (Although they are all simple and easy ones)  
And an interesting thing is happening:) Excited!

**Link to work:**  
[Tweet (with screenshot of the page)](https://twitter.com/siideemt/status/1042893503657762817)


### Day 32: September 22, 2018

**Today's Progress:** 
- Added a Tweet button to My Page  
- Made it include the current day in the tweet text  

**Thoughts:**  
Added a Tweet button. It was easy (thanks to Twitter Publish)  
Now I want to automatically count up the Day when the user clicks Tweet button, likely it requires JS.

あとこの3日間で作ったLPをUnitStockに出品してみました。どなたか興味を持ってくださると嬉しい…

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 33: September 23, 2018

**Today's Progress:** 
- Changed the tweet text to include next day number  
- Implemented auto count up of Day when tweet button is clicked

**Thoughts:**  
I found out I don't need to use strong parameters when I don't use users' free input for updating the data.  

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 34: September 24, 2018

**Today's Progress:** 
- Made some improvements in layout
- Fixed the calculation of the next day when the user is on Day 100
- Refactored to use the calculation function everywhere
- Refactored to use mixin in scss
- Refactored to remove duplicated loading of twitter's widget.js

**Thoughts:**  
Tomorrow I will try to fix the issue of sometimes it does not render the embedded tweets properly. Then I might push it to Heroku.  
I want to change the design of the progress bar too.

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 35: September 25, 2018

**Today's Progress:** 
- Trying to fix a bug, but no yet solved

**Thoughts:**  
Embedded tweets are not rendered with widget.js when opening the page for the first time.  
I think the issue is similar to this:  
[javascript - How to make Twitter widget.js run properly on first page load using `link_to` with Turbolinks on Rails 5 - Stack Overflow](https://stackoverflow.com/questions/43213044/how-to-make-twitter-widget-js-run-properly-on-first-page-load-using-link-to-wi)  
But I cannot figure out how I can apply this code to my code.

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 36: September 26, 2018

**Today's Progress:** 
- Fixed the issue of widget.js not loading  
- Started improving progress bar design

**Thoughts:**  
I fixed the bug (not sure if it is the best way to fix, but at least it's working) and deployed my app to Heroku. Phase 3.

**Link to work:**  
[On The Day](https://on-the-day.herokuapp.com/)  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 36: September 26, 2018

**Today's Progress:** 
- Fixed the issue of widget.js not loading  
- Started improving progress bar design

**Thoughts:**  
I fixed the bug (not sure if it is the best way to fix, but at least it's working) and deployed my app to Heroku. Phase 3.

**Link to work:**  
[On The Day](https://on-the-day.herokuapp.com/)  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 37: September 27, 2018

**Today's Progress:** 
- Changed progress bar design

**Thoughts:**  
Changed the progress bar to progress "dots". I think now I have everything I wanted in this app, so I'm moving on to something different. When I learn new things I will come back and make improvements again.

**Link to work:**  
[On The Day](https://on-the-day.herokuapp.com/)  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)


### Day 38: September 28, 2018

**Today's Progress:** 
- Set up CodePen to use React

**Thoughts:**  
It took me an hour to configure CodePen for React! The URL added from the search box didn't work for me, instead, I needed to use the URLs from http://reactjs.org Getting Started docs.  
Now I start freeCodeCamp's Markdown Previewer challenge!

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/XxWrvK)  
[GitHub: sidemt/markdown-previewer](https://github.com/sidemt/markdown-previewer)


### Day 39: September 29, 2018

**Today's Progress:** 
- Implement basic functionalities of Markdown Previewer

**Thoughts:**  
I made all required test suites pass. I will improve the design from tomorrow.  
I had absolutely no idea how to do this until a few days ago. It's amazing. It's working. I wrote this code. It's so much fun to learn new things!!

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/XxWrvK)  
[GitHub: sidemt/markdown-previewer](https://github.com/sidemt/markdown-previewer)


### Day 40: September 30, 2018

**Today's Progress:** 
- Markdown Previewer: Improve the design
- Publish it on GitHub pages

**Thoughts:**  
It's now Day40 and I finished up a #freeCodeCamp project, Markdown Previewer!  
I never thought I could keep going with this challenge for 40 days in a row. I never thought I could build a Markdown previewer either.

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/XxWrvK)  
[GitHub: sidemt/markdown-previewer](https://github.com/sidemt/markdown-previewer)


### Day 41: October 1, 2018

**Today's Progress:** 
- freeCodeCamp's Drum Machine project
  - research for how to use HTML5 audio tag
  - research for how to make it play a sound on click
  - research for how to make it play a sound on key press

**Thoughts:**  
I had never used the audio tag of HTML5. When I learned HTML for the first time 15 years ago I think it was an era of HTML3 transitioning to 4. It feels like a new feature. lol  
I didn't know that http://cloudinary.com can manage not only images but also audio files! It can convert audio files to different format too. すごい。  
とりあえず必要そうなものをかき集めたのでここから組み立てていく。

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/LgVEdg)  
[GitHub: sidemt/drum-machine](https://github.com/sidemt/drum-machine)


### Day 42: October 2, 2018

**Today's Progress:** 
- freeCodeCamp's Drum Machine project
  - Made each key play a different sound
  - Made it show a different text on each key press

**Thoughts:**  
I'm copy&pasting almost the same codes 9 times... for each key. There must be a smarter way to do it.  
It also plays the sound on click, but it does not update the text. I'm now writing the onclick event as an attribute in an HTML tag. I think I need to do it in React.

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/LgVEdg)  
[GitHub: sidemt/drum-machine](https://github.com/sidemt/drum-machine)


### Day 43: October 3, 2018

**Today's Progress:**  
- freeCodeCamp's Drum Machine project
  - Reduced unnecessary repetition in the code
  - Implemented all functions to make the test suite pass

**Thoughts:**  
Looking back one of the freeCodeCamp lessons, [React: Pass a Callback as Props | Learn freeCodeCamp](https://learn.freecodecamp.org/front-end-libraries/react/pass-a-callback-as-props), I think I made some improvements by breaking down the code into components and passing common values as properties.  
Now I have all the tests pass, so I will start working on the visual design tomorrow.

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/LgVEdg)  
[GitHub: sidemt/drum-machine](https://github.com/sidemt/drum-machine)


### Day 44: October 4, 2018

**Today's Progress:**  
- freeCodeCamp's Drum Machine project
  - Implement visual design

**Thoughts:**  
Japanese flavored Drum Machine. Done! -> [Drum Machine](https://codepen.io/sidemt/full/LgVEdg/)  

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/LgVEdg)  
[GitHub: sidemt/drum-machine](https://github.com/sidemt/drum-machine)
