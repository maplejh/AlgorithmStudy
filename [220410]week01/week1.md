### 1. 알고리즘 정리

- 알고리즘 정의  

  문제를 해결하기 위한 단계적인 절차를 의미한다. 주어진 문제에 대해 여러 종류의 알고리즘 중에서 효율적인 알고리즘을 고안하는 것이 매우 중요하다.   

  - 컴퓨터에 의해 특정한 일을 수행할 수 있는 명령어 집합으로 다음의 조건을 만족해야한다.  
    1. **입력(input)**: 입력은 없거나 하나 이상 존재할 수 있다.  
    2. **출력(output)**: 출력은 반드시 하나 이상 존재해야한다.  
    3. **명확성(unambiguity)**: 각 명령어의 의미는 모호하지 않고 명확해야 한다.  
    4. **유한성(finiteness)**: 반드시 유한 시간 이내에 종료되어야한다.  
    5. **효과성(effectiveness)**: 각 명령어는 기본적이면서 단순해야 하고 컴퓨터에 의해 실행 가능해야 한다.  

cf) 자주나오는 알고리즘들(추가예정)  

----

### 2. 알고리즘 분석

- 시간복잡도  

  **입력크기**에 따라서 **기본연산**이 몇 번 수행되는지 결정하는 절차 -> 실제와는 독립적인 측정법 // 기본연산이 수행되는 횟수를 입력의 크기에 대한 함수로 구함  

- 공간복잡도  

  알고리즘이 수행되면서 필요한 기억 용량의 크기  

- 분석방법  

  - **Every-case time complexity: T(n)**  
    depending on: input size  
  - Worst-case time complexity: W(n)  
    depending on: input size, input values  
  - Average-case time complexity: A(n)  
    depending on: input size, input values  
  - Best-case time complexity: B(n)  
    depending on: input size, input values  

----

### 3. 차수표기법  

- 복잡도 부류    

  일반적으로 n이 매우 커진다고 가정하고 비교  

  http://www.ktword.co.kr/test/view/view.php?m_temp1=6146&id=1420    

  - 상수시간  
  - 로그 시간  
  - 선형시간  
  - 로그선형시간  
  - 제곱시간  
  - 세제곱시간  
  - 지수 시간  

  시간복잡도 연산 크기 순서: 상수시간< 로그시간< 선형시간< 제곱시간< 세제곱시간< 지수시간  

- Big-Oh  

  O(f(n)): 최고차항의 차수가 f(n)과 일치하거나 더 작은 함수들의 집합(최악의 경우) -> 가장 많이 쓰인다고 함  

- Big-Omega  

  Ω(f(n)): 최고차항의 차수가 f(n)과 일치하거나 더 큰 함수들의 집합(최선의 경우)  

- Theta  

  Θ(f(n)): 최고차항의 차수가 f(n)과 일치하는 함수들의 집합(최선과 최악의 중간)  

---

cf)  

파이썬 1초 연산 횟수 2천만(20,000,000)~1억(1000,000,000)정도 (N의 범위에 따라 알고리즘 선택)  
int의 경우에는 리스트 길이가 100만(1,000,000)개일때 4mb정도 (데이터개수가 천만(10,000,000)이상이 넘어가지 않도록)  

파이썬 자료형 및 연산자의 시간복잡도는 https://www.ics.uci.edu/~pattis/ICS-33/lectures/complexitypython.txt 참고해보기  

```python
# https://github.com/ndb796/python-for-coding-test/blob/master/1/1.py
import time
start_time = time.time() # 측정 시작

# 프로그램 소스코드
end_time = time.time() # 측정 종료
print("time:", end_time - start_time) # 수행 시간 출력
```
