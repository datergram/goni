# goni
깃허브 실습용

데이터 그램 발표용. 
태풍 고니가 올라오는 저녁에..
git  설명

### git
 vcs version control system. 
 종류 cvs. svn. git
 git? github?
 버젼관리란 동일 파일은 하나만 유지하자. 
 공짜. 무재한
 그대신 전부 오픈. 전화 번호, 계좌 번호, 각종 비번 하믄 인터넷 검색됩니다. 
 오픈 소스의 집합소. 구글도 보고 있다.
 오픈! 공유!
 
### 실습 하나
 git 가입 및 계정 생성
 branch 생성  gh-pages  
 
 http://username**.github.io/**git_repository/file_name
 ex) http://dubu.github.io/goni/index.html
 
### git 으로 할 수 있것들
 슬라이드 
 홈페이지
 블로그
 markdown 홈페이지
 bl.ock.io
등
 

내꺼 만들기
같이 쓰는거 만들기. 출석부? // 소감문. 

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

재미있는거 
실습위주로
불을 지피다~

왜 하는가?
비슷한애들 
구글드라이브 , 클라우드, 블로그?
뭐가 다른가 파일 단위 같이 협업?

문서중복. 웹으로 한 페이지 만들어 보자 

실습 웹에서  한 페이지 글 쓰고 삭제 하기 

쓰는 방법은 과감하게 삭제
필요하면 다 쓴다. 

불을 지피자 

이제부터 산으로~

아이 파이썬 노트북 
ppt 뭐가 좋을까 
블로그로 쓰기도 하고 
홈페이지? 깃헙페이지~
내 홈페이지 빠르게 만들어 보자~

앞으로 이런거를 할꺼 같은데. 
네이버를 글어다가 ~ 이미지 바꿔치기 
조그만 더하면 피씽 사이트 


같이 공유의 장점
깃 사용법. 코드 검색. 비슷한 코드의 검색. 
같은 파일은 하나만 존재하게 한다. 중복의 삭제
