문제 : <mark>**몫 구하기</mark>**

###### 문제 설명

정수 `num1`, `num2`가 매개변수로 주어질 때, `num1`을 `num2`로 나눈 몫을 return 하도록 solution 함수를 완성해주세요.

##### 제한사항

- 0 < `num1` ≤ 100
- 0 < `num2` ≤ 100

![](file://C:\Users\LIM\AppData\Roaming\marktext\images\2022-12-28-01-28-54-image.png?msec=1672158534789)

##### 입출력 예 설명

입출력 예 #1

- `num1`이 10, `num2`가 5이므로 10을 5로 나눈 몫 2를 return 합니다.

입출력 예 #2

- `num1`이 7, `num2`가 2이므로 7을 2로 나눈 몫 3을 return 합니다.

def solution(num1, num2):
 return num1 // num2

// : 몫

문제 : <mark>**나머지 구하기</mark>**

###### 문제 설명

정수 `num1`, `num2`가 매개변수로 주어질 때, `num1`를 `num2`로 나눈 나머지를 return 하도록 solution 함수를 완성해주세요.

---

#### 제한사항

- 0 < `num1` ≤ 100
- 0 < `num2` ≤ 100

![](file://C:\Users\LIM\AppData\Roaming\marktext\images\2022-12-28-01-31-34-image.png?msec=1672158694404)

#### 입출력 예 설명

입출력 예 #1

- `num1`이 3, `num2`가 2이므로 3을 2로 나눈 나머지 1을 return 합니다.

입출력 예 #2

- `num1`이 10, `num2`가 5이므로 10을 5로 나눈 나머지 0을 return 합니다.

def solution(num1, num2):
 return num1 % num2

문제 : **<mark>짝수의 합</mark>**



###### 문제 설명

정수 `n`이 주어질 때, `n`이하의 짝수를 모두 더한 값을 return 하도록 solution 함수를 작성해주세요.

---

##### 제한사항

0 < `n` ≤ 1000

---

##### 입출력 예

| n   | result |
| --- | --- |
| 10  | 30  |
| 4   | 6   |

---

##### 입출력 예 설명

입출력 예 #1

- `n`이 10이므로 2 + 4 + 6 + 8 + 10 = 30을 return 합니다.

입출력 예 #2

- `n`이 4이므로 2 + 4 = 6을 return 합니다.

def solution(n):

    return sum(i for i in range(1,n+1) if i%2==0)

문제 : <mark>배열의 평균값</mark>

###### 문제 설명

정수 배열 `numbers`가 매개변수로 주어집니다. `numbers`의 원소의 평균값을 return하도록 solution 함수를 완성해주세요.

---

##### 제한사항

- 0 ≤ `numbers`의 원소 ≤ 1,000
- 1 ≤ `numbers`의 길이 ≤ 100
- 정답의 소수 부분이 .0 또는 .5인 경우만 입력으로 주어집니다.

---

##### 입출력 예

| numbers | result |
| --- | --- |
| [1, 2, 3, 4, 5, 6, 7, 8, 9, 10] | 5.5 |
| [89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99] | 94.0 |

---

##### 입출력 예 설명

입출력 예 #1

- `numbers`의 원소들의 평균 값은 5.5입니다.

입출력 예 #2

- `numbers`의 원소들의 평균 값은 94.0입니다.

def solution(numbers):

    answer = 0

    answer = sum(numbers)/len(numbers)

    return answer

문제 : <mark>머쓱이보다 키 큰 사람</mark>


###### 문제 설명

머쓱이는 학교에서 키 순으로 줄을 설 때 몇 번째로 서야 하는지 궁금해졌습니다. 머쓱이네 반 친구들의 키가 담긴 정수 배열 `array`와 머쓱이의 키 `height`가 매개변수로 주어질 때, 머쓱이보다 키 큰 사람 수를 return 하도록 solution 함수를 완성해보세요.

---

##### 제한사항

- 1 ≤ `array`의 길이 ≤ 100
- 1 ≤ `height` ≤ 200
- 1 ≤ `array`의 원소 ≤ 200

---

##### 입출력 예

| array | height | result |
| --- | --- | --- |
| [149, 180, 192, 170] | 167 | 3   |
| [180, 120, 140] | 190 | 0   |

---

##### 입출력 예 설명

입출력 예 #1

- 149, 180, 192, 170 중 머쓱이보다 키가 큰 사람은 180, 192, 170으로 세 명입니다.

입출력 예 #2

- 180, 120, 140 중 190보다 큰 수는 없으므로 0명입니다.

def solution(array, height):

    answer = 0

    for x in array :

        if x > height :

            answer = answer + 1

    return answer
