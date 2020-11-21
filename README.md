# json-server

## 아래 절차를 진행하면 node_modules폴더와 의존성을 위한 package.json 파일이 생성됨  

```
mkdir json-server-exam && cd json-server-exam
npm init -y
npm install -g json-server --save-dev
```

## json-server를 실행함  
```
## 기본포트 사용, watch 옵션(db.json 파일의 변경을 감지하는 기능) 적용
json-server --watch db.json

## 포트 변경 / watch 옵션 적용
json-server --watch db.json --port 5000
```

## package.json 파일의 script를 변경하여 바로 실행하는 명령어 지정 가능  
```
"scripts": {
  "start": "json-server --watch db.json
};
```
```
npm start
```

## 업로드 되어 있는 파일을 참고하여 아래 명령을 실행할 수 있음  
- GET
- POST
- PUT
- PATCH
- DELETE

## 브라우저를 열고 아래 주소로 접속  
``` 
## 메인 페이지
localhost:3000

## json 파일 접속json 최상위 분류가 todos 인 경우)
localhost:3000/todos

## json 파일의 todos에서 id를 사용하여 특정 todo를 취득  
localhost:3000/todos/1

