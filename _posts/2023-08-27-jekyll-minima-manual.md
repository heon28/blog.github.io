---
layout: post
title: "jekyll-minima-description"
autor: 
- 이병헌
---

### 1. 블로그 포스트 생성
To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter.   
추가로 카테고리와 작성자를 기록하고 싶다면, 다음과 같이 기록
```
---
categories: junk
author:
- Bart Simpson
- Nelson Mandela Muntz
meta: "Springfield"
---
```

### 2. Jkeyll 코드 스닛펫
(1) Jkeyll이 제공하는 코드 스닛펫
```markdown
{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}
```
{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

(2) 마크다운 자체 코드 스닛펫

```
<!-- ```ruby
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
``` -->
```

```ruby
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
```

### 3. 하이퍼링크 텍스트 기입하는 방법

```
Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll.
[jekyll-docs-linkurl]: http://jekyllrb.com/docs/home
```
위와 같이 기재하면, 마크다운에서는 'Jekyll docs'라는 텍스트에 하이퍼링크를 걸게되고, 링크를 변수로 설정하여 "[변수명] : 링크url" 과 같이 따로 기재해두면 됨!
위의 마크다운 코드를 아래에 출력하면, 다음과 같음!!

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll.

[jekyll-docs]: http://jekyllrb.com/docs/home

### 4. 마크다운
```
# H1 (h1)
## H2 (h2)
### H3 (h3)
*이탤릭체(Italic)* 는, <i>다앙한 방법으로</i> <em>기재할 수 </em>있음.
> 여기에 글을 쓰면 블록을 따로 음영화하여 강조하고 이탤릭체가 사용됨.
> 하지만, *위에서 사용한* <i>이탤릭체를</i> 한 번 더 <em> 기입하게 되면 </em>이탤릭체가 없어짐.

코드 스닛펫은 `code variable`를 이용 가능. 길게 사용할 시, back quote(=grave, 억음부호)를 3번 사용하면 됨
```
# H1 (h1)
## H2 (h2)
### H3 (h3)

*이탤릭체(Italic)* 는, <i>다앙한 방법으로</i> <em>기재할 수 </em>있음.
> 여기에 글을 쓰면 블록을 따로 음영화하여 강조하고 이탤릭체가 사용됨.
> 하지만, *위에서 사용한* <i>이탤릭체를</i> 한 번 더 <em> 기입하게 되면 </em>이탤릭체가 없어짐.

코드 스닛펫은 `code variable`를 이용 가능. 길게 사용할 시, back quote(=grave, 억음부호)를 3번 사용하면 됨


```
- unordered list1
- unordered list2

1. ordered list1
2. ordered list2

Title 1               | Title 2               | Title 3               | Title 4
--------------------- | --------------------- | --------------------- | ---------------------
lorem                 | lorem ipsum           | lorem ipsum dolor     | lorem ipsum dolor sit

Title 1 | Title 2 | Title 3 | Title 4
--- | --- | --- | ---
lorem | lorem ipsum | lorem ipsum dolor | lorem ipsum dolor sit
```
- unordered list1
- unordered list2

1. ordered list1
2. ordered list2

Title 1               | Title 2               | Title 3               | Title 4
--------------------- | --------------------- | --------------------- | ---------------------
lorem                 | lorem ipsum           | lorem ipsum dolor     | lorem ipsum dolor sit

Title 1 | Title 2 | Title 3 | Title 4
--- | --- | --- | ---
lorem | lorem ipsum | lorem ipsum dolor | lorem ipsum dolor sit