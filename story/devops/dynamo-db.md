## 테이블을 생성하자

**Todoli**라는 프로젝트의 백엔드는 스프링으로 구성되어있습니다. 해당 프로젝트에는 댓글을 달 수 있으며 **AWS CLI를 이용해 DynamoDB에 Comment 테이블을 생성해야합니다.**

```java
public class Comment {
    private String id; // PK, UUID
    private String name;
    private String content;
    private LocalDateTime createdAt;
}
```

## 테이블에 삽입하자

백엔드 개발자 김동학은 서버에서 데이터베이스에 저장이 제대로 되지 않는 것 같다고 문제를 제기했습니다. 의문이 생긴 당신은 다음과 같은 컬럼 데이터를 **CURL을 사용해서 삽입합니다.**

```
{
    "id": "d4101e6b-1a3b-47a9-8094-94182060f198",
    "name": "enbraining",
    "content": "I'm so hungry",
    "createAt": 알아서
}
```

