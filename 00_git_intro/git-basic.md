# 마크다운(MarkDown)

> 일단 텍스트 형식으로 다운을 사용하는 마크업 언어의 일종으로 사용이 쉽고 간결하다.
>
> 단, 모든HTML마크업을 대체하지 않는다.

## 1. 문법

### 1.1 Header

> 헤더는 제목을 표현할 때 사용합니다.
>
> 단순히 글자의 크기를 나타낼 때 사용하는 것이 아니라 의미론적인 중요도를 갖습니다.

- h1~h6 까지 표현이 가능합니다.
- #의 개수로 표현하거나 <h1></h1>형태로 표현 가능합니다.



### 1.2 List

> 목록을 나열할 때 사용합니다.
>
> 순서가 필요한 항목과 그렇지 않은 항목으로 구분할 수 있습니다.
>
> 순서/순서x 항목을 같이 사용할 수 있습니다.

- 순서가 없는 항목
  - 순서가 없는 하위 항목
  - 순서가 없는 하위 항목

1. 순서가 있는 항목
2. 순서가 있는 항목
   1. 순서가 있는 하위 항목
   2. 순서가 있는 하위 항목



- 순서가 없는 항목
  1. 순서가 있는 하위 항목



### 1.3 Code Block

> 코드 블럭은 작성한 코드를 정리하거나 강조하고 싶을 때 사용합니다.
>
> 코드 블럭은 인라인과 블럭 단위로 구분할 수 있습니다.

- Inline
  - 인라인으로 처리하고 싶은 부분을 `(백틱)으로 감싸줍니다.
- Block
  - (백틱)을 3번 입력하고 `Enter`을 눌러서 생성합니다.



```bash
$ git add .
$ git commit -m "commit message"
$ git push origin master
```



### 1.4 Image

> 로컬에 있는 이미지를 삽입하거나 이미지 링크를 활용하여 표시합니다.

- ![]() 를 작성하고 ()안에 주소를 입력합니다.
  - 이때 [] 안에는 이미지 이름을 입력합니다.
- 로컬에 있는 이미지 파일을 로드할 때는 절대 경로가 아닌 상대 경로를 사용합니다.

![박보영 사진](data:image/jpeg;base64,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)



![](.\Image\박보영 사진2.jpg)

### 1.5 Link

> 특정 주소로 링크를 걸 때 사용합니다.

- []() 를 작성하고 () 안에 링크를 걸 주소를 입력합니다.

[네이버](https://www.naver.com/)



### 1.6 Table

> 표를 작성하여 요소를 구분할 수 있습니다.

- `|(파이프)` 사이에 컬럼을 작성하고 `Enter` 를 입력합니다.
- 마지막 컬럼을 작성하고 뒤에 `|` 를 붙여줍니다.

| Working Directory | Staging Arear | Remote Repo |
| ----------------- | ------------- | ----------- |
| working tree      | INDEX         | history     |
| working copy      | cache         |             |
|                   |               |             |
|                   |               |             |
|                   |               |             |



### 1.7 기타

**인용문**

- `>` 를 입력하고 `Enter` 키를 누릅니다.

> git은 컴퓨터의 파일 변경 사항을 추적합니다.

- 중첩된 인용문을 사용할 수 있습니다.

> $ git add .
>
> > 
> >
> > $ git commit -m "first commit"

수평선

- `---`,`***`,`___` 를 입력하여 작성합니다.

Working Directory

---

Staging Area

___

Remote Repository(Github)



**강조**

- 이탤릭체는 해당 부분을 *,_ 1개로 감싸줍니다.
- 보드체는 해당 부분을 **,__ 2개로 감싸줍니다.
- 취소선은 ~~ 2개로 감싸줍니다.

이것은 *이텔릭체*입니다.

이것은 **보드체**입니다.

이것은 ~~취소선~~입니다.

