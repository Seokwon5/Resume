# Resume


안녕하세요 🙇🏻 

백엔드 개발자 이석원 입니다.

__프로그래밍 언어 Java 와 swift에 관심이 많고 꾸준히 공부하고 있습니다.

* Email : tjrdnjs5@gmail.com
* Notion : https://www.notion.so/0e13608d975f49409fac39e306355e42?pvs=4

## Education

* 동국대학교 wise캠퍼스 컴퓨터공학과 4학년 졸업 
  * 2016.03 ~ 2022.02

* 서울경신고등학교 졸업
  * 2011.03 ~ 2014.02
  
## Skills

* Programming Language
  - Java
  - Swift
 
* Programming Tool
  - Intellij
  - Eclipse
  - Xcode
 
* Programming Skills

  - Spring boot
  - MySql
  - Lombok, Thymeleaf
  - UIKit, SwiftUI
  - Snapkit, Alamofire
  - RestAPI
  - UserDefaults, Coredata, Firebase, Database

## Projects

### [게시판 서비스]

* __가장 기본적이고 보편적인 게시판 기능입니다. 2024년 1월 기준 가장 최신의 스프링 부트와 관련 기술들, 자바 17 기능들, 개발 도구들을 경험하고 개발하였습니다.__
  
* Detail: https://github.com/Seokwon5/fastcampus-project-board

* 기간

    * 2023.12 ~ ing (리팩토링하며 계속 서비스 중)
    
* 내용

    * __ 기능 구현__
        
        - Spring Boot와 JPA를 활용하여 게시글과 댓글 간 일대다 관계, Auditing기능을 구현하고 Lombok을 활용하여 간결한 코드로 작성
          
        - Java를 활용하여 컨트롤러를 통해 생성자 주입 및 게시글 관련 글과 댓글을 작성, 수정, 삭제 기능을 구현.
          
        - Spring Security를 설정하여 URL 접근 권한 및 로그인, 로그아웃 기능을 정의하고 구현
          
        - Java와 Record를 사용하여 HTTP 요청을 통해 받은 데이터를 담는 과정과, 게시글 조회 등의 응답 데이터를 담는 과정을 구현.
          
        - 데이터 전송 객체인 DTO를 구현하여 서비스 계층과 컨트롤러 간의 데이터 교환을 구현.


### [포켓북]

* __사용자가 가진 책들을 저장하고 분류하는 서재 관리 어플리케이션__

* RestAPI를 공부하면서 진행한 개인 프로젝트
  
* Detail: https://github.com/Seokwon5/PocketBook#readme

* 기간

    * 2023.08 ~ ing (리팩토링하며 계속 서비스 중)
    
* 내용

    * __ 기능 구현__
        
        - Alamofire를 이용하여 네이버 OpenAPI를 요청하고 받아 사용자가 가진 책을 업로드
          
        - UserDefaults를 활용해 책 데이터 저장
          
        - 모든 책 정보를 TableView에 저장하고 filter 메소드로 분류
          
        - 현재 읽고 있는 책과 다 읽은 책을 CollectionView, TableView를 활용하여 홈 화면에 등록
          
        - SnapKit을 활용하여 UI 구현

    * __ 오류 해결 __
 
       -  상태 변경 후, 제대로 변경되었는지 확인하기 위해 ListViewController에서 didUpdateReview 프로토콜을 받고 해당 배열을 찾아 배경색을 변경해주도록 설정하였습니다.
  
          그러나 색은 변하지 않았고 디버깅 메세지를 걸어 어느부분에서 호출되지 않는지 찾아본 결과
          해당 배열의 인덱스를 찾기 전 새로운 데이터 정보를 업데이트해주는 코드를 먼저 삽입하지 않은 이유로 인해 발생하였고 해결할 수 있었습니다.

          이처럼 코드 순서를 실수하지 않도록 꾸준히 디버깅 메세지를 걸어 확인하는 습관을 길러야겠다는 생각을 하였습니다.

 

### [렘비]

* __친구들의 MBTI를 저장해두고 관리하는 어플리케이션__

* [AppStore 다운로드] https://apps.apple.com/us/app/%EB%A0%98%EB%B9%84/id6446311376?platform=iphone

* SwiftUI를 공부하면서 진행한 개인 프로젝트

* Detail: https://github.com/Seokwon5/Rembi/blob/main/README.md

* 기간

    * 2023.01 ~ ing (리팩토링하며 계속 서비스 중)
    
* 내용
  
   * __ 기능 구현 __
      
     CoreData
       - Coredata를 적용하여 데이터의 CRUD(생성, 읽기, 업데이트,삭제) 작업을 구현하였습니다.
       - ObservableObject 프로토콜을 채택하여 SwiftUI에서 저장된 데이터를 관찰할 수 있도록 구현하였습니다.

     ListView
       - @FetchRequest 프로퍼티 래퍼를 사용하여 모델의 객체들을 가져왔습니다.
       - FetchedResults 타입을 통해 CoreData의 fetchRequest의 결과를 구현하였습니다.

     Picker
       - picker를 이용하여 데이터를 저장하기 위해 상태변수와 바인딩하였습니다.

     NSSortDescriptor
       - Picker를 이용하여 정렬 기준을 선택하도록 NSSortDescriptor메소드를 이용하여 구현하였습니다.

     NSPredicate
       - 같은 mbti를 가진 객체들을 필터링 하여 볼 수 있도록 FetchRequest의 NSPredicate 메소드를 이용하여 가져오는 데이터의 기준을 설정하였습니다.


      * __ 오류 해결 __
 
        - MBTI를 저장한 뒤, 같은 성격을 가진 사람들을 모아보는 기능을 만들어 이용자들이 성격별로 지인들을 한눈에 볼 수 있도록 모든 MBTI 성격모델을 만들고 CoreData안의 mbti객체와
          같은 성격일 경우에만 뿌려주는 FetchResult 데이터 구조를 만들던 중,
          predicate에 조건문을 달았을 경우 MBTI모델을 읽기 전 FetchRequest가 먼저 실행 되는 오류를
          해결하기 위해 데이터의 흐름을 다시 파악하고 init 메소드를 따로 설정하는 방법으로 먼저 predicate 조건을 읽고 그 뒤에 fetchRequest가 실행되도록 하였습니다.

   
<br></br>

