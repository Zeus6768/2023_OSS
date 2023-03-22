# 3주차 Git

## 이미지
![한국항공대학교](../img/kau/kau.png)

## 링크
[LMS](https://lms.kau.ac.kr)

### ProGit 링크
[ProGit](https://git-scm.com/book/en/v2)

## 주요 git 명령어
- add : 파일을 추적 대상으로 포함시킬 때, 또는 커밋 대상으로 포함시킬 때 사용
  - 예) git add
- commit
- branch
- merge
- status
- log
  - 예) git log --oneline --decorate --graph --all

## 2주차 과제
```bash
#!/bin/sh

LINE="----------"

echo $LINE
echo "name :\n신재우\n"

echo $LINE
echo "student id :\n2015123056\n"

echo $LINE
HOMEWORK=$(find /home/kau2 -name w2_homework.txt 2> /dev/null)
echo "\nfile path :\n$HOMEWORK\n"

echo $LINE
ROW=$(wc -l $HOMEWORK | cut -c 1)
echo "line number :\n$ROW\n"

echo $LINE
LAST=$(tail -n 1 $HOMEWORK)
echo "last line :\n$LAST"

exit 0
```

# 마크다운 사용법
## 제목(Header)

`<h1>`부터 `<h6>`까지 제목을 표현할 수 있습니다. 

    # 제목1
    ## 제목2
    ### 제목3
    #### 제목4
    ##### 제목5
    ###### 제목6

제목1(h1)과 제목2(h2)는 다음과 같이 표현할 수 있습니다.

    제목1
    =====

    제목2
    -----

<br><br><br>

## 강조(Emphasis)

<br>

    이탤릭체는 *별표(asterisk)* 혹은 _언더바(underscore)_를 사용하세요.
    두껍게는 **별표(asterisk)** 혹은 __언더바(underscore)__를 사용하세요. 
    **_이탤릭체_와 두껍게**를 같이 사용할 수 있습니다.
    취소선은 ~~물결표시(tilde)~~를 사용하세요.
    <u>밑줄</u>은 `<u></u>`를 사용하세요. 

이탤릭체는 *별표(asterisk)* 혹은 _언더바(underscore)_를 사용하세요.
두껍게는 **별표(asterisk)** 혹은 __언더바(underscore)__를 사용하세요. 
**_이탤릭체_와 두껍게**를 같이 사용할 수 있습니다.
***이탤릭체*와 두껍게**를 같이 사용할 수 있습니다.
취소선은 ~~물결표시(tilde)~~를 사용하세요.

<br><br><br>

## 목록(List)

<br>

    1. 순서가 필요한 목록
    2. 순서가 필요한 목록
       - 순서가 필요하지 않은 목록
       - 순서가 필요하지 않은 목록
    3. 순서가 필요한 목록
       1. 순서가 필요한 목록
       2. 순서가 필요한 목록
    4. 순서가 필요한 목록

    - 순서가 필요하지 않은 목록에 사용 가능한 기호
      - 대쉬(hyphen)
      * 별표(asterisk)
      + 더하기(plus sign)

1. 순서가 필요한 목록
2. 순서가 필요한 목록
   - 순서가 필요하지 않은 목록
   - 순서가 필요하지 않은 목록
3. 순서가 필요한 목록
   1. 순서가 필요한 목록
   2. 순서가 필요한 목록
4. 순서가 필요한 목록

- 순서가 필요하지 않은 목록에 사용 가능한 기호
  - 대쉬(hyphen)
  * 별표(asterisk)
  + 더하기(plus sign)

<br><br><br>

## 링크(Links)

<br>

    [GOOGLE] (https://google.com)

    [NAVER] (https://naver.com "링크 설명(title)을 작성하세요.")

    [상대적 참조] (../users/login)

    [Dribble] [Dribble Link]

    [Github] [1]

    문서 안에서 [참조 링크]를 그대로 사용할 수도 있습니다.

    다음과 같이 문서 내 일반 URL이나 꺽쇠 괄호(`< >`, Angle Brackets) 안의 URL은 자동으로 링크를 사용합니다. 
    구글 : https://google.com
    네이버 : <https://naver.com>

    [Dribble Link]: https://dribble.com
    [1]: https://github.com
    [참조 링크]: https://naver.com "네이버로 이동합니다."

[GOOGLE](https://google.com)

[NAVER](https://naver.com "링크 설명(title)을 작성하세요.")

[상대적 참조](../users/login)

[Dribble][Dribble Link]

[Github][1]

문서 안에서 [참조 링크]를 그대로 사용할 수도 있습니다.

다음과 같이 문서 내 일반 URL이나 꺽쇠 괄호(`< >`, Angle Brackets) 안의 URL은 자동으로 링크를 사용합니다.

구글 : https://google.com

네이버 : <https://naver.com>

[Dribble Link]: https://dribble.com

[1]: https://github.com

[참조 링크]: https://naver.com "네이버로 이동합니다."
