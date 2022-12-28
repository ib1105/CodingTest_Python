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


문제 : 중복된 숫자 개수

###### 문제 설명

정수가 담긴 배열 `array`와 정수 `n`이 매개변수로 주어질 때, `array`에 `n`이 몇 개 있는 지를 return 하도록 solution 함수를 완성해보세요.

------

##### 제한사항

- 1 ≤ `array`의 길이 ≤ 100
- 0 ≤ `array`의 원소 ≤ 1,000
- 0 ≤ `n` ≤ 1,000

------

##### 입출력 예

| array              | n    | result |
| ------------------ | ---- | ------ |
| [1, 1, 2, 3, 4, 5] | 1    | 2      |
| [0, 2, 3, 4]       | 1    | 0      |

------

##### 입출력 예 설명

입출력 예 #1

- [1, 1, 2, 3, 4, 5] 에는 1이 2개 있습니다.

입출력 예 #2

- [0, 2, 3, 4] 에는 1이 0개 있습니다.



def solution(array, n):
    return array.count(n)
    
    
문제 : 배열 뒤집기

###### 문제 설명

정수가 들어 있는 배열 `num_list`가 매개변수로 주어집니다. `num_list`의 원소의 순서를 거꾸로 뒤집은 배열을 return하도록 solution 함수를 완성해주세요.

------

##### 제한사항

- 1 ≤ `num_list`의 길이 ≤ 1,000
- 0 ≤ `num_list`의 원소 ≤ 1,000

------

##### 입출력 예

| num_list              | result                |
| --------------------- | --------------------- |
| [1, 2, 3, 4, 5]       | [5, 4, 3, 2, 1]       |
| [1, 1, 1, 1, 1, 2]    | [2, 1, 1, 1, 1, 1]    |
| [1, 0, 1, 1, 1, 3, 5] | [5, 3, 1, 1, 1, 0, 1] |

------

##### 입출력 예 설명

입출력 예 #1

- `num_list`가 [1, 2, 3, 4, 5]이므로 순서를 거꾸로 뒤집은 배열 [5, 4, 3, 2, 1]을 return합니다.

입출력 예 #2

- `num_list`가 [1, 1, 1, 1, 1, 2]이므로 순서를 거꾸로 뒤집은 배열 [2, 1, 1, 1, 1, 1]을 return합니다.

입출력 예 #3

- `num_list`가 [1, 0, 1, 1, 1, 3, 5]이므로 순서를 거꾸로 뒤집은 배열 [5, 3, 1, 1, 1, 0, 1]을 return합니다.



def solution(num_list):

  num_list.reverse()

  return num_list    
  
  
문제 : 배열 원소의 길이



###### 문제 설명

문자열 배열 `strlist`가 매개변수로 주어집니다. `strlist` 각 원소의 길이를 담은 배열을 retrun하도록 solution 함수를 완성해주세요.

------

##### 제한사항

- 1 ≤ `strlist` 원소의 길이 ≤ 100
- `strlist`는 알파벳 소문자, 대문자, 특수문자로 구성되어 있습니다.

------

##### 입출력 예

| strlist                        | result       |
| ------------------------------ | ------------ |
| ["We", "are", "the", "world!"] | [2, 3, 3, 6] |
| ["I", "Love", "Programmers."]  | [1, 4, 12]   |

------

##### 입출력 예 설명

입출력 예 #1

- ["We", "are", "the", "world!"]의 각 원소의 길이인 [2, 3, 3, 6]을 return합니다.

입출력 예 #2

- ["I", "Love", "Programmers."]의 각 원소의 길이인 [1, 4, 12]을 return합니다.



def solution(strlist):

  return [len(str) for str in strlist]  
  
  
문제 : 문자열 뒤집기

###### 문제 설명

문자열 `my_string`이 매개변수로 주어집니다. `my_string`을 거꾸로 뒤집은 문자열을 return하도록 solution 함수를 완성해주세요.

------

##### 제한사항

- 1 ≤ `my_string`의 길이 ≤ 1,000

------

##### 입출력 예

| my_string | return  |
| --------- | ------- |
| "jaron"   | "noraj" |
| "bread"   | "daerb" |

------

##### 입출력 예 설명

입출력 예 #1

- `my_string`이 "jaron"이므로 거꾸로 뒤집은 "noraj"를 return합니다.

입출력 예 #2

- `my_string`이 "bread"이므로 거꾸로 뒤집은 "daerb"를 return합니다.



def solution(my_string):

  return my_string[::-1]


문제 : 짝수 홀수 개수

###### 문제 설명

정수가 담긴 리스트 `num_list`가 주어질 때, `num_list`의 원소 중 짝수와 홀수의 개수를 담은 배열을 return 하도록 solution 함수를 완성해보세요.

---

##### 제한사항

- 1 ≤ `num_list`의 길이 ≤ 100
- 0 ≤ `num_list`의 원소 ≤ 1,000

---

##### 입출력 예

| num_list | result |
| --- | --- |
| [1, 2, 3, 4, 5] | [2, 3] |
| [1, 3, 5, 7] | [0, 4] |

---

##### 입출력 예 설명

입출력 예 #1

- [1, 2, 3, 4, 5]에는 짝수가 2, 4로 두 개, 홀수가 1, 3, 5로 세 개 있습니다.

입출력 예 #2

- [1, 3, 5, 7]에는 짝수가 없고 홀수가 네 개 있습니다.

제목 : 삼각형의 완성조건 (1)

###### 문제 설명

선분 세 개로 삼각형을 만들기 위해서는 다음과 같은 조건을 만족해야 합니다.

- 가장 긴 변의 길이는 다른 두 변의 길이의 합보다 작아야 합니다.

삼각형의 세 변의 길이가 담긴 배열 `sides`이 매개변수로 주어집니다. 세 변으로 삼각형을 만들 수 있다면 1, 만들 수 없다면 2를 return하도록 solution 함수를 완성해주세요.

---

##### 제한사항

- `sides`의 원소는 자연수입니다.
- `sides`의 길이는 3입니다.
- 1 ≤ `sides`의 원소 ≤ 1,000

---

##### 입출력 예

| sides | result |
| --- | --- |
| [1, 2, 3] | 2   |
| [3, 6, 2] | 2   |
| [199, 72, 222] | 1   |

---

##### 입출력 예 설명

입출력 예 #1

- 가장 큰 변인 3이 나머지 두 변의 합 3과 같으므로 삼각형을 완성할 수 없습니다. 따라서 2를 return합니다.

입출력 예 #2

- 가장 큰 변인 6이 나머지 두 변의 합 5보다 크므로 삼각형을 완성할 수 없습니다. 따라서 2를 return합니다.

입출력 예 #3

- 가장 큰 변인 222가 나머지 두 변의 합 271보다 작으므로 삼각형을 완성할 수 있습니다. 따라서 1을 return합니다.

def solution(sides):

    sides.sort()

    sum=sides[0]+sides[1]

    if sides[2]<sum:

        return 1

    else:

        return 2

문제 : 최댓값 만들기 (1)

###### 문제 설명

정수 배열 `numbers`가 매개변수로 주어집니다. `numbers`의 원소 중 두 개를 곱해 만들 수 있는 최댓값을 return하도록 solution 함수를 완성해주세요.

---

##### 제한사항

- 0 ≤ `numbers`의 원소 ≤ 10,000
- 2 ≤ `numbers`의 길이 ≤ 100

---

##### 입출력 예

| numbers | result |
| --- | --- |
| [1, 2, 3, 4, 5] | 20  |
| [0, 31, 24, 10, 1, 9] | 744 |

---

##### 입출력 예 설명

입출력 예 #1

- 두 수의 곱중 최댓값은 4 * 5 = 20 입니다.

입출력 예 #1

- 두 수의 곱중 최댓값은 31 * 24 = 744 입니다.

def solution(numbers):

    numbers.sort(reverse=True)

    return numbers[0] * numbers[1]

문제 : 특정 문자 제거하기

###### 문제 설명

문자열 `my_string`과 문자 `letter`이 매개변수로 주어집니다. `my_string`에서 `letter`를 제거한 문자열을 return하도록 solution 함수를 완성해주세요.

---

##### 제한사항

- 1 ≤ `my_string`의 길이 ≤ 100
- `letter`은 길이가 1인 영문자입니다.
- `my_string`과 `letter`은 알파벳 대소문자로 이루어져 있습니다.
- 대문자와 소문자를 구분합니다.

---

##### 입출력 예

| my_string | letter | result |
| --- | --- | --- |
| "abcdef" | "f" | "abcde" |
| "BCBdbe" | "B" | "Cdbe" |

---

##### 입출력 예 설명

입출력 예 #1

- "abcdef" 에서 "f"를 제거한 "abcde"를 return합니다.

입출력 예 #2

- "BCBdbe" 에서 "B"를 모두 제거한 "Cdbe"를 return합니다.

def solution(my_string, letter):    

    return my_string.replace(letter,'')
