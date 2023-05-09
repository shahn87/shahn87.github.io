---
layout: post
title:  "Jekyll 을 이용해 Github page 만들기"
date:   2023-05-09 23:09:08 +0900
categories: Develop
---
네이버 블로그를 이용해 일상 블로그를 하고 있다. (사람들에게 보여주기 위해서라기 보다는 단순 기록용으로.)
하지만, 왠지 네이버 블로그에는 개발 내용을 넣고 싶은 기분이 들지 않는다. 그래서 찾게 된 것이 바로 Github Page.

내가 Github Page 를 선택하게 된 두 가지 이유.
1. 무료로 사용할 수 있다.
2. 개발 블로그로 적격이다.

이제 바로 해보자.

Github page 를 만드는 방법 ([pages.github.com][pages-github] )
1. {username}.github.io 이름으로 github repository 를 만든다.
2. terminal 에서 repository 를 clone 한다.
{% highlight shell %}
git clone https://github.com/username/username.github.io
{% endhighlight %}
3. 프로젝트 폴더로 이동해서 index.html 파일을 만든다.
{% highlight shell %}
cd username.github.io
echo "Hello World" > index.html
{% endhighlight %}
4. Git 에 add, commit, push 한다.
{% highlight shell %}
git add --all
git commit -m "Initial commit"
git push -u origin main
{% endhighlight %}

위의 순서대로 실행하면, 1분만에 (변경이 완료될 때까지 기다리는 시간을 제외하고) 아래와 같은 화면을 볼 수 있다.
![hello world blog](/assets/2023-05-09-hello-world-blog.png)

쉽다 쉬워.

[pages-github]: https://pages.github.com/
