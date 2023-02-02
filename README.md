# REST-API
REST-API 활용 실습 REPO

## REST API
REST는 HTTP를 기반으로 클라이언트가 서버의 리소스에 접근하는 방식을 규정한 아키텍쳐이고 REST API는 REST를 기반으로 서비스 API를 구현한 것을 의미한다.

<br/>

1. JSON 서버 설치하기
```console
npm i json-server --save-dev
```

2. 프로젝트 루트 폴더에 리소스를 제공하는 데이터베이스 역할을 하는 db.json 파일을 생성한다.


3. db.json 파일의 변경을 감지하려면 watch 옵션을 추가하고 기본 포트는 3000이며 이를 변경하려면 port 옵션을 추가한다.
```console
json-server --watch db.json --port 5000
```

4. package.json에서 scripts를 다음과 같이 추가한후 `npm start`명령어로 JSON 서버를 실행한다.
```json
{
  "name": "json-server-exam",
  "version": "1.0.0",
  "scripts": {
    "start": "json-server --watch db.json"
  },
  "devDependencies": {
    "json-server": "^0.16.1"
  }
}
```

```console
npm start
```

4. public 폴더 생성 후 서버를 중단/재실행 한다. public 폴더의 각각의 html 파일을 추가한다.
