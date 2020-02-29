# HTML 문법

## 문서저장

* HTML문서는 Text 기반으로 작성하며 ‘파일명.html’ 로 저장한다.
* HTML언어는 대소문자를 구분하지 않는다.
  * 단 통일해서 쓰는 것이 좋다.

## 태그 \(Tag\)

태그\(Tag\)는 정보\(내용\)의 의미나 기능을 표시하는 방법이다.   
HTML은 W3C에서 정한 태그들을 사용하여 문서의 구조를 표현한다.

```markup
<TAG> 내용 </TAG>
```

```markup
<member>
    <id>1</id>
    <name></name>
    <age>20</age>
    <weight measure='kg'>70</weight>
</member>
```

* 태그는 각각 의미를 가지고 있다.
* open\(start\) 태그와 close\(end\) 태그 짝으로 이루어져 있다. 
  * 내용의 시작과 끝을 표현한다.
  * close 태그는 `/` 가 붙는다. \(`<id>`**`</id>`**\)
  * 내용이 없는 경우 `<TAG/>` 로 사용한다.
    * HTML 의 경우 `/` 는 생략 할 수 있다.
    * `<br/>` `<br>`
* 추가적인 의미는 태그의 속성을 사용한다.

### 태그의 속성\(Attribute\)

태그에 기능이나 의미를 추가 하기 위해 속성을 사용한다.

```markup
<TAG attribute="value" attribute="value"></Tag>    
```

```markup
<weight measure='kg'>70</weight>
<a href='http://www.naver.com'></a>
<img src=''>
```

