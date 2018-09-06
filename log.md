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
This page ([Plain Old Ruby Objects]{https://www.learnhowtoprogram.com/rails/building-an-e-commerce-site-with-ajax-and-apis/plain-old-ruby-objects)) is helping me a lot, but I'm afraid I have some misunderstanding.

**Link to work:**  
[GitHub: sidemt/on_the_day](https://github.com/sidemt/on_the_day)
