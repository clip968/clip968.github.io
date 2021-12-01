# 유레카 프로젝트를 해오며...

## 1. Github 홈페이지 생성

  1. clip968.github.io repo 생성
  2. D:\git\clip968.github.io로 클론
  3. index.html 수정
  4. git push로 수정된 사항 반영

## 2. Jekyll 설치
  - 참고한 페이지: <https://ogaeng.com/jekyll-blog-install/>
  1. Ruby 먼저 설치
  2. Ruby Prompt로 Jekyll 설치
  ```ruby
  gem install jekyll bundler
  ```
  3. Jekyll 버전 확인
  ```ruby
  jekyll -v
  ```
  4. Jekyll Setup
  ```ruby
  jekyll new . --force
  ```
  5. Jekyll 실행하기
  ```ruby
  bundle exec jekyll serve
  ```
  ### Jekyll Webrick Error
  - 참고한 페이지: <https://junho85.pe.kr/1850>
  > 'require': cannot load such file -- webrick (LoadError)
  - 해결하는 법:
  ```ruby
  bundle add webrick
  ```
  ### Another Jekyll Error
  - 참고한 페이지: <https://velog.io/@minji-o-j/jekyll-오류-해결>
  > Jekyll 4.2.0 Please append --trace to the serve command 
  > for any additional information or backtrace
  - 해결하는 법:
  ```ruby
  bundle exec jekyll serve --trace
  ```
   6. 적용 사항 Commit 작성 후 Push
   7. 예시 파일인 MongoDB 따라서 작성해보기
## 3. 테마 적용
  - 테마 페이지 1: <http://jekyllthemes.org>
  - 테마 페이지 2: <https://jekyllthemes.io/free>

  1. 처음 적용 했던 테마:

        Hydejack : http://jekyllthemes.org/themes/hydejack/

    그러나 문제는 초보자였던 나에게 너무 어려웠던 템플릿
    따라서 더 쉬운 템플릿으로 갈아타기로 결정
  2. 테마 최종 결정:
        
        Pixyll : https://jekyllthemes.io/theme/pixyll

  3. Zip 파일로 받아 압축해제
  4. Post 제외 모든 파일을 붙여 넣기
  5. Git Push로 해당 사항 적용

 ## 4. 댓글 기능 추가
  - Disqus 사이트 주소 : <https://disqus.com>
 1. Disqus 사이트 회원가입
 2. Disqus 세팅
 ### Pixyll 테마 사용시 주의할 사항
  - Pixyll 테마 사용시 ppt에 나온 key-value를 쓰지 않는다.
  - 또한 disqus 홈페이지에서 universal code도 쓰지 않는다.
  - 적용 방법: 

      disqus_shortname: clip968-github-io

    _config.yml안에 disqus_shortname 칸이 존재하는데 이곳에 자신의 disqus 계정 shortname을 적으면 된다.
  - 보는 법:
      
      우측 상단 프로필 클릭 > Settings
    
  

    

