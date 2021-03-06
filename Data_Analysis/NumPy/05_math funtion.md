### sum( )
- 배열 전체 혹은 특정 축의 모든 원소의 합을 계산한다
```py
arr = np.arange(9).reshape(3, 3)
print(np.sum(arr))
=> 36
```
- `np.sum(arr[0])`과 같은 방법으로 열을 지정할 수 있다
- `np.sum(arr.T[0])`같은 방법으로 행도 지정할 수 있긴 하다. 맞는 방법이긴 한가

### mean( )
- 산술평균을 구하는 함수다.
- 위랑 같은 방법으로 사용한다
- 쟤도 `.T`써서 행도 지정할 수 있긴 하다

### std( ), var( )
- 각각 표준편차, 분산을 구한다.
- 책에 분모의 기본값은 n이라고 적혀있다
- 선택적으로 자유도를 줄 수 있다고 한다

### min( ), max( )
- 최소 값, 최대 값을 구해준다

### argmin( ), argmax( )
- 최소, 최대 원소의 색인값을 반환한다

### cumsum( ), cumprod( )
- 각각 원소의 누적 합, 곱을 배열로 반환한다
```
arr = np.arange(9).reshape(3, 3)
print(np.cumsum(arr))
-> [ 0, 1, 3, 6, 10, 15, 21, 28, 36]
```

---
### axis=
- `axis=`에 정수 인자를 넣어 n차원 배열끼리 연산할지 지정할 수 있다
  - 지정을 안하면 배열을 `flatten`으로 바꿔서 명령을 수행한다

### dtype=
- `dtype=`를 이용해 데이터 타입을 따로 지정해 줄 수 있다
- datatype.md 를 참고하자