# C++




<details>
<summary><strong>Constructor와 Destructor에 대해 설명하라.</strong></summary>
  <hr>

  **생성자**: 객체가 생성될 때 실행되는 함수, 객체의 초기화가 목적

  **소멸자**: 객체의 사용이 끝나고 메모리에 반환될때 실행되는 함수

  <hr>
</details>




<details>
<summary><strong>C++에서 Default Constructor는 무엇을 의미하는가?</strong></summary>
<hr>

   클래스에는 생성자가 반드시 있어야 한다.

   사용자가 생성자를 따로 생성하지 않으면 컴파일러가 기본 생성자를 자동으로 생성해준다.

<hr>
</details>




<details>
   <summary><strong>C++에서 <code>Virtual</code>은 왜 존재하는가?</strong></summary>
   <hr>

   오버라이딩을 기대하는 함수에 쓴다.

   virtual을 쓰면 런타임에 함수가 매핑이 되는 동적바인딩이 수행된다.

   <hr>
</details>




<details>
  <summary><code>\n</code>과 <code>endl</code>의 차이는 무엇인가?</summary>
  <hr>
      endl=버퍼를 비우는 것 (버퍼는 임시공간 stdout 버퍼를 비우면, 화면으로 그 내용이 출력된다. 이를 flush 합니다 )
      따라서 버퍼를 비우지 않는 ln이 더욱 빠릅니다.
  <hr>
</details>




<details>
   <summary><strong><code>malloc</code>과 <code>new</code>의 차이는 무엇인가?</strong></summary>
   <hr>
  1. malloc은 라이브러리 제공 함수로, stdlib.h 을 include 해주어야 사용 가능하지만, new는 기본으로 제공하는 키 워드이므로 별도의 라이브러리 추가 없이 바로 사용 가능합니다.
  
   malloc은 함수이다. 함수 내에서 메모리를 할당한다.(동적으로 메모리 할당+ 초기값 지정 x)

   new는 연산자이다. 생성자를 호출하면서 메모리를 할당한다.(할당과 동시에 초기화 가능+반드시 delete)

   <hr>
</details>




<details>
   <summary><strong>struct와 class의 차이는 무엇인가?</strong></summary>
   <hr>

   둘 다 데이터를 담는 그릇이다.

   struct : 기본 접근 제어자 public

   class : 기본 접근 제어자 private

   <hr>
</details>
