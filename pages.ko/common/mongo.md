# mongo

> 레거시 MongoDB 셸. 새로운 셸에 대해서는 `mongosh`를 참조.
> 참고: 모든 연결 옵션은 하나의 문자열로 대체할 수 있습니다: `mongodb://user@host:port/db_name?authSource=authdb_name`.
> 더 많은 정보: <https://docs.mongodb.com/manual/reference/program/mongo>.

- 기본 포트(`mongodb://localhost:27017`)에서 로컬 데이터베이스에 연결:

`mongo`

- 데이터베이스에 연결:

`mongo --host {{호스트}} --port {{포트}} {{데이터베이스_이름}}`

- 지정된 데이터베이스에서 지정된 사용자 명으로 인증(비밀번호 입력이 필요합니다):

`mongo --host {{호스트}} --port {{포트}} --username {{사용자_명}} --authenticationDatabase {{인증_데이터베이스_이름}} {{데이터베이스_이름}}`

- 데이터베이스에서 JavaScript 표현식을 평가:

`mongo --eval '{{JSON.stringify(db.foo.findOne())}}' {{데이터베이스_이름}}`
