# Javascript

-var는 참조변수 값을 할당할때 자동으로 스스로 공간을 갖는다 (오토박싱)  
-모든변수는 참조변수, 기본형식이라는것이 없다

## Wrapper클래스

-boolena
-Number(정수)  
-Number(실수)  
-String(문자)  
-String(문자열)

    var x=3;
    var x=new Number(3);//동일한 방법

-undefined:객체는 있으나 아직 값을 할당하지 않는 상태  
-어떤 메소드를 사용할 수 있는지는 할당되는 객체에 따라서 달라진다.

    num=3.4 =>new Number(3.4);
    num=3=>new Number(3);
    num= "3"=>new String("3");

## 배열객체

### push/pop메소드를 이용한 데이터 관리Stack

---

-var nums=new Array();

    nums.push(5);
    alert(nums)
    nums.push(10);
    alert(nums)
    nums.push(21);
    alert(nums)

    var n1=nums.pop();//21
    var n2=nums.pop();//10
    var n3=nums.pop();//5

### 인덱스를 이용한 데이터 관리:list

---

    var nums=new Array();
    nums[0]=5;
    nums[1]=10;
    nums[2]=21; //[5,10,21]
    ---
    var nums=new Array();
    nums[3]=5;//[undefind,undefined,undefined,5]

---

splice():은 삭제도 가능 추가도 가능하다
splice(i):i번째부터 끝까지 삭제
splice(i,v):i번째부터 v번까지 삭제
splice(i,j,v):i번부터j번까지 삭제하고 그 자리에 v값을 넣어라

# Object

---

var exam=new Object();
exam.kor=30;
exam.eng=70;
exam.math=80;
자바스크립트는 맨땅에 객체도 생성이 가능하다

\*키를 이용한 데이터 관리:Map
exam["kor"]=30;
exam["eng"]=70;
exam["math"]=80;

간단한 표기법
var exam={"kor":30,"eng":50}

eval()

# AJAX

AJAX:비동기통신
Asynchronous Javascript And XML(비동기식 자바 스크립트와 XML)
브라우저->XMLHttpRequest:내가 원하는 데이터만 로딩하는것

# JSON

JSON:JavaScript Object Notaion
