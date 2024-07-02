# mbcac_team
## Windows에서 자격증명 확인 / github 관련 자격증명 삭제

## github.com 회원가입

## github 사이트에서 Repository 생성
* Repository 주소 복사
  
## git 다운로드/설치
* user.name / user.email 등록
  + git config -- global user.name="개인 아이디"
  + git config -- global user.email="개인 이메일 주소"
* cmd > git config --list : 등록된 항목 확인
  
## github 토큰 신청/발급
* github.com 화면 우측 상단 아이콘 클릭 > Settings > 왼쪽 메뉴 하단 Developer settings > Personal access tokens >
* Tokens(classic) > Generate new token > Generate new token(classic) >
* Note:간단 설명 입력 > Generate token

## 로컬 Repository 에 원격 리파지토리 복사
* 원격 저장소에 등록된 프로젝트를 최초로 로컬 저장소에 복제한다
* git init
* git clone [원격 저장소 주소]
* git config --list <-- origin 이라는 이름으로 원격 저장소의 주소가 등록된 것을 확인

## 로컬 저장소의 내용변경 및 원격 저장소에 병합(push)하기
* 로컬 저장소에 있는 파일을 변경하고 저장한다
* git add . : 현재 데렉토리(프로젝트 루트)에서 staging 작업 실행(업로드할 파일을 모은다)
* git status : 현재 상태 확인
* git commit -m "변경 내역에 기록할 메시지"
* git status
* git push -u origin main : origin은 원격 저장소의 주소에 대한 별칭으로 로컬에 설정된 상태임, main : 원격 저장소 브랜티 이름
* 위의 명령은 -u(--set-upstream) 설정, 인증을 위한 웹브라우저가 실행됨
* 웹브라우저 하단의 초록버튼을 누르고 화면이 전환되면 브라우저를 닫는다
* git 명렬을 실행하던 콘솔창을 닫고 다시 실행한다.
* git status 명령으로 git의 현재 작업 상태 확인
* 파일 변경 상태가 표시되지 않으면 대상 파일을 열고 다시 변경하고 저장한다
* git add . : 변경된 로컬 저장소의 내용을 staging
* git status : 변경된 파일이 git에 의해 표시되는지 확인
* git commit -m : "변경내역에 기록할 메시지"
* git status : 위에서 commit 한 정보가 확인되는지
* git push origin main :  최종적으로 로컬 프로젝트를 원격 저장소(origin)의 main 브랜치에 병합한다
* github.com 에 접속하여 해당 파일의 내용이 변경되어 있는지 확인한다
  






------------------------------------------------------------------------

## 팀 프로젝트 안내
* 주제: 열심히 하자
* 기간: 3달
  + 1달: 분석
  + 1달: 설계
  + 1달: 구현
    - 1주: 로그인
    - 2주: 게시판
    - 3주: 뉴스  
<a name="top"></a>
## 목차
1. [code1](#code1)    
2. [code2](#code2)  
3. [code3](#code3)  
4. [code4](#code4)  
5. [code5](#code5)  
6. [code6](#code6)  


## 아래의 코드를 참고하세요
```jsp 
<%@ page language="java" contentType="application/json; charset=UTF-8"
    pageEncoding="UTF-8" trimDirectiveWhitespaces="true"%>

<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>
<%@ taglib prefix="fmt" uri="http://java.sun.com/jsp/jstl/fmt" %>

<jsp:useBean id="dao" class="com.mbcac.board.BoardDAO"/>
<jsp:useBean id="board" class="com.mbcac.board.BoardVO">
	<jsp:setProperty name="board" property="*"/>
</jsp:useBean>
<c:set var="added" value="${dao.add(board)}"/>
{"added":${added}}
```

[github마크다운으로 색상 설정하기](https://gist.github.com/luigiMinardi/4574708d404cdf4fe0da7ac6fe2314db)
$\color{#ff0000}{\textsf{색상 설정}}$
<P>
	
<a name="code1">code1</a> [go to top](#top)
```jsp 
<%@ page language="java" contentType="application/json; charset=UTF-8"
    pageEncoding="UTF-8" trimDirectiveWhitespaces="true"%>

<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>
<%@ taglib prefix="fmt" uri="http://java.sun.com/jsp/jstl/fmt" %>

<jsp:useBean id="dao" class="com.mbcac.board.BoardDAO"/>
<jsp:useBean id="board" class="com.mbcac.board.BoardVO">
	<jsp:setProperty name="board" property="*"/>
</jsp:useBean>
<c:set var="added" value="${dao.add(board)}"/>
{"added":${added}}
```

<a name="code2">code2</a> [go to top](#top)
```jsp 
<%@ page language="java" contentType="application/json; charset=UTF-8"
    pageEncoding="UTF-8" trimDirectiveWhitespaces="true"%>

<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>
<%@ taglib prefix="fmt" uri="http://java.sun.com/jsp/jstl/fmt" %>

<jsp:useBean id="dao" class="com.mbcac.board.BoardDAO"/>
<jsp:useBean id="board" class="com.mbcac.board.BoardVO">
	<jsp:setProperty name="board" property="*"/>
</jsp:useBean>
<c:set var="added" value="${dao.add(board)}"/>
{"added":${added}}
```

<a name="code3">code3</a> [go to top](#top)
```jsp 
<%@ page language="java" contentType="application/json; charset=UTF-8"
    pageEncoding="UTF-8" trimDirectiveWhitespaces="true"%>

<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>
<%@ taglib prefix="fmt" uri="http://java.sun.com/jsp/jstl/fmt" %>

<jsp:useBean id="dao" class="com.mbcac.board.BoardDAO"/>
<jsp:useBean id="board" class="com.mbcac.board.BoardVO">
	<jsp:setProperty name="board" property="*"/>
</jsp:useBean>
<c:set var="added" value="${dao.add(board)}"/>
{"added":${added}}
```

<a name="code4">code4</a> [go to top](#top)
```jsp 
<%@ page language="java" contentType="application/json; charset=UTF-8"
    pageEncoding="UTF-8" trimDirectiveWhitespaces="true"%>

<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>
<%@ taglib prefix="fmt" uri="http://java.sun.com/jsp/jstl/fmt" %>

<jsp:useBean id="dao" class="com.mbcac.board.BoardDAO"/>
<jsp:useBean id="board" class="com.mbcac.board.BoardVO">
	<jsp:setProperty name="board" property="*"/>
</jsp:useBean>
<c:set var="added" value="${dao.add(board)}"/>
{"added":${added}}
```

<a name="code5">code5</a> [go to top](#top)
```jsp 
<%@ page language="java" contentType="application/json; charset=UTF-8"
    pageEncoding="UTF-8" trimDirectiveWhitespaces="true"%>

<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>
<%@ taglib prefix="fmt" uri="http://java.sun.com/jsp/jstl/fmt" %>

<jsp:useBean id="dao" class="com.mbcac.board.BoardDAO"/>
<jsp:useBean id="board" class="com.mbcac.board.BoardVO">
	<jsp:setProperty name="board" property="*"/>
</jsp:useBean>
<c:set var="added" value="${dao.add(board)}"/>
{"added":${added}}
```

<a name="code6">code6</a> [go to top](#top)
```jsp 
<%@ page language="java" contentType="application/json; charset=UTF-8"
    pageEncoding="UTF-8" trimDirectiveWhitespaces="true"%>

<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>
<%@ taglib prefix="fmt" uri="http://java.sun.com/jsp/jstl/fmt" %>

<jsp:useBean id="dao" class="com.mbcac.board.BoardDAO"/>
<jsp:useBean id="board" class="com.mbcac.board.BoardVO">
	<jsp:setProperty name="board" property="*"/>
</jsp:useBean>
<c:set var="added" value="${dao.add(board)}"/>
{"added":${added}}
```
