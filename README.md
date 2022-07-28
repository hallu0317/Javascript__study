# JS_study

### JS에서 자료형 선언 3가지 방법

자바스크립트에는 int, double, string과 같은 변수형이 존재하지 않으며 가변형 변수만 존재한다.   

- var : 변수를 선언 + 동시에 값을 초기화   
- let : 블록 스코프 지역 변수를 선언. + 동시에 값을 초기화 (가변형 블럭 지역변수)   
- const : 블록 스코프 읽기 전용 상수를 선언 (불변형 블럭 지역  변수)   
초기화 없이 선언된 변수는 undefined 값을 가지며 접근을 시도하는 경우 ReferenceError 예외가 발생함.

---
### 템플릿 리터럴
- var a= 20, b=5, c= "자바스크립트"
- ES6 이전 : var str = "나는 " + (a+b) + "살이고 " + c + "를 좋아한다.";
- ES6 이후 : let str = `나는 ${a+b}살이고 ${c}를 좋아한다.`;
---
### 함수
- charAt(n) : n번째 문자를 출력
- indexOf("?") : ?라는 글자가 있다면 글자의 인덱스를 출력, 없다면 -1
- includes("?") : ?라는 글자가 있다면 true, 없다면 false 출력
- slice(n,m) : n ~ m-1 까지의 문자를 출력 (음수 사용가능)
- split("?") : ? 라는 문자를 기준으로 문자열을 분리함.
- trim() : 앞, 뒤 공백을 제거함.
- map() : 배열 내의 모든 요소 각각에 대하여 주어진 함수를 호출한 결과를 모아 새로운 배열을 반환   
  ex) const array = [1, 4, 9, 16]   
      const map1 = array.map(x => x * 2);  => [2, 8, 18, 32]   
      var roots = array.map(Math.sqrt) => [1, 2, 3, 4]   
      
- filter() : 주어진 함수의 조건을 만족하는 모든 요소를 모아 새로운 배열로 반환   
  ex) const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present']   
      const result = words.filter(word => word.length > 6);    
      => ["exuberant", "destruction", "present"]   

- reduce() : 누산기(acc), 현재값(cur), 현재 인덱스(idx), 원본 배열(src) 네 개의 인자를 가진다.   
  ex) [0,1,2,3,4].reduce( (prev, curr) => prev + curr);    
  ex) var sum = [0, 1, 2, 3].reduce((acc,cur) => acc+cur,0);   
---
### 형변환
- 정수 => 문자열 : String(num); , num.toString();
- 문자열 => 정수 : Number(str); , parseInt(str);
---
### ... 전개구문
- let arr = [1,2,3] , let arr2 = [...arr]
- console.log(arr2) = [1,2,3]
---


