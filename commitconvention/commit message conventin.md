*[1. 협업을 위한 git 커밋컨벤션 설정하기](https://overcome-the-limits.tistory.com/entry/%ED%98%91%EC%97%85-%ED%98%91%EC%97%85%EC%9D%84-%EC%9C%84%ED%95%9C-%EA%B8%B0%EB%B3%B8%EC%A0%81%EC%9D%B8-git-%EC%BB%A4%EB%B0%8B%EC%BB%A8%EB%B2%A4%EC%85%98-%EC%84%A4%EC%A0%95%ED%95%98%EA%B8%B0)와 [2. 커밋 메시지 컨벤션 가이드](https://gist.github.com/stephenparish/9941e89d80e2bc58a153)와 [3. 커밋 메시지 규약 정리](https://velog.io/@outstandingboy/Git-%EC%BB%A4%EB%B0%8B-%EB%A9%94%EC%8B%9C%EC%A7%80-%EA%B7%9C%EC%95%BD-%EC%A0%95%EB%A6%AC-the-AngularJS-commit-conventions#scope%EC%97%90-%EB%93%A4%EC%96%B4%EA%B0%88-%EC%88%98-%EC%9E%88%EB%8A%94-%ED%95%AD%EB%AA%A9%EB%93%A4)를 참고했습니다.

## 커밋 메시지의 형식

```markdown
<type>(<scope>): <subject> - (제목)
<BLANK LINE> - (한 줄을 띄어 제목과 본문을 분리한다.)
<body> - (본문)
<BLANK LINE> - (한 줄을 띄어 본문과 꼬리말을 분리한다.)
<footer> - (꼬리말)
```

## 제목

1. 제목의 총 글자 수는 50자 이내로 작성한다.
2. 첫 글자를 **대문자**로 작성한다.

### **\<type>에 들어갈 수 있는 항목**

- Feat : 새로운 기능 추가
- Fix : 버그 수정
- Docs : 문서 관련
- Style : 스타일 변경 (포매팅 수정, 들여쓰기 추가, …)
- Refactor : 코드 리팩토링
- Test : 테스트 관련 코드
- Build : 빌드 관련 파일 수정
- Ci : CI 설정 파일 수정
- Perf : 성능 개선
- Chore : 그 외 자잘한 수정

### **\<scope>에 들어갈 수 있는 항목**

어디가 변경되었는지, 변경된 부분은 모두 들어갈 수 있다.

예를 들어, $location, $browser, $compile, $rootScope, ngHref, ngClick, ngView, 등등...

***\<scope>는 생략 가능.**

메소드 추가나 변경 사항이 있다면 해당 메소드의 클래스 이름을 적는 방법도 있다.

### \<subject>

변경 사항에 대한 간결한 설명을 포함한다. (무엇을 변경했는지, 어떻게 변경했는지)

## 본문

1. 본문은 **한 줄 당 72자 내**로 작성한다.

2. 본문 내용은 양에 구애받지 않고 **최대한 상세히 작성한다**.

3. 본문 내용은 **어떻게 변경했는지**보다 **무엇을 변경했는지** 또는 **왜 변경했는지** 를 설명한다.

## 꼬리말

1. 꼬리말은 optional이고 이슈 트래커 ID를 작성한다.

2. 꼬리말은 "유형: #이슈 번호" 형식으로 사용한다.
