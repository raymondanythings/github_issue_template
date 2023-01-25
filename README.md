[Airbnb 코드스타일 가이드 바로가기](https://github.com/tipjs/javascript-style-guide#28.2 "Airbnb 코드스타일 가이드")


## 레포지토리 초기 세팅
1. 라벨 설정하기
   - YOUR_GH_TOKEN : 깃허브 Personal access token [깃허브 토큰발급 바로가기](https://github.com/settings/apps)
   - YOUR_REPOSITORY : 해당하는 레포지토리 경로 ex) myname/myProject
    ```bash
    npx github-label-sync --access-token <<YOUR_GH_TOKEN>> --labels ./labels.json <<YOUR_REPOSITORY>>
    ```


## 커밋 컨벤션
 - regex
   - ^(🎨|🐛|💄|♻️|🗑️|🚧|🧪)(feat|fix|style|refactor|cleanup|chore|test)\s:\s.+
 - 유다시티 커밋컨벤션
      ```HTML
      <type>(<scope>): <subject> - Subject line
      <BLANK LINE>               - 줄 바꿈으로 구분한다
      <body>                     - Message body
      <BLANK LINE>               
      <footer>                   - Message footer

      1. **Subject line**
         1. 변경 사항에 대한 간단한 설명.
      2. **Message body**
         1. 수정 이유와 전후 비교 설명.  
         2. 명령형 현재 시제로 작성한다. (changed X, change O)
      3. **Message footer**
         1. 주요 변경사항은 푸터에 변화에 대한 상세설명, 정의, 이전 노트와 함께 명시되어야 한다.
         2. 전후를 Before : scope: { ~~ } After : scope: { ~~~ } 와 같이 상세하게 명시한다.
         3. 처리 완료된, 즉 close 된 이슈에 대해서는 `Closes #123, #124` 로 표기한다.
      ```
  .