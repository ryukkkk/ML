# ML

## 머신러닝을 위한 다양한 용어와 코드집

###1. numpy Fuction
- np.argmax(...)&np.argmin(...) : np.arrage안의 최댓값&최솟값의 index 반환

```python
a = np.array([[1,2,3,4],[5,22,42,1],[11,2,1,5]])
np.argmax(a, axis =1) , np.argmin(a,axis=0)
#result -> (array([3, 2, 0]), array([0, 0, 2, 1]))
```
- np.array(a).reshape(8,) : arrat의 size가 같을때 다차원 변환
- a.dot(b) : Matrix 간 곱셈

- broadcasting : shape이 다른 배열간 연산 지원

```python
test_a = np.array([[1,2,3,],[4,5,6],[7,8,9]],float)
scalar = 3

test_a + scalar#모든 값에 scalar만큼 더해짐
```
 - 연산의 속도 : numpy>list comprehension>for문(100,000,000번의 loop가 돌 때 약 4배 이상의 성능차이가 남(Concatenate의 성능)->numpy는 python의 가장 큰 특징인 dynamic typing을 포기함)

- np.where(a>0,3,2) : a의 값중 0보다 크면 3을 삽입하고 그렇지 않으면 2를 삽입한 tuple을 return 

- test_array[test_array>3] : 조건의 True인 index의 element만 추출

# ML 용어
| Word  | Meaning|
| ------------- | ------------- |
| coefficiend of determination  | 결정계수(R^2)  |
| overfitting  | 과대적합  |
| underfitting  | 과소적합  |
| linear regression  | 선형회기  |