# big-O

[Big O notation](https://www.youtube.com/watch?v=Chcl71vEkRg)  
[Big Ω notation/ Big θ notation](https://www.youtube.com/watch?v=cNrsDdxdsfw)  
[Big O notation](https://www.youtube.com/watch?v=Chcl71vEkRg)

# 시간 복잡도(점근적 실행 시간, asymptotic runtime)

- O(big-O): 시간의 상한  
  배열의 모든 값을 출력하는 알고리즘은 O(N)으로 표현할 수 있지만
  O(N^3),O(N^2),O(2^N)도 옳은 표현이다.
  다시 말하자면 알고리즘의 수행 시간은 적어도 이들 중 하나보다 빠르기만 하면 된다.

- Ω (big-Omega): 시간의 하한  
  배열의 모든 값을 출력하는 알고리즘은 Ω(N) 뿐만 아니라 Ω(logN) 혹은 Ω(1)로도 표현할 수 있다.결국, 해당 알고리즘은 Ω 수행 시간보다 빠를 수 없게 된다.

- θ (big-theta): 딱 맞는 수행 시간  
  θ는 O와 Ω 둘 다 의미한다. 즉, 어떤 알고리즘의 수행시간이 O(N)이면서 Ω(N)이라면, 이 알고리즘의 수행 시간을 θ(N)로 표현할 수 있다.

# 공간 복잡도

- 사용하는 스택 공간 또는 공간 복잡도 계산에 포함된다.
- 함수들이 호출 스택에 동시에 존재하지 않으면 계산에 포함되지 않는다.

#

> 1.  상수항은 무시하라  
>     O(N) = O(2N)
> 2.  지배적이지 않은 항은 무시하라  
>     O(N^2) = O(N^2 + N)
> 3.  여러 부분으로 이루어진 알고리즘: 덧셈 vs 곱셈
>
> - O(A+B)  
>   만약 알고리즘이 "A 일을 모두 끝마친 후에 B일을 수행하라"의 형태라면 A와 B의 수행 시간을 더해야 한다.
> - O(A\*B)  
>   만약 알고리즘이 "A 일을 할 떄마다 B 일을 수행하라"의 형태라면 A와 B의 수행시간을 곱해야 한다.
