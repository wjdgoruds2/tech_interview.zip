# JAVA




<details>
   <summary><strong>Java의 Collection에 대해서 설명해 주세요.</strong></summary>
<hr>
   <p>여러 데이터를 담을 수 있는 자료구조</p>
   <p>collection인터페이스는 list+set+queue크게 3가지로 분리할 수 있습니다.Map같은 경우에도 인터페이스의 상속을 받고 있지는 않지만 collection으로 분류됩니다.
   </p>
   <p>set은 순서를 유지하지 않는 데이터의 집합으로 중복을 허용하지 않습니다.(Hashset,Treeset)</p>
   <p>List는 순서가 있는 데이터 집합으로 데이터의 중복을 허용합니다.(Linkedlist,Vecor,Arraylist)</p>
   <p>queue는 list와 유사합니다.(Linkedlist,Priorityqueue)</p>
   <p>Map은 key,value의 쌍으로 이루어진 데이터 집합으로 순서는 유지되지 않으며 키의 중복은 허용되지 않으나 value의 중복을 허용됩니다.(Hashtable,Hashmap,Treemap)</p>
<hr>
</details>




<details>
   <summary><strong>Wrapper Class란 무엇인가요?</strong></summary>
<hr>
   <p>java에는 primitive type과 reference type이 있습니다. </p>
   <p>기본 타입의 데이터를 객체로 표현해야하는 경우가 있습니다.따라서 기본 자료타입을 객체로 다루기 위해서 사용하는 클래스들을 래퍼 클래스라고 합니다.</p>
   <p>primitive type의 경우 NULL 값을 담지 못하고, 제네릭 프로그래밍에 쓰지 못한다는 특징이 있는데, 이러한 경우와 같이 데이터를 객체로 표현해야 할 때 쓰이는 것이 Wrapper입니다.</p>
<hr>
</details>




<details>
   <summary><strong>직렬화(Serialization)과 역직렬화(Deserialization)에 대해서 설명해 주세요.</strong></summary>
<hr>
   <p><strong>직렬화 </strong>: 데이터를 연속적인 데이터로 변형하는 것으로 객체를 통째로 파일로 저장하거나 전송하고 싶을때 주고 사용합니다.</p>
   <p><strong>역직렬화 </strong>: 직렬화된 데이터를 변환하여 다시 객체의 형태로 표현하는 것으로 저장된 파일을 읽거나 전송된 스트림 데이터를 읽어 원래 객체의 형태로 복원합니다.</p>
<hr>
</details>




<details>
   <summary><strong>Java Generic에 대해서 설명해 주세요.</strong></summary>
<hr>

제네릭이란 어떤 객체의 타입인지에 관계없이 프로그래밍하는 것을 말합니다. 객체를 초기화할때 타입을 지정해주기 때문에 타입캐스팅이 필요없고 컴파일 타임에 타입체크를 해주기때문에 디버깅이 쉽다는 장점이 있습니다.

**제네릭**

- 다양한 타입의 객체를 사용하는 메소드나 클래스에서 객체를 초기화할 때 타입을 지정해주는 기법

**장점**

- 코드 간결
- 컴파일 타임에 오류 체크
- 타입 캐스팅할 필요 없음
- 재사용성 증가


<details>
  <summary><strong><em>제네릭을 사용하지 않을 경우</em></strong></summary>
  <p><strong>EX)</strong> 만약 제네릭을 사용하지 않고 <code>Object</code> 클래스를 상속받는 경우 매번 타입캐스팅을 해주어야함.
     만약 타입캐스팅이 잘못되면 런타임시 <code>ClassCastException</code> 오류 발생함
  </p>
</details>


<hr>
</details>




<details>
   <summary><strong>equals와 ==의 차이는 무엇인가요?</strong></summary>
<hr>

기본적인 동작은 똑같은데 , equals는 override할수 있기때문에 사용자가 원하는 논리적인 통일성을 비교할 수 있다.

`==`

- 참조 비교 : 두 객체가 같은 메모리 공간을 가리키는 지 확인(참조(주소)값을 비교하는 연산자)

`equals()`

- 내용 비교 : 두 객체의 값 확인

<hr>
</details>




<details>
   <summary><strong>hashCode란 무엇인가요?</strong></summary>
<hr>
   <p>두 객체가 동일한 객체인지 비교 가능</p>
   <p>heap 에 저장된 객체의 메모리 주소 반환</p>
<hr>
</details>




<details>
   <summary><strong>문자열을 리터럴(string = "abcd")로 할당하는 것과 객체(string = new String("abcd"))로 할당하는 방식의 차이가 무엇인가요?</strong></summary>
<hr>
   <p>리터럴 : string constant pool에 생성</p>
   <p>new : heap에 생성</p>
   <p>== 연산도 다름</p>
<hr>
</details>




<details>
   <summary><strong>익명함수란?</strong></summary>
<hr>
   <p>리터럴 방식으로 만들어진 이름없는 함수</p>
   <p>재사용을 안하기때문에 이름없이 만든다.</p>
   <pre><code>//리터럴 방식
var a = 10;
var name = superman;

//익명함수
var funcA = function(name){
alert(name + &quot;님 환영합니다&quot;);
}</code></pre>
<hr>
</details>




<details>
   <summary><strong>Lambda란?</strong></summary>
<hr>
   <p>람다란 함수형 프로그래밍을 지원하기 위해 자바8부터 나온 표현식으로, 함수형 인터페이스를 이용하는 방식입니다. 익명함수의 한 형태입니다.</p>
   <p>코드가 간결해지고 가독성이 높아진다는 장점이 있는 반면에, 남용시 디버깅이 어려워질 수 있다는 단점이 존재합니다.</p>
<hr>
</details>




<details>
   <summary><strong>정적 바인딩 vs 동적 바인딩</strong></summary>
<hr>
   <p><strong>바인딩</strong> : 함수를 호출할 때 함수가 위치한 메모리로 연결시켜주는 것</p>
   <p><strong>정적 바인딩</strong> : 컴파일 타임에 결정, 컴파일 시간에 정보가 결정되므로 효율 좋음</p>
   <p><strong>동적 바인딩</strong> : 런타임에 결정, 런타임에 자유롭게 바뀌므로 적응성 좋음, 타입 체크로 인한 수행 속도 저하</p>
<hr>
</details>




<details>
   <summary><strong>Callable과 Runnable의 차이는?</strong></summary>
<hr>

둘다 스레드를 구현하기 위한 인터페이스임

**Callable**

- 리턴 타입 존재
- Exception 발생

**Runnable**

- 리턴 타입 없음
- Exception 없음

<hr>
</details>




<details>
   <summary><strong>Thread-safe하게 프로그래밍 하려면?</strong></summary>
<hr>

- `volatile` : 캐시에 저장하지 않고 메모리에서 접근하겠다 (ex. 하나의 스레드만 RW하고 나머지는 R하는 경우)
- `synchronized` 키워드 : Lock기법
- `Atomic` 클래스 : CAS(Compare And Swap)기반, 특정 메모리 위치 값과 주어진 값을 비교해 같으면 새로운 값으로 변경


<hr>
</details>




<details>
   <summary><code>HashSet </code>vs <code>TreeSet</code></summary>
<hr>

**HashSet**

- 해싱으로 구현
- TreeSet보다 빠름
- 정렬 불가

**TreeSet**

- 이진탐색트리 형태로 데이터 저장
- 레드-블랙 트리로 구현됨
- 추가/삭제에는 시간 걸리지만 검색과 정렬 뛰어남
- 저장순서 유지X

<hr>
</details>




<details>
   <summary><code>HashMap</code> vs <code>HashTable</code></summary>
<hr>

**HashMap**

- 비동기
- 보조해시 사용

**HashTable**

- 동기, thread-safe
- 멀티스레드가 아니라면 HashMap보다는 성능이 떨어짐
- Null 허용하지 않음


<hr>
</details>




<details>
   <summary><code>HashSet</code> vs <code>HashMap</code></summary>
<hr>

**HashSet**

- 중복된 객체 비허용
- 객체 저장
- equals() hashCode() 메소드로 중복 여부 체크
- HashMap에 비해 느림

**HashMap**

- Map 인터페이스 구현
- key-value 형식 데이터 저장
- HashSet에 비해 빠름



<hr>
</details>
