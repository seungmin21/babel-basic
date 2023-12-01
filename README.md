babel 사용한 명령어 및 순서 가이드

1. npm init -y를 사용
2. app.js 파일을 생성한 뒤 const, let 등등의 ES6 문법을 사용
3. 처음 설정 실행 파일을 만들때는 .babelrc 파일을 만들어서 사용
  그러나 babel.config.json 파일을 만들어서 preset을 사용
4. package.json 파일에 script 명령어에 build:babel 명령어를 추가
  4-1 "build:babel" : "babel app.js --out-dir dist 입력
    -> build:babel(run 키워드 이후 입력될 명령어) babel 변환할 디렉토리 --out-dir(전체 내보내기) 내보내는 곳 위치 지정
5. 실행 명령어 npm run build:babel
              npx babel app.js --out-dir dist
