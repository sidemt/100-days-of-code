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


### Day 45: October 5, 2018

**Today's Progress:**  
- freeCodeCamp's JavaScript Calculator project
  - Created a component to render a key with given id and value (text)
  - Created a component to render a number key
  - Render number keys 0-9 using a for loop

**Thoughts:**  
Started building JavaScript Calculator for #freeCodeCamp project.  
Found out how to use a for loop in React. And what I've learned in the previous project is helping me so far!

For loop in React: [Reactでループする - Qiita](https://qiita.com/mo4_9/items/b88cea7dc68d682b45b6)

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/xyOZwx)  
[GitHub: sidemt/js-calculator](https://github.com/sidemt/js-calculator)


### Day 46: October 6, 2018

**Today's Progress:**  
- freeCodeCamp's JavaScript Calculator project
  - Assigned click events to number keys, AC, decimal dot

**Thoughts:**  
I'm having fun going through JavaScript docs looking for a way to handle the user input (String?) as calculation. Learning built in functions I didn't know.  

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/xyOZwx)  
[GitHub: sidemt/js-calculator](https://github.com/sidemt/js-calculator)


### Day 47: October 7, 2018

**Today's Progress:**  
- freeCodeCamp's JavaScript Calculator project
  - Implement input of mathematical operators
  - Implement execution of calculation

**Thoughts:**  
I used Function object which is said to work similar to `eval()` according to [eval() - JavaScript | MDN](https://developer.mozilla.org/ja/docs/Web/JavaScript/Reference/Global_Objects/eval) 
Like below:  
```
  calculate(str){
    if (str != undefined) {
      var f = new Function('return ' + str + ';');
      return f();
    } else {
      return 0; 
    }
  }
```

Still not sure when to use React and when Redux. To understand it, I'm trying to use Redux now.

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/xyOZwx)  
[GitHub: sidemt/js-calculator](https://github.com/sidemt/js-calculator)


### Day 48 October 8, 2018

**Today's Progress:**  
- freeCodeCamp's JavaScript Calculator project
  - Add state `calculation` which stores numbers and operators as an array

**Thoughts:**  
結局Reduxの理解が不足していて上手く使えず、Reactオンリーに戻ってみました。  

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/xyOZwx)  
[GitHub: sidemt/js-calculator](https://github.com/sidemt/js-calculator)


### Day 49 October 9, 2018

**Today's Progress:**  
- freeCodeCamp's Pomodoro Clock project
  - Created needed elements with specified ids
  - Created component to display remaining time in mm:ss format
  - Created a function to decrement break time

**Thoughts:**  
I completed JavaScript Calculator challenge yesterday! [JavaScript Calculator](https://codepen.io/sidemt/full/xyOZwx/)  
So I started working on Pomodoro Clock. The last challenge to get Front End Libraries Certification.  
I think the count down function can be implemented with using something similar to this technique: [How TO - JavaScript Countdown Timer](https://www.w3schools.com/howto/howto_js_countdown.asp)  

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/LgxNay)  
[GitHub: sidemt/pomodoro-clock](https://github.com/sidemt/pomodoro-clock)


### Day 50 October 10, 2018

**Today's Progress:**  
- freeCodeCamp's Pomodoro Clock project
  - Created a function to increment break length, decrement/increment session length
  - Started developing a function to countdown

**Thoughts:**  
It's Day50!! I'm proud that I have come here without missing a day. I didn't think I could do it.

Today I started developing the countdown function using setInterval and clearInterval.

- 4ヶ月前の私が書いたブログに助けられました。→ [On the New Orbit: コールバック関数を自分のために解説 (JavaScript)](https://ontheneworbit.blogspot.com/2018/06/javascript.html#more)  
これ↓
>引数として渡すときは、関数名の後に()を付けない。渡した時点で今すぐ実行するのではなく、関数の定義をhigher-order functionに渡すだけなので。

- clearIntervalで止まらない→ setInterval()の戻り値 `intervalID` をグローバルな変数で受け取っておいて、clearIntervalに渡してあげることで解決。  
参考: [window.clearInterval - Web API インターフェイス | MDN](https://developer.mozilla.org/ja/docs/Web/API/WindowTimers/clearInterval)

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/LgxNay)  
[GitHub: sidemt/pomodoro-clock](https://github.com/sidemt/pomodoro-clock)


### Day 51 October 11, 2018

**Today's Progress:**  
- freeCodeCamp's Pomodoro Clock project
  - Created a function to toggle Break/Session
  - Added beep sound to play when the timer reaches 0

**Thoughts:**  
At first, I tried `.fastSeek(0)` to rewind the audio element, but I had to use `.currentTime = 0` instead. Due to browser compatibility?  
Now all tests passed! I will start the visual improvement tomorrow.  

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/LgxNay)  
[GitHub: sidemt/pomodoro-clock](https://github.com/sidemt/pomodoro-clock)


### Day 52 October 12, 2018

**Today's Progress:**  
- freeCodeCamp's Pomodoro Clock project
  - Corrected usage of setState
  - Started working on visual design improvement

**Thoughts:**  
I read this article [How to become a pro with React setState() in 10 minutes](https://medium.freecodecamp.org/get-pro-with-react-setstate-in-10-minutes-d38251d1c781) and corrected my code.

I was doing this:
```
    let currentLength = this.state.breakLength;
    let newLength = currentLength - 1;
    if (newLength > 0) {
      this.setState({
        breakLength: newLength
      })
    }
```

But according to the article this seems better:
```
    if (this.state.breakLength > 1) {
      this.setState((state) => ({
        breakLength: state.breakLength - 1
      }))
      this.updateTimeLeft(BREAK);
    }
```

I think I need some revision on React and basic JavaScript to understand React properly.

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/LgxNay)  
[GitHub: sidemt/pomodoro-clock](https://github.com/sidemt/pomodoro-clock)


### Day 53 October 13, 2018

**Today's Progress:**  
- freeCodeCamp's Pomodoro Clock project
  - Implement responsive layout
  - Apply Google Fonts
  - Change background color according to Session/Break state
  - Changed the variable isRunning to one of the state properties

**Thoughts:**  
Finished the Pomodoro Clock project and earned the [Front End Libraries Certification](https://www.freecodecamp.org/certification/sidemt/front-end-libraries)!!  

**Link to work:**  
[CodePen](https://codepen.io/sidemt/pen/LgxNay)  
[GitHub: sidemt/pomodoro-clock](https://github.com/sidemt/pomodoro-clock)  
[GitHub Pages: Pomodoro Clock](https://sidemt.github.io/pomodoro-clock/)


### Day 54 October 14, 2018

**Today's Progress:**  
- Planning to create a portfolio page
- Some research on web hosting services and domain registrar
- Prepared my works on GitHub pages

**Thoughts:**  
日本のポピュラーなサービスを使った経験をしておいた方が良いと思っていて（そのサービスが良いにしても悪いにしても）、最初さくらインターネットで検討してたんですが（先日の北海道地震での対応が見事だったとの話も記憶に新しいので）ライトプランが年間一括しかないようなのでロリポップから始めてみようかな…？という方に傾いてます。  
実は独自ドメインは使ったことがないのでトライしたい。

**Link to work:**  
[GitHub Repo](https://github.com/sidemt/charonworks)  


### Day 55 October 15, 2018

**Today's Progress:**  
- Signed up for [https://lolipop.jp/](https://lolipop.jp/)
- Uploaded a temporary top page
- Started building the portfolio

**Thoughts:**  
FCCの最初の課題がポートフォリオで、まだ何も書くことないのにそんな無茶な…と思ったんですけれど（笑）  
いまだ自分がやったことに自信がないからか、何を書いたら良いのやら…となってしまう。やっぱり。  
それを自信をもってアピールできる力も大事だな…

**Link to work:**  
[GitHub Repo](https://github.com/sidemt/charonworks)  


### Day 56 October 16, 2018

**Today's Progress:**  
- 各プロジェクトにどんな情報を書くか、どう書けば見やすいか検討

**Thoughts:**  
Bootstrapのcardでまとめてみている。

各情報としては、身の回りの友人に劇団とか劇場・ライブハウスとかに繋がりある人が多いので、そういう劇団とかライブハウスとかのホームページとか作らせてもらえないかしらとぼんやり思っていて。  
まずはその層に見せるつもりで作ろう。と思っています。  

**Link to work:**  
[GitHub Repo](https://github.com/sidemt/charonworks)  


### Day 57 October 17, 2018

**Today's Progress:**  
- 各プロジェクトの情報を一通り記載

**Thoughts:**  
コードじゃなくて文章をどう書くかで詰まっています（笑）  
freeCodeCamp序盤で作った天気アプリとかWikipedia検索とかの方が、後の方で作ったポモドーロタイマーとかMarkdownエディタとかよりもプログラミング畑の人じゃない人にはうけそうだと気づいてページの上の方に持って来てみたり。  
どうしても裏で難しいことをやってるものを見せたくなるんですけど、今私がアピールしたい層に見せるにはそれじゃないんだと思う。たぶん。  

**Link to work:**  
[GitHub Repo](https://github.com/sidemt/charonworks)  


### Day 58 October 18, 2018

**Today's Progress:**  
- Implemented grid layout
- Added nav bar

**Thoughts:**  
Bootstrapのgridを使うたびに「今回初めて正しい使い方ができた気がする」と思ってるような…。毎回「あ！なるほどこうやって使うのか！」って思ってるというか。  

今回「ああなるほど」って思ったところのメモ  
- `col-4` を1列に3個並べようとするとき、 `margin` を追加してしまうと1列から溢れる
- `row` で囲った中にたくさんの(最終的に複数行にまたがって表示されてほしい) `col` を入れて、それぞれに `class="col-lg-4 col-md-6 col-sm-12"` と付けると、lgの時は1行に3つ、mdのときは2つ、smのときは1つずつ表示される。


**Link to work:**  
[GitHub Repo](https://github.com/sidemt/charonworks)  


### Day 59 October 19, 2018

**Today's Progress:**  
- Added a mail form
- Registered for a custom domain name

**Thoughts:**  
メールフォームを追加。

PHPのコードはフリーで配布されてる物を使わせていただきましたが（とにかくまずは実現出来る手段があることを試しておきたかったので。）  
そこにBootstrapのスタイルを適用したり、HTML5のrequired属性を追加したり。

使わせていただいたのはこちら  
[【MailForm01】PHPメールフォーム多機能版（著作権リンク無し）フリー（無料）｜PHP工房](https://www.php-factory.net/mail/01.php)

ドメイン名も取得して、設定の反映待ち。

**Link to work:**  
[GitHub Repo](https://github.com/sidemt/charonworks)  


### Day 60 October 20, 2018

**Today's Progress:**  
- Visual design improvements

**Thoughts:**  
よしできた！と思って自分のiPhoneでも確認してみたら、Safariで全然うまく表示できてないことが発覚（苦笑） Browser compatibility...

```
background-color: rgba(0,0,0, 0.4);
```

みたいに指定した不透明度が全く読み込まれず、表示されてない状態。

**Link to work:**  
[GitHub Repo](https://github.com/sidemt/charonworks)  


### Day 61 October 21, 2018

**Today's Progress:**  
- Fixed bugs of browser imcompatibility

**Thoughts:**  
ポートフォリオ的なページ作りました。  
昨日悩んでいたのは、iPhoneで見ると `rgb(165, 42, 0, 0.2);` みたいにopacityを指定した色が表示されない事だったんですが、単純に書き方が間違ってたっぽくて `rgba(165, 42, 0, 0.2);` とすると表示されました。

**Link to work:**  
[GitHub Repo](https://github.com/sidemt/charonworks)  
[http://www.charonworks.com](http://www.charonworks.com)  


### Day 62 October 22, 2018

**Today's Progress:**  
- Set up freeCodeCamp locally

**Thoughts:**  
Because I wanted to try working on a real-world project, I set up the development environment for freeCodeCamp. I'm getting some errors on install. Work in progress.


[Set up freeCodeCamp locally](https://github.com/freeCodeCamp/freeCodeCamp/blob/master/docs/how-to-setup-freecodecamp-locally.md)

**Link to work:**  
None


### Day 63 October 23, 2018

**Today's Progress:**  
- Set up freeCodeCamp locally (Work in progress)

**Thoughts:**  
Still trying to set up freeCodeCamp locally, but haven't been successful. I'm searching with the error messages and looking into the documentation again but cannot find the solution yet.

`npm rum bootstrap` is failing with an error saying "Failed at the commitizen@2.10.1 postinstall script." (I'm not sure if this is the main part)  

The installation has been unsuccessfull but it's good to know that a real-world project can involve such a large number of node_modules!  

[Set up freeCodeCamp locally](https://github.com/freeCodeCamp/freeCodeCamp/blob/master/docs/how-to-setup-freecodecamp-locally.md)

**Link to work:**  
None


### Day 64 October 24, 2018

**Today's Progress:**  
- Set up freeCodeCamp locally (Work in progress)
  - Solved an error and completed `npm run bootstrap`

**Thoughts:**  
I solved the error in `npm run bootstrap` but now I'm facing another error in the next step `npm run seed`. The same error has been filed as an issue in freeCodeCamp's GitHub repo recently so I might wait a few days to see how it goes. I will work on something else while waiting for it.  

[Set up freeCodeCamp locally](https://github.com/freeCodeCamp/freeCodeCamp/blob/master/docs/how-to-setup-freecodecamp-locally.md)

**Link to work:**  
[Commented on GitHub issue](https://github.com/freeCodeCamp/freeCodeCamp/issues/18459#issuecomment-432359734)


### Day 65 October 25, 2018

**Today's Progress:**  
- Resolved a conflict on the PR I submitted before
- Set up WSL to use as a development environment for Ruby on Rails

**Thoughts:**  
[My PR](https://github.com/kallaway/100-days-of-code/pull/193) (it is a small correction in translation) was having a conflict so I solved it. Hoping it to be merged.  

Also, started setting up the dev environment for dev.to . I set up WSL (Windows Subsystem for Linux) to use rbenv. (rbenv does not work on Windows... at least for me.) I hope it goes well.

**Link to work:**  
[Improve Japanese translation by sidemt · Pull Request #193 · kallaway/100-days-of-code](https://github.com/kallaway/100-days-of-code/pull/193)  


### Day 66 October 26, 2018

**Today's Progress:**  
- Completed the setup of freeCodeCamp dev environment

**Thoughts:**  
Finally, I have freeCodeCamp running on my local! There is no first timers welcome issue now but I'm hoping to contribute someday.

**Link to work:**  
None


### Day 67 October 27, 2018

**Today's Progress:**  
- freeCodeCamp's Timestamp Microservice project

**Thoughts:**  
まだよくわからないけどできた感がすごくて狐につままれたようってまさにこういう気持ちだなと…（笑）

**Link to work:**  
[Timestamp Microservice](https://topaz-cereal.glitch.me/)  
[Timestamp Microservice: Code](https://glitch.com/edit/#!/topaz-cereal)  


### Day 68 October 28, 2018

**Today's Progress:**  
- freeCodeCamp's Request Header Parser project

**Thoughts:**  
I could accomplish the user stories by adding just a few lines so I'm not sure if I'm doing it right...

**Link to work:**  
[Request Header Parser](https://dynamic-sand.glitch.me/)  
[Request Header Parser: Code](https://glitch.com/edit/#!/dynamic-sand)  


### Day 69 October 30, 2018

**Today's Progress:**  
- Revision on Timestamp Microservice project & Request Header Parser project

**Thoughts:**  
Compared my code and the example code and reviewed on what I thought I didn't understand clearly (where to write the code (which was server.js), callbacks and error handling). This video https://youtu.be/QnLBGxtteV8 helped me.

**Link to work:**  
None  


### Day 70 October 31, 2018

**Today's Progress:**  
- URL Shortener Microservice project at freeCodeCamp
  - Receive the URL posted from the form
  - Validate its format
  - Connect to the DB on mLab

**Thoughts:**  
I used 'url-regex' library to check if the URL is in a valid format, but it can't be used to check if the URL begins with `http(s)://` (it accepts URL without `http(s)://` if it begins with `www`). So I added a regex to check that part. 

```
function isValidUrl(url) {
  // 'url-regex' cannot check if the URL begins with 'http(s)://'
  const httpRegex = /^https?\:\/\//i;
  // Check if the URL begins with 'http(s)://' AND is in a valid URL format checked with 'url-regex'
  return httpRegex.test(url) && urlRegex({exact: true, strict: true}).test(url);
};
```

Useful link: regex checker - [RegExr](https://regexr.com/)

**Link to work:**  
[URL Shortener Microservice: Code](https://glitch.com/edit/#!/groovy-hydrofoil)  


### Day 71 November 1, 2018

**Today's Progress:**  
- Completed URL Shortener Microservice project at freeCodeCamp

**Thoughts:**  
It took me so long to figure out the response from mLab DB was not an object `{ original: "www.google.com" }` but an object in an array `[{ original: "https://www.freecodecamp.com" }]`  
I was trying to retrieve the original URL value by `result.original` or `result['original']` but kept getting `undefined` . I needed to do `result[0]['original']`

But thinking about callback was fun. It's difficult, but fun.  

**Link to work:**  
[URL Shortener Microservice](https://groovy-hydrofoil.glitch.me/)  
[URL Shortener Microservice: Code](https://glitch.com/edit/#!/groovy-hydrofoil)  


### Day 72 November 2, 2018

**Today's Progress:**  
- Review the URL Shortener Microservice project
- Start working on Exercise Tracker

**Thoughts:**  
Reviewed the URL Shortener project by comparing my code to the example code.  
I learned that I can separate the code into modules, just like we do in Ruby on Rails projects.

Then started working on the next project, Exercise Tracker.

**Link to work:**  
[Exercise Tracker: Code](https://glitch.com/edit/#!/metal-enquiry)  
