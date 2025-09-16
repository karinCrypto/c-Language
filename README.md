# c-Language
혼자공부하는 C언어  책



human in the roof
https://www.samsungsds.com/kr/insights/human_in_the_loop.html

int * var [5] ;
var[5] 배열  > 배열이 우선순위로 빠진다. 
int * X ;  int* X ; int *X ; int*X ; > 띄어쓰기 상관 없다.
포인터 배열

int (*var) [5] ; 괄호로 감싼 포인터가 일등이된다. 
* var 포인터 
int X [5];  > 실행되고 사라지고 남은 나머지가 있음. 숫자가 다섯개가 남아있는 배열이 위치해있음
배열 포인터

long * var ( long,long);
1) var (long,long) 함수> 먼저 실행함 
2) long * X ;
3) long 포인터를 리턴하는 함수

long (* var) ( long,long);
(* var) 포인터 
long X ( long,long); > 입력의 숫자가 두개가 들어오는 길이값을 가짐 
함수 포인터 >가짜지만 진짜처럼, 복사본이지만 원본처럼 쓸수있다. 

double ( *var(double(*)[3]) ) [3] ;
var( double(*)[3] ) 함수
double(*X)[3] 입력 타입
double (*X)[3] ; 남은 나머지 
-> 배열 포인터 리턴 타입

void (*signal(int signum,void(*handler)(int)))(int);
signal(int signum,void(*handler)(int)) => 함수
void (*X)(int); 리턴 값
void(*handler)(int);
입력 함수포인터 출력 함수포인터 인 함수


