name: inverse
layout: true
---
class: middle, full-text
# goni

깃허브 실습


.footnote[
- 태풍 고니가 올라오는 저녁에..
- [발표자](https://www.facebook.com/kozazz): 곽두환
]

---
### 링크
- 미리 보시면 좋습니다.
- https://www.facebook.com/groups/datergram/

- http://datergram.github.io

- http://datergram.github.io/blog

- http://datergram.github.io/goni

- http://datergram.github.io/goni/slide

- https://github.com/datergram/goni

- https://github.com/datergram/goni/tree/gh-pages/slide

- https://github.com/mbostock/bl.ocks.org

- http://ilmol.com/2015/01/Jekyll,Git%20%EC%9D%84%20%EB%AA%B0%EB%9D%BC%EB%8F%84%20%EB%AC%B4%EB%A3%8C%20Github%20Pages%20%EC%A6%90%EA%B8%B0%EA%B8%B0.html

---
### 들어가기에 앞서
- 열정에 불을 지피다
- 오늘 개콘보다 재밌습니다
- 다 기억 못합니다
- 구경만 해도 좋습니다
- git은 웹에서 하는 것으로.. 좋은 툴도 많고, shell 명령어도 많습니다만 생략. 
- 원숭이깃 참고 http://backlogtool.com/git-guide/kr/intro/intro1_1.html
- git clone ,add ,commit , push, pull

---
### 끝나고 나면
- 평생쓸 홈페이지 주소가 생깁니다.
- script 코드를 올릴 공간을 가지게 됩니다. 
- 프로그래머 같은 기분이 듭니다.

---
### 왜 필요한가
- 중복의 안좋은 기억 메일로 공유하던 문서
- 보고서-1.txt 보고서-2.txt 보고서-최종.txt 보고서-final.txt
- 같은 파일은 하나만 존재하게 한다. 중복의 삭제
- 비슷한애들 
- 구글드라이브 , 클라우드, 블로그 vs git
- 뭐가 다른가 파일 단위 같이 협업?

---
### git
- vcs version control system. 
- 종류 cvs. svn. git
- git? github?
- 버젼관리란 동일 파일은 하나만 유지하자. 
- 공짜. 무제한
- 그대신 전부 오픈. 전화 번호, 계좌 번호, 각종 비번 하믄 인터넷 검색됩니다. 
- 오픈 소스의 집합소. 구글도 보고 있다.
- 오픈! 공유!

---
### 실습 하나 
- git 가입 및 계정 생성
- branch 생성  gh-pages  
- http://username**.github.io/**git_repository/file_name
- ex) http://dubu.github.io/goni/index.html
- 파일 생성 aa.txt 
- 폴더 생성 및 파일 생성
- history 확인 및 이전 상태 확인

---
### 실습 둘 
- js. jQuery. chrome 개발자도구.
- 네이버에 다음 로그를
- 뉴스 이미지 삭제
- 뉴스 제목 바꾸기, 글자 키우기 등

---
### 실습 셋 
- 내 홈피 생성. index.html
- gist  코드 블럭
- bl.ocks.org
- chrome extension 안되는데;
- bug fix , fork, pull request 요청. 

---
```
var observer = new MutationObserver(redraw);

observer.observe(document.documentElement, {childList: true, subtree: true});

redraw();

function redraw() {
  var container = document.querySelector(".repository-sidebar");
  if (!container) return;

  var parts = location.pathname.substring(1).split("/"),
      user = parts[0],
      id = parts[1],
      sha = parts[2];
  if (!user || !/^[a-z0-9][a-z0-9]*$/i.test(user)) return;
  if (!/^([0-9]+|[0-9a-f]{20})$/.test(id)) id = null;
  if (!/^[0-9a-f]{40}$/.test(sha)) sha = null;

  var anchor = container.querySelector(".bl-ocks-button"),
      href = "http://bl.ocks.org/" + user + (id ? "/" + id + (sha ? "/" + sha : "") : "");

  if (!anchor) {
    anchor = document.createElement("a");
    anchor.className = "minibutton sidebar-button bl-ocks-button";
    anchor.innerHTML = '<span class="octicon octicon-link-external"></span>bl.ocks.org';
  }

  // Disconnect to avoid observing our own mutations.
  if (anchor.href !== href || anchor.parentNode !== container) {
    observer.disconnect();
    anchor.href = href;
    container.appendChild(anchor);
    observer.observe(document.documentElement, {childList: true, subtree: true});
  }
}
```

---
### 실습 마지막
- http://datergram.github.io
- http://github.com/datergram
- git 권한추가
- 같이 만드는 스터디 홈페이지 

---
### git 으로 할 수 있는 것들
- 아이파이썬 노트북 
- 슬라이드 
- 홈페이지
- 블로그
- markdown 홈페이지
- bl.ock.org
- 등등

---
### F&A
- Q 영화 예능 동영상 깃에 올려서 공유하면 안될까요?
- A
- Q github 용량 제한 없나요?
- A
- Q 

