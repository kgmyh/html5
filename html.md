# HTML 기본 문법

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
  * 내용이 없는 경우 `<TAG/>` 로 사용한다. \(내용이 없는 태그는 **empty tag** 라고 한다.\)
    * HTML 의 경우 `/` 는 생략 할 수 있다.
    * `<br/>` 또는 `<br>`
* 추가적인 의미는 태그의 속성을 사용한다.

### 태그의 속성\(Attribute\)

태그에 기능이나 의미를 추가 하기 위해 속성을 사용한다.

```markup
<TAG attribute="value" attribute="value"></Tag>    
```

```markup
<weight measure='kg'>70</weight>
<a href='http://www.naver.com'></a>
<img src='/imgs/images.png'>
```

* value는 작은따옴표나 큰따옴표로 감싼다.
* 속성이 여러개일 때는  공백을 구분자로 나열하면 된다.
  * `<a href='/add'  class='btn'>`

### 태그의 계층 구조

태그는 내용으로 태그를 사용할 수 있다.  감싸는 태그를 부모태그/부모요소 라고 하고 내용으로 사용된 태그를 자식태그/자식요소 라고 한다.   
부모 태그와 자식태그는 계층 관계를 가진다. 즉 자식태그는 부모태그에 속하게 된다.

```markup
<부모태그>
    <자식태그> 내용 </자식태그>
</부모태그>
```

{% tabs %}
{% tab title="예1" %}
```markup
<ul>
    <li></li>
    <li><li>
    <li></li>
</ul>
```
{% endtab %}

{% tab title="예2" %}
```markup
<table>
    <tr>
        <td>ID</td>
        <td></td>
    <tr>
</table>
```
{% endtab %}
{% endtabs %}

첫번째 예의 경우 **`<ul>`** 태그는 목록을 만들때 사용하며 **`<li>`**는 목록내의 item을 만들때 사용한다. 목록안에 item들이 있으므로 `<ul> </ul>`  안에 `<li> </li>` 를 사용하고 item 내용을 &lt;li&gt;&lt;/li&gt; 안에 표시한다.    
이 구조에서 `<ul>` 은 부모 요소, `<li>` 는 자식 요소가 된다.

두번째 예의 경우 태그간의 계층 관계는 여러 단계로 표시할 수 있다.  
**`<table>`** 태그는 표를 만들때 사용하며 **`<tr>`**은 행을 표시하고 **`<td>`**는 열을 표시한다.  
`<table> </table>` 안에 `<tr></tr>` 이 있고 `<tr></tr>` 안에 `<td></td>` 가 있다.   




