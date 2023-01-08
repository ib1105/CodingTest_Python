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
    
    
문제 : 문자 반복 출력하기

###### 문제 설명

문자열 `my_string`과 정수 `n`이 매개변수로 주어질 때, `my_string`에 들어있는 각 문자를 `n`만큼 반복한 문자열을 return 하도록 solution 함수를 완성해보세요.

------

##### 제한사항

- 2 ≤ `my_string` 길이 ≤ 5
- 2 ≤ `n` ≤ 10
- "my_string"은 영어 대소문자로 이루어져 있습니다.

------

##### 입출력 예

| my_string | n    | result            |
| --------- | ---- | ----------------- |
| "hello"   | 3    | "hhheeellllllooo" |

------

##### 입출력 예 설명

입출력 예 #1

- "hello"의 각 문자를 세 번씩 반복한 "hhheeellllllooo"를 return 합니다.

def solution(my_string, n):

  return "".join([s * n for s in my_string])

''.join(리스트)를 이용하면 매개변수로 들어온 ['a', 'b', 'c'] 이런 식의 리스트를 'abc'의 

문자열로 합쳐서 반환해주는 함수인 것입니다.

"".join(array) 배열의 각 원소를 하나의 원소로 합쳐서 반환



문제 : 짝수는 싫어요

###### 문제 설명

정수 `n`이 매개변수로 주어질 때, `n` 이하의 홀수가 오름차순으로 담긴 배열을 return하도록 solution 함수를 완성해주세요.

------

##### 제한사항

- 1 ≤ `n` ≤ 100

------

##### 입출력 예

| n    | result                      |
| ---- | --------------------------- |
| 10   | [1, 3, 5, 7, 9]             |
| 15   | [1, 3, 5, 7, 9, 11, 13, 15] |

------

##### 입출력 예 설명

입출력 #1

- 10 이하의 홀수가 담긴 배열 [1, 3, 5, 7, 9]를 return합니다.

입출력 #1

- 15 이하의 홀수가 담긴 배열 [1, 3, 5, 7, 9, 11, 13, 15]를 return합니다.



def solution(n):

  return [i for i in range(1,n+1) if i%2==1]



문제 : 문자열안에 문자열

###### 문제 설명

문자열 `str1`, `str2`가 매개변수로 주어집니다. `str1` 안에 `str2`가 있다면 1을 없다면 2를 return하도록 solution 함수를 완성해주세요.

------

##### 제한사항

- 1 ≤ `str1`의 길이 ≤ 100
- 1 ≤ `str2`의 길이 ≤ 100

------

##### 입출력 예

| str1                     | str2   | result |
| ------------------------ | ------ | ------ |
| "ab6CDE443fgh22iJKlmn1o" | "6CD"  | 1      |
| "ppprrrogrammers"        | "pppp" | 2      |

------

##### 입출력 예 설명

입출력 예 #1

- "ab`6CD`E443fgh22iJKlmn1o" `str1`에 `str2`가 존재하므로 1을 return합니다.

입출력 예 #2

- "ppprrrogrammers" `str1`에 `str2`가 없으므로 2를 return합니다.



def solution(str1, str2):

  return 1 if str2 in str1 else 2



문제 : 중앙값 구하기

###### 문제 설명

중앙값은 어떤 주어진 값들을 크기의 순서대로 정렬했을 때 가장 중앙에 위치하는 값을 의미합니다. 예를 들어 1, 2, 7, 10, 11의 중앙값은 7입니다. 정수 배열 `array`가 매개변수로 주어질 때, 중앙값을 return 하도록 solution 함수를 완성해보세요.

------

##### 제한사항

- `array`의 길이는 홀수입니다.
- 0 < `array`의 길이 < 100
- -1,000 < `array`의 원소 < 1,000

------

##### 입출력 예

| array             | result |
| ----------------- | ------ |
| [1, 2, 7, 10, 11] | 7      |
| [9, -1, 0]        | 0      |

------

##### 입출력 예 설명

입출력 예 #1

- 본문과 동일합니다.

입출력 예 #2

- 9, -1, 0을 오름차순 정렬하면 -1, 0, 9이고 가장 중앙에 위치하는 값은 0입니다.



def solution(array):

  array.sort();   

  index = int(len(array)/2)

  return array[index]



array[index] : 배열의 n번째 요소 구하는법



문제 : 배열의 유사도

###### 문제 설명

두 배열이 얼마나 유사한지 확인해보려고 합니다. 문자열 배열 `s1`과 `s2`가 주어질 때 같은 원소의 개수를 return하도록 solution 함수를 완성해주세요.

------

##### 제한사항

- 1 ≤ `s1`, `s2`의 길이 ≤ 100
- 1 ≤ `s1`, `s2`의 원소의 길이 ≤ 10
- `s1`과 `s2`의 원소는 알파벳 소문자로만 이루어져 있습니다
- `s1`과 `s2`는 각각 중복된 원소를 갖지 않습니다.

------

##### 입출력 예

| s1              | s2                          | result |
| --------------- | --------------------------- | ------ |
| ["a", "b", "c"] | ["com", "b", "d", "p", "c"] | 2      |
| ["n", "omg"]    | ["m", "dot"]                | 0      |

------

##### 입출력 예 설명

입출력 예 #1

- "b"와 "c"가 같으므로 2를 return합니다.

입출력 예 #2

- 같은 원소가 없으므로 0을 return합니다.

def solution(s1, s2):

  return len(set(s1) & set(s2))



set은 집합을 만들어주는 함수이다.

합집합 | 

교집합 &

차집합 -

교집합을 제외한 나머지 ^



문제 : 자릿수 더하기

###### 문제 설명

정수 `n`이 매개변수로 주어질 때 `n`의 각 자리 숫자의 합을 return하도록 solution 함수를 완성해주세요

------

##### 제한사항

- 0 ≤ `n` ≤ 1,000,000

------

##### 입출력 예

| n      | result |
| ------ | ------ |
| 1234   | 10     |
| 930211 | 16     |

------

##### 입출력 예 설명

입출력 예 #1

- 1 + 2 + 3 + 4 = 10을 return합니다.

입출력 예 #2

- 9 + 3 + 0 + 2 + 1 + 1 = 16을 return합니다.



def solution(n):

  array = list(map(int,str(n)))

  return sum(i for i in array)



map(함수,리스트)

map(함수, 튜플)

map: 리스트나, 튜플에 하나하나씩 접근하여 함수로 변환(int로 변환), 그리고 list 형식으로 저장



문제 : 제곱수 판별하기

###### 문제 설명

어떤 자연수를 제곱했을 때 나오는 정수를 제곱수라고 합니다. 정수 `n`이 매개변수로 주어질 때, `n`이 제곱수라면 1을 아니라면 2를 return하도록 solution 함수를 완성해주세요.

------

##### 제한사항

- 1 ≤ `n` ≤ 1,000,000

------

##### 입출력 예

| n    | result |
| ---- | ------ |
| 144  | 1      |
| 976  | 2      |

------

##### 입출력 예 설명

입출력 예 #1

- 144는 12의 제곱이므로 제곱수입니다. 따라서 1을 return합니다.

입출력 예 #2

- 976은 제곱수가 아닙니다. 따라서 2를 return합니다.



import math



def solution(n):   

  a = math.sqrt(n)

  if int(a) == a:

​    return 1

  else:

​    return 2

print(solution(144))



math함수, sqrt : 제곱근 구하는 함수. ex) 144 = 12



문제 : 순서쌍의 개수

###### 문제 설명

순서쌍이란 두 개의 숫자를 순서를 정하여 짝지어 나타낸 쌍으로 (a, b)로 표기합니다. 자연수 `n`이 매개변수로 주어질 때 두 숫자의 곱이 `n`인 자연수 순서쌍의 개수를 return하도록 solution 함수를 완성해주세요.

------

##### 제한사항

- 1 ≤ n ≤ 1,000,000

------

##### 입출력 예

| n    | result |
| ---- | ------ |
| 20   | 6      |
| 100  | 9      |

------

##### 입출력 예 설명

입출력 예 #1

- `n`이 20 이므로 곱이 20인 순서쌍은 (1, 20), (2, 10), (4, 5), (5, 4), (10, 2), (20, 1) 이므로 6을 return합니다.

입출력 예 #2

- `n`이 100 이므로 곱이 100인 순서쌍은 (1, 100), (2, 50), (4, 25), (5, 20), (10, 10), (20, 5), (25, 4), (50, 2), (100, 1) 이므로 9를 return합니다.



def solution(n):

  count = 0

  for i in range(1,n+1):

​    if n%i == 0:

​      count += 1



  return count

print(solution(100))



약수구하는법이다 

n값 / 1부터 n까지 의 값 중 나머지가 0인 값이 약수이다.



문제 : 숨어있는 숫자의 덧셈 (1)

###### 문제 설명

문자열 `my_string`이 매개변수로 주어집니다. `my_string`안의 모든 자연수들의 합을 return하도록 solution 함수를 완성해주세요.

------

##### 제한사항

- 1 ≤ `my_string`의 길이 ≤ 1,000
- `my_string`은 소문자, 대문자 그리고 한자리 자연수로만 구성되어있습니다.

------

##### 입출력 예

| my_string       | result |
| --------------- | ------ |
| "aAb1B2cC34oOp" | 10     |
| "1a2b3c4d123"   | 16     |

------

##### 입출력 예 설명

입출력 예 #1

- "aAb1B2cC34oOp"안의 한자리 자연수는 1, 2, 3, 4 입니다. 따라서 1 + 2 + 3 + 4 = 10 을 return합니다.

입출력 예 #2

- "1a2b3c4d123Z"안의 한자리 자연수는 1, 2, 3, 4, 1, 2, 3 입니다. 따라서 1 + 2 + 3 + 4 + 1 + 2 + 3 = 16 을 return합니다.

def solution(my_string):

  return sum(int(i) for i in my_string if i.isnumeric())

​    

print(solution("aAb1B2cC34oOp"))    


문제 : 대문자와 소문자

###### 문제 설명

문자열 `my_string`이 매개변수로 주어질 때, 대문자는 소문자로 소문자는 대문자로 변환한 문자열을 return하도록 solution 함수를 완성해주세요.

---

##### 제한사항

- 1 ≤ `my_string`의 길이 ≤ 1,000
- `my_string`은 영어 대문자와 소문자로만 구성되어 있습니다.

---

##### 입출력 예

| my_string | result |
| --- | --- |
| "cccCCC" | "CCCccc" |
| "abCdEfghIJ" | "ABcDeFGHij" |

---

##### 입출력 예 설명

입출력 예 #1

- 소문자는 대문자로 대문자는 소문자로 바꾼 "CCCccc"를 return합니다.

입출력 예 #2

- 소문자는 대문자로 대문자는 소문자로 바꾼 "ABcDeFGHij"를 return합니다.

def solution(my_string):

    answer = ''

    for i in my_string:

        if i.isupper():

            answer+=i.lower()

        else:

            answer+=i.upper()

    return answer

print(solution("cccCCC"))

문제 : 암호 해독

###### 문제 설명

군 전략가 머쓱이는 전쟁 중 적군이 다음과 같은 암호 체계를 사용한다는 것을 알아냈습니다.

- 암호화된 문자열 `cipher`를 주고받습니다.
- 그 문자열에서 `code`의 배수 번째 글자만 진짜 암호입니다.

문자열 `cipher`와 정수 `code`가 매개변수로 주어질 때 해독된 암호 문자열을 return하도록 solution 함수를 완성해주세요.

---

##### 제한사항

- 1 ≤ `cipher`의 길이 ≤ 1,000
- 1 ≤ `code` ≤ `cipher`의 길이
- `cipher`는 소문자와 공백으로만 구성되어 있습니다.
- 공백도 하나의 문자로 취급합니다.

---

##### 입출력 예

| cipher | code | result |
| --- | --- | --- |
| "dfjardstddetckdaccccdegk" | 4   | "attack" |
| "pfqallllabwaoclk" | 2   | "fallback" |

---

##### 입출력 예 설명

입출력 예 #1

- "dfjardstddetckdaccccdegk" 의 4번째, 8번째, 12번째, 16번째, 20번째, 24번째 글자를 합친 "attack"을 return합니다.

입출력 예 #2

- "pfqallllabwaoclk" 의 2번째, 4번째, 6번째, 8번째, 10번째, 12번째, 14번째, 16번째 글자를 합친 "fallback"을 return합니다.

def solution(cipher, code):

    return cipher[code-1::code]

print(solution("dfjardstddetckdaccccdegk",4))

arr[A:B:C]의 의미는, index A 부터 index B 까지 C의 간격으로 배열을 만들어라는 말입니다.

문제:주사위의 개수

###### 문제 설명

머쓱이는 직육면체 모양의 상자를 하나 가지고 있는데 이 상자에 정육면체 모양의 주사위를 최대한 많이 채우고 싶습니다. 상자의 가로, 세로, 높이가 저장되어있는 배열 `box`와 주사위 모서리의 길이 정수 `n`이 매개변수로 주어졌을 때, 상자에 들어갈 수 있는 주사위의 최대 개수를 return 하도록 solution 함수를 완성해주세요.

---

##### 제한사항

- `box`의 길이는 3입니다.
- `box[0]` = 상자의 가로 길이
- `box[1]` = 상자의 세로 길이
- `box[2]` = 상자의 높이 길이
- 1 ≤ `box`의 원소 ≤ 100
- 1 ≤ `n` ≤ 50
- `n` ≤ `box`의 원소
- 주사위는 상자와 평행하게 넣습니다.

---

##### 입출력 예

| box | n   | result |
| --- | --- | --- |
| [1, 1, 1] | 1   | 1   |
| [10, 8, 6] | 3   | 12  |

##### 입출력 예 설명

입출력 예 #1

- 상자의 크기가 가로 1, 세로 1, 높이 1이므로 모서리의 길이가 1인 주사위는 1개 들어갈 수 있습니다.

입출력 예 #2

- 상자의 크기가 가로 10, 세로 8, 높이 6이므로 모서리의 길이가 3인 주사위는 12개 들어갈 수 있습니다.

def solution(box, n):

    answer = []

    for i in box:

        answer.append(i//n)

    return answer[0]*answer[1]*answer[2]

print(solution([10, 8, 6],1))

문제:문자열 정렬하기 (1)

###### 문제 설명

문자열 `my_string`이 매개변수로 주어질 때, `my_string` 안에 있는 숫자만 골라 오름차순 정렬한 리스트를 return 하도록 solution 함수를 작성해보세요.

---

##### 제한사항

- 1 ≤ `my_string`의 길이 ≤ 100
- `my_string`에는 숫자가 한 개 이상 포함되어 있습니다.
- `my_string`은 영어 소문자 또는 0부터 9까지의 숫자로 이루어져 있습니다. - - -

##### 입출력 예

| my_string | result |
| --- | --- |
| "hi12392" | [1, 2, 2, 3, 9] |
| "p2o4i8gj2" | [2, 2, 4, 8] |
| "abcde0" | [0] |

---

##### 입출력 예 설명

입출력 예 #1

- "hi12392"에 있는 숫자 1, 2, 3, 9, 2를 오름차순 정렬한 [1, 2, 2, 3, 9]를 return 합니다.

입출력 예 #2

- "p2o4i8gj2"에 있는 숫자 2, 4, 8, 2를 오름차순 정렬한 [2, 2, 4, 8]을 return 합니다.

입출력 예 #3

- "abcde0"에 있는 숫자 0을 오름차순 정렬한 [0]을 return 합니다.

def solution(my_string):
 answer = []
 for i in my_string:
 if i.isdigit():
 answer.append(int(i))
 answer.sort()
 return answer

int(i)를 사용하여 배열에 넣을때 int형으로 넣는다.(default: "문자")

문제: 가장 큰 수 찾기

###### 문제 설명

정수 배열 `array`가 매개변수로 주어질 때, 가장 큰 수와 그 수의 인덱스를 담은 배열을 return 하도록 solution 함수를 완성해보세요.

---

##### 제한사항

- 1 ≤ `array의` 길이 ≤ 100
- 0 ≤ `array` 원소 ≤ 1,000
- `array`에 중복된 숫자는 없습니다.

---

##### 입출력 예

| array | result |
| --- | --- |
| [1, 8, 3] | [8, 1] |
| [9, 10, 11, 8] | [11, 2] |

---

##### 입출력 예 설명

입출력 예 #1

- 1, 8, 3 중 가장 큰 수는 8이고 인덱스 1에 있습니다.

입출력 예 #2

- 9, 10, 11, 8 중 가장 큰 수는 11이고 인덱스 2에 있습니다.

def solution(array):

    return [max(array), array.index(max(array))]

print(solution([1, 8, 3]))

문제: 배열 회전시키기

###### 문제 설명

정수가 담긴 배열 `numbers`와 문자열 `direction`가 매개변수로 주어집니다. 배열 `numbers`의 원소를 `direction`방향으로 한 칸씩 회전시킨 배열을 return하도록 solution 함수를 완성해주세요.

---

##### 제한사항

- 3 ≤ `numbers`의 길이 ≤ 20
- `direction`은 "left" 와 "right" 둘 중 하나입니다.

---

##### 입출력 예

| numbers | direction | result |
| --- | --- | --- |
| [1, 2, 3] | "right" | [3, 1, 2] |
| [4, 455, 6, 4, -1, 45, 6] | "left" | [455, 6, 4, -1, 45, 6, 4] |

---

##### 입출력 예 설명

입출력 예 #1

- `numbers` 가 [1, 2, 3]이고 `direction`이 "right" 이므로 오른쪽으로 한 칸씩 회전시킨 [3, 1, 2]를 return합니다.

입출력 예 #2

- `numbers` 가 [4, 455, 6, 4, -1, 45, 6]이고 `direction`이 "left" 이므로 왼쪽으로 한 칸씩 회전시킨 [455, 6, 4, -1, 45, 6, 4]를 return합니다.

def solution(numbers, direction):

    if direction == "right":

        answer = [numbers[-1]] + numbers[:len(numbers)-1]

    else:

        answer = numbers[1:] + [numbers[0]]

    return answer

print(solution([1, 2, 3],"right"))

ex) num[:5] = 배열 0~5까지

num[1:] = 배열 1부터 끝까지

문제: 최댓값 만들기 (2)

###### 문제 설명

정수 배열 `numbers`가 매개변수로 주어집니다. `numbers`의 원소 중 두 개를 곱해 만들 수 있는 최댓값을 return하도록 solution 함수를 완성해주세요.

---

##### 제한사항

- -10,000 ≤ `numbers`의 원소 ≤ 10,000
- 2 ≤ `numbers` 의 길이 ≤ 100

---

##### 입출력 예

| numbers | result |
| --- | --- |
| [1, 2, -3, 4, -5] | 15  |
| [0, -31, 24, 10, 1, 9] | 240 |
| [10, 20, 30, 5, 5, 20, 5] | 600 |

---

##### 입출력 예 설명

입출력 예 #1

- 두 수의 곱중 최댓값은 -3 * -5 = 15 입니다.

입출력 예 #2

- 두 수의 곱중 최댓값은 10 * 24 = 240 입니다.

입출력 예 #3

- 두 수의 곱중 최댓값은 20 * 30 = 600 입니다.

def solution(numbers):

    numbers.sort()

    return max(numbers[0] * numbers[1], numbers[-1] * numbers[-2])

print(solution([1, 2, -3, 4, -5]))

문제:피자 나눠 먹기 (2)

###### 문제 설명

머쓱이네 피자가게는 피자를 여섯 조각으로 잘라 줍니다. 피자를 나눠먹을 사람의 수 `n`이 매개변수로 주어질 때, `n`명이 주문한 피자를 남기지 않고 모두 같은 수의 피자 조각을 먹어야 한다면 최소 몇 판을 시켜야 하는지를 return 하도록 solution 함수를 완성해보세요.

---

##### 제한사항

1 ≤ `n` ≤ 100

---

##### 입출력 예

| n   | result |
| --- | --- |
| 6   | 1   |
| 10  | 5   |
| 4   | 2   |

---

##### 입출력 예 설명

입출력 예 #1

- 6명이 모두 같은 양을 먹기 위해 한 판을 시켜야 피자가 6조각으로 모두 한 조각씩 먹을 수 있습니다.

입출력 예 #2

- 10명이 모두 같은 양을 먹기 위해 최소 5판을 시켜야 피자가 30조각으로 모두 세 조각씩 먹을 수 있습니다.

입출력 예 #3

- 4명이 모두 같은 양을 먹기 위해 최소 2판을 시키면 피자가 12조각으로 모두 세 조각씩 먹을 수 있습니다.

def solution(n):

    answer = 1

    while answer * 6 % n != 0:

        answer += 1

    return answer

print(solution(6))

문제 : 인덱스 바꾸기

###### 문제 설명

문자열 `my_string`과 정수 `num1`, `num2`가 매개변수로 주어질 때, `my_string`에서 인덱스 `num1`과 인덱스 `num2`에 해당하는 문자를 바꾼 문자열을 return 하도록 solution 함수를 완성해보세요.

---

##### 제한사항

- 1 < `my_string`의 길이 < 100
- 0 ≤ `num1`, `num2` < `my_string`의 길이
- `my_string`은 소문자로 이루어져 있습니다.
- `num1` ≠ `num2`

---

##### 입출력 예

| my_string | num1 | num2 | result |
| --- | --- | --- | --- |
| "hello" | 1   | 2   | "hlelo" |
| "I love you" | 3   | 6   | "I l veoyou" |

---

##### 입출력 예 설명

입출력 예 #1

- "hello"의 1번째 인덱스인 "e"와 2번째 인덱스인 "l"을 바꾸면 "hlelo"입니다.

입출력 예 #2

- "I love you"의 3번째 인덱스 "o"와 " "(공백)을 바꾸면 "I l veoyou"입니다.

def solution(my_string, num1, num2):

    A = list(my_string)

    A[num1], A[num2] = A[num2], A[num1]

    answer = ''.join(A)

    return answer

print(solution("hello",1,2))


문제 : 자릿수 더하기

###### 문제 설명

자연수 N이 주어지면, N의 각 자릿수의 합을 구해서 return 하는 solution 함수를 만들어 주세요.
예를들어 N = 123이면 1 + 2 + 3 = 6을 return 하면 됩니다.

##### 제한사항

- N의 범위 : 100,000,000 이하의 자연수

------

##### 입출력 예

| N    | answer |
| ---- | ------ |
| 123  | 6      |
| 987  | 24     |

##### 입출력 예 설명

입출력 예 #1
문제의 예시와 같습니다.

입출력 예 #2
9 + 8 + 7 = 24이므로 24를 return 하면 됩니다.

def solution(n):
    answer = list(map(str,str(n)))
    return sum(int(i) for i in answer)



문제:평균 구하기

###### 문제 설명

정수를 담고 있는 배열 arr의 평균값을 return하는 함수, solution을 완성해보세요.

#### 제한사항

- arr은 길이 1 이상, 100 이하인 배열입니다.
- arr의 원소는 -10,000 이상 10,000 이하인 정수입니다.

#### 입출력 예

| arr       | return |
| --------- | :----: |
| [1,2,3,4] |  2.5   |
| [5,5]     |   5    |

def solution(arr):
    answer = 0
    return sum(arr)/ len(arr)



문제: 자연수 뒤집어 배열로 만들기

###### 문제 설명

자연수 n을 뒤집어 각 자리 숫자를 원소로 가지는 배열 형태로 리턴해주세요. 예를들어 n이 12345이면 [5,4,3,2,1]을 리턴합니다.

##### 제한 조건

- n은 10,000,000,000이하인 자연수입니다.

##### 입출력 예

| n     | return      |
| ----- | ----------- |
| 12345 | [5,4,3,2,1] |

def solution(n):
    answer = list(map(int,str(n)))
    

    return answer[::-1]



참고)https://blockdmask.tistory.com/425

리스트 방식


제목: 문자열 내 p와 y의 개수

###### 문제 설명

대문자와 소문자가 섞여있는 문자열 s가 주어집니다. s에 'p'의 개수와 'y'의 개수를 비교해 같으면 True, 다르면 False를 return 하는 solution를 완성하세요. 'p', 'y' 모두 하나도 없는 경우는 항상 True를 리턴합니다. 단, 개수를 비교할 때 대문자와 소문자는 구별하지 않습니다.

예를 들어 s가 "pPoooyY"면 true를 return하고 "Pyy"라면 false를 return합니다.

##### 제한사항

- 문자열 s의 길이 : 50 이하의 자연수
- 문자열 s는 알파벳으로만 이루어져 있습니다.

---

##### 입출력 예

| s   | answer |
| --- | --- |
| "pPoooyY" | true |
| "Pyy" | false |

##### 입출력 예 설명

입출력 예 #1  
'p'의 개수 2개, 'y'의 개수 2개로 같으므로 true를 return 합니다.

입출력 예 #2  
'p'의 개수 1개, 'y'의 개수 2개로 다르므로 false를 return 합니다.

※ 공지 - 2021년 8월 23일 테스트케이스가 추가되었습니다.

def solution(s):

    # 함수를 완성하세요

    return s.lower().count('p') == s.lower().count('y')
    
    
문제 : 핸드폰 번호 가리기

###### 문제 설명

프로그래머스 모바일은 개인정보 보호를 위해 고지서를 보낼 때 고객들의 전화번호의 일부를 가립니다.  
전화번호가 문자열 phone_number로 주어졌을 때, 전화번호의 뒷 4자리를 제외한 나머지 숫자를 전부 `*`으로 가린 문자열을 리턴하는 함수, solution을 완성해주세요.

##### 제한 조건

- phone_number는 길이 4 이상, 20이하인 문자열입니다.

##### 입출력 예

| phone_number | return |
| --- | --- |
| "01033334444" | "*******4444" |
| "027778888" | "*****8888" |

def solution(s):

  return '*' * (len(s) - 4) + s[-4:]

print(solution("01033334444"))

문제:나누어 떨어지는 숫자 배열

###### 문제 설명

array의 각 element 중 divisor로 나누어 떨어지는 값을 오름차순으로 정렬한 배열을 반환하는 함수, solution을 작성해주세요.  
divisor로 나누어 떨어지는 element가 하나도 없다면 배열에 -1을 담아 반환하세요.

##### 제한사항

- arr은 자연수를 담은 배열입니다.
- 정수 i, j에 대해 i ≠ j 이면 arr[i] ≠ arr[j] 입니다.
- divisor는 자연수입니다.
- array는 길이 1 이상인 배열입니다.

##### 입출력 예

| arr | divisor | return |
| --- | --- | --- |
| [5, 9, 7, 10] | 5   | [5, 10] |
| [2, 36, 1, 3] | 1   | [1, 2, 3, 36] |
| [3,2,6] | 10  | [-1] |

##### 입출력 예 설명

입출력 예#1  
arr의 원소 중 5로 나누어 떨어지는 원소는 5와 10입니다. 따라서 [5, 10]을 리턴합니다.

입출력 예#2  
arr의 모든 원소는 1으로 나누어 떨어집니다. 원소를 오름차순으로 정렬해 [1, 2, 3, 36]을 리턴합니다.

입출력 예#3  
3, 2, 6은 10으로 나누어 떨어지지 않습니다. 나누어 떨어지는 원소가 없으므로 [-1]을 리턴합니다.

def solution(arr, divisor):

    answer = [i for i in arr if i % divisor == 0]

    answer.sort()

    if answer == []:

        answer = [-1]

        return answer

    return answer

print(solution([3,2,6],10))

문제:제일 작은 수 제거하기

###### 문제 설명

정수를 저장한 배열, arr 에서 가장 작은 수를 제거한 배열을 리턴하는 함수, solution을 완성해주세요. 단, 리턴하려는 배열이 빈 배열인 경우엔 배열에 -1을 채워 리턴하세요. 예를들어 arr이 [4,3,2,1]인 경우는 [4,3,2]를 리턴 하고, [10]면 [-1]을 리턴 합니다.

##### 제한 조건

- arr은 길이 1 이상인 배열입니다.
- 인덱스 i, j에 대해 i ≠ j이면 arr[i] ≠ arr[j] 입니다.

##### 입출력 예

| arr | return |
| --- | --- |
| [4,3,2,1] | [4,3,2] |
| [10] | [-1] |

def solution(mylist):

    mylist.remove(min(mylist))

    return mylist

print(solution([4,3,2,1,0]))

문제:합성수 찾기

###### 문제 설명

약수의 개수가 세 개 이상인 수를 합성수라고 합니다. 자연수 `n`이 매개변수로 주어질 때 `n`이하의 합성수의 개수를 return하도록 solution 함수를 완성해주세요.

---

##### 제한사항

- 1 ≤ `n` ≤ 100

---

##### 입출력 예

| n   | result |
| --- | --- |
| 10  | 5   |
| 15  | 8   |

---

##### 입출력 예 설명

입출력 예 #1

- 10 이하 합성수는 4, 6, 8, 9, 10 로 5개입니다. 따라서 5를 return합니다.

입출력 예 #1

- 15 이하 합성수는 4, 6, 8, 9, 10, 12, 14, 15 로 8개입니다. 따라서 8을 return합니다.

def solution(n):

    answer = 0

    for i in range(1, n+1):

        cnt = 0

        for j in range(1, i+1):

            if i % j == 0:

                cnt += 1

        if cnt >= 3:

            answer += 1

    return answer

print(solution(10))

문제:음양 더하기

###### 문제 설명

어떤 정수들이 있습니다. 이 정수들의 절댓값을 차례대로 담은 정수 배열 absolutes와 이 정수들의 부호를 차례대로 담은 불리언 배열 signs가 매개변수로 주어집니다. 실제 정수들의 합을 구하여 return 하도록 solution 함수를 완성해주세요.

---

##### 제한사항

- absolutes의 길이는 1 이상 1,000 이하입니다.
  - absolutes의 모든 수는 각각 1 이상 1,000 이하입니다.
- signs의 길이는 absolutes의 길이와 같습니다.
  - `signs[i]` 가 참이면 `absolutes[i]` 의 실제 정수가 양수임을, 그렇지 않으면 음수임을 의미합니다.

---

##### 입출력 예

| absolutes | signs | result |
| --- | --- | --- |
| `[4,7,12]` | `[true,false,true]` | 9   |
| `[1,2,3]` | `[false,false,true]` | 0   |

---

##### 입출력 예 설명

**입출력 예 #1**

- signs가 `[true,false,true]` 이므로, 실제 수들의 값은 각각 4, -7, 12입니다.
- 따라서 세 수의 합인 9를 return 해야 합니다.

**입출력 예 #2**

- signs가 `[false,false,true]` 이므로, 실제 수들의 값은 각각 -1, -2, 3입니다.
- 따라서 세 수의 합인 0을 return 해야 합니다.

def solution(absolutes, signs):

    res = []

    for idx in range(len(signs)):

        if signs[idx] == True:

            res.append(absolutes[idx])

        else:

            res.append(-absolutes[idx])

    return sum(res)

print(solution([4,7,12], [True,False,True]))

문제:중복된 문자 제거

###### 문제 설명

문자열 `my_string`이 매개변수로 주어집니다. `my_string`에서 중복된 문자를 제거하고 하나의 문자만 남긴 문자열을 return하도록 solution 함수를 완성해주세요.

---

##### 제한사항

- 1 ≤ `my_string` ≤ 110
- `my_string`은 대문자, 소문자, 공백으로 구성되어 있습니다.
- 대문자와 소문자를 구분합니다.
- 공백(" ")도 하나의 문자로 구분합니다.
- 중복된 문자 중 가장 앞에 있는 문자를 남깁니다.

---

##### 입출력 예

| my_string | result |
| --- | --- |
| "people" | "peol" |
| "We are the world" | "We arthwold" |

---

##### 입출력 예 설명

입출력 예 #1

- "people"에서 중복된 문자 "p"와 "e"을 제거한 "peol"을 return합니다.

입출력 예 #2

- "We are the world"에서 중복된 문자 "e", " ", "r" 들을 제거한 "We arthwold"을 return합니다.

def solution(my_string):
 answer = ''.join(dict.fromkeys(my_string))
 return answer

dict.fromkeys(리스트) : 리스트의 중복제거, 문자열로 되어있는 입력을 dict.fromkeys를 사용하면 배열로 하나 하나씩 출력된다.

문제:모스부호 (1)

###### 문제 설명

머쓱이는 친구에게 모스부호를 이용한 편지를 받았습니다. 그냥은 읽을 수 없어 이를 해독하는 프로그램을 만들려고 합니다. 문자열 `letter`가 매개변수로 주어질 때, `letter`를 영어 소문자로 바꾼 문자열을 return 하도록 solution 함수를 완성해보세요.  
모스부호는 다음과 같습니다.

```
morse = { 
    '.-':'a','-...':'b','-.-.':'c','-..':'d','.':'e','..-.':'f',
    '--.':'g','....':'h','..':'i','.---':'j','-.-':'k','.-..':'l',
    '--':'m','-.':'n','---':'o','.--.':'p','--.-':'q','.-.':'r',
    '...':'s','-':'t','..-':'u','...-':'v','.--':'w','-..-':'x',
    '-.--':'y','--..':'z'
}
```

---

##### 제한사항

- 1 ≤ `letter`의 길이 ≤ 1,000
- return값은 소문자입니다.
- `letter`의 모스부호는 공백으로 나누어져 있습니다.
- `letter`에 공백은 연속으로 두 개 이상 존재하지 않습니다.
- 해독할 수 없는 편지는 주어지지 않습니다.
- 편지의 시작과 끝에는 공백이 없습니다.

---

##### 입출력 예

| letter | result |
| --- | --- |
| ".... . .-.. .-.. ---" | "hello" |
| ".--. -.-- - .... --- -." | "python" |

---

##### 입출력 예 설명

입출력 예 #1

- .... = h
- . = e
- .-.. = l
- .-.. = l
- --- = o
- 따라서 "hello"를 return 합니다.

입출력 예 #2

- .--. = p
- -.-- = y
- - = t
- .... = h
- --- = o
- -. = n
- 따라서 "python"을 return 합니다.

---

- a ~ z에 해당하는 모스부호가 순서대로 담긴 배열입니다.
- `{".-","-...","-.-.","-..",".","..-.","--.","....","..",".---","-.-",".-..","--","-.","---",".--.","--.-",".-.","...","-","..-","...-",".--","-..-","-.--","--.."}`

def solution(letter):

    morse = {

        '.-':'a','-...':'b','-.-.':'c','-..':'d','.':'e','..-.':'f',

        '--.':'g','....':'h','..':'i','.---':'j','-.-':'k','.-..':'l',

        '--':'m','-.':'n','---':'o','.--.':'p','--.-':'q','.-.':'r',

        '...':'s','-':'t','..-':'u','...-':'v','.--':'w','-..-':'x',

        '-.--':'y','--..':'z'

    }

    return ''.join([morse[i] for i in letter.split(' ')])

print(solution(".... . .-.. .-.. ---"))

- 파이썬에서 {}형식으로 되어있는 것은 dict, dictionary형식으로 'key' : value 형식으로 구성되어있다.

문제:가운데 글자 가져오기

###### 문제 설명

단어 s의 가운데 글자를 반환하는 함수, solution을 만들어 보세요. 단어의 길이가 짝수라면 가운데 두글자를 반환하면 됩니다.

###### 재한사항

- s는 길이가 1 이상, 100이하인 스트링입니다.

##### 입출력 예

| s   | return |
| --- | --- |
| "abcde" | "c" |
| "qwer" | "we" |

def solution(s):
 center = int(len(s)/2)
 if len(s) % 2 != 0:
 return s[center]
 else:
 return s[center-1:center+1]
 
 문제 : 2차원으로 만들기

###### 문제 설명

정수 배열 `num_list`와 정수 `n`이 매개변수로 주어집니다. `num_list`를 다음 설명과 같이 2차원 배열로 바꿔 return하도록 solution 함수를 완성해주세요.

`num_list`가 [1, 2, 3, 4, 5, 6, 7, 8] 로 길이가 8이고 `n`이 2이므로 `num_list`를 2 * 4 배열로 다음과 같이 변경합니다. 2차원으로 바꿀 때에는 num_list의 원소들을 앞에서부터 n개씩 나눠 2차원 배열로 변경합니다.

| num_list | n   | result |
| --- | --- | --- |
| [1, 2, 3, 4, 5, 6, 7, 8] | 2   | [[1, 2], [3, 4], [5, 6], [7, 8]] |

---

##### 제한사항

- `num_list`의 길이는 `n`의 배 수개입니다.
- 0 ≤ `num_list`의 길이 ≤ 150
- 2 ≤ `n` < `num_list`의 길이

---

##### 입출력 예

| num_list | n   | result |
| --- | --- | --- |
| [1, 2, 3, 4, 5, 6, 7, 8] | 2   | [[1, 2], [3, 4], [5, 6], [7, 8]] |
| [100, 95, 2, 4, 5, 6, 18, 33, 948] | 3   | [[100, 95, 2], [4, 5, 6], [18, 33, 948]] |

---

##### 입출력 예 설명

입출력 예 #1

- `num_list`가 [1, 2, 3, 4, 5, 6, 7, 8] 로 길이가 8이고 `n`이 2이므로 2 * 4 배열로 변경한 [[1, 2], [3, 4], [5, 6], [7, 8]] 을 return합니다.

입출력 예 #2

- `num_list`가 [100, 95, 2, 4, 5, 6, 18, 33, 948] 로 길이가 9이고 `n`이 3이므로 3 * 3 배열로 변경한 [[100, 95, 2], [4, 5, 6], [18, 33, 948]] 을 return합니다.

def solution(num_list, n):

    answer = []

    for i in range(0, len(num_list), n):

        answer.append(num_list[i:i+n])

    return answer

print(solution([1, 2, 3, 4, 5, 6, 7, 8],2))

문제 : 내적

###### 문제 설명

길이가 같은 두 1차원 정수 배열 a, b가 매개변수로 주어집니다. a와 b의 [내적](https://en.wikipedia.org/wiki/Dot_product)을 return 하도록 solution 함수를 완성해주세요.

이때, a와 b의 내적은 `a[0]*b[0] + a[1]*b[1] + ... + a[n-1]*b[n-1]` 입니다. (n은 a, b의 길이)

---

##### 제한사항

- a, b의 길이는 1 이상 1,000 이하입니다.
- a, b의 모든 수는 -1,000 이상 1,000 이하입니다.

---

##### 입출력 예

| a   | b   | result |
| --- | --- | --- |
| `[1,2,3,4]` | `[-3,-1,0,2]` | 3   |
| `[-1,0,1]` | `[1,0,-1]` | -2  |

---

##### 입출력 예 설명

입출력 예 #1

- a와 b의 내적은 `1*(-3) + 2*(-1) + 3*0 + 4*2 = 3` 입니다.

입출력 예 #2

- a와 b의 내적은 `(-1)*1 + 0*0 + 1*(-1) = -2` 입니다.

def solution(a, b):

    return sum([x*y for x, y in zip(a,b)])

print(solution([1,2,3,4],[-3,-1,0,2]))

zip : 각 배열의 원소들을 쌍으로 뽑는 것

문제 : 한 번만 등장한 문자

###### 문제 설명

문자열 `s`가 매개변수로 주어집니다. `s`에서 한 번만 등장하는 문자를 사전 순으로 정렬한 문자열을 return 하도록 solution 함수를 완성해보세요. 한 번만 등장하는 문자가 없을 경우 빈 문자열을 return 합니다.

---

##### 제한사항

- 0 < `s`의 길이 < 1,000
- `s`는 소문자로만 이루어져 있습니다.

---

##### 입출력 예

| s   | result |
| --- | --- |
| "abcabcadc" | "d" |
| "abdc" | "abcd" |
| "hello" | "eho" |

---

##### 입출력 예 설명

입출력 예 #1

- "abcabcadc"에서 하나만 등장하는 문자는 "d"입니다.

입출력 예 #2

- "abdc"에서 모든 문자가 한 번씩 등장하므로 사전 순으로 정렬한 "abcd"를 return 합니다.

입출력 예 #3

- "hello"에서 한 번씩 등장한 문자는 "heo"이고 이를 사전 순으로 정렬한 "eho"를 return 합니다.

def solution(s):

    answer = "".join(sorted([ ch for ch in s if s.count(ch) == 1]))

    return answer

print(solution("hello"))

s.count(i) = 배열 s에서 매개변수 i의 갯수

문제 : 이진수 더하기

###### 문제 설명

이진수를 의미하는 두 개의 문자열 `bin1`과 `bin2`가 매개변수로 주어질 때, 두 이진수의 합을 return하도록 solution 함수를 완성해주세요.

---

##### 제한사항

- return 값은 이진수를 의미하는 문자열입니다.
- 1 ≤ `bin1`, `bin2`의 길이 ≤ 10
- `bin1`과 `bin2`는 0과 1로만 이루어져 있습니다.
- `bin1`과 `bin2`는 "0"을 제외하고 0으로 시작하지 않습니다.

---

##### 입출력 예

| bin1 | bin2 | result |
| --- | --- | --- |
| "10" | "11" | "101" |
| "1001" | "1111" | "11000" |

---

##### 입출력 예 설명

입출력 예 #1

- 10 + 11 = 101 이므로 "101" 을 return합니다.

입출력 예 #2

- 1001 + 1111 = 11000 이므로 "11000"을 return합니다.
  

def solution(bin1, bin2):

    a = int(bin1,2)

    b = int(bin2,2)

    answer = bin(a+b)

    return answer[2::]

print(solution("10","11"))


문제 : 숨어있는 숫자의 덧셈 (2)

###### 문제 설명

문자열 `my_string`이 매개변수로 주어집니다. `my_string`은 소문자, 대문자, 자연수로만 구성되어있습니다. `my_string`안의 자연수들의 합을 return하도록 solution 함수를 완성해주세요.

---

##### 제한사항

- 1 ≤ `my_string`의 길이 ≤ 1,000
- 1 ≤ `my_string` 안의 자연수 ≤ 1000
- 연속된 수는 하나의 숫자로 간주합니다.
- 000123과 같이 0이 선행하는 경우는 없습니다.
- 문자열에 자연수가 없는 경우 0을 return 해주세요.

---

##### 입출력 예

| my_string | result |
| --- | --- |
| "aAb1B2cC34oOp" | 37  |
| "1a2b3c4d123Z" | 133 |

---

##### 입출력 예 설명

입출력 예 #1

- "aAb1B2cC34oOp"안의 자연수는 1, 2, 34 입니다. 따라서 1 + 2 + 34 = 37 을 return합니다.

입출력 예 #2

- "1a2b3c4d123Z"안의 자연수는 1, 2, 3, 4, 123 입니다. 따라서 1 + 2 + 3 + 4 + 123 = 133 을 return합니다.

def solution(my_string):

    answer = 0

    temp = ''

    for i in my_string:

        if i.isdigit():

            temp += i

        else:

            if temp:

                answer += int(temp)

                temp = ''

    if temp:

        answer += int(temp)

    return answer

print(solution("aAb1B2cC34oOp"))

문제 : 공 던지기

###### 문제 설명

머쓱이는 친구들과 동그랗게 서서 공 던지기 게임을 하고 있습니다. 공은 1번부터 던지며 오른쪽으로 한 명을 건너뛰고 그다음 사람에게만 던질 수 있습니다. 친구들의 번호가 들어있는 정수 배열 `numbers`와 정수 `K`가 주어질 때, `k`번째로 공을 던지는 사람의 번호는 무엇인지 return 하도록 solution 함수를 완성해보세요.

---

##### 제한사항

- 2 < `numbers`의 길이 < 100
- 0 < `k` < 1,000
- `numbers`의 첫 번째와 마지막 번호는 실제로 바로 옆에 있습니다.
- `numbers`는 1부터 시작하며 번호는 순서대로 올라갑니다.

---

##### 입출력 예

| numbers | k   | result |
| --- | --- | --- |
| [1, 2, 3, 4] | 2   | 3   |
| [1, 2, 3, 4, 5, 6] | 5   | 3   |
| [1, 2, 3] | 3   | 2   |

---

##### 입출력 예 설명

입출력 예 #1

- 1번은 첫 번째로 3번에게 공을 던집니다.
- 3번은 두 번째로 1번에게 공을 던집니다.

입출력 예 #2

- 1번은 첫 번째로 3번에게 공을 던집니다.
- 3번은 두 번째로 5번에게 공을 던집니다.
- 5번은 세 번째로 1번에게 공을 던집니다.
- 1번은 네 번째로 3번에게 공을 던집니다.
- 3번은 다섯 번째로 5번에게 공을 던집니다.

입출력 예 #3

- 1번은 첫 번째로 3번에게 공을 던집니다.
- 3번은 두 번째로 2번에게 공을 던집니다.
- 2번은 세 번째로 1번에게 공을 던집니다.

def solution(numbers, k):

    return numbers[2 * (k - 1) % len(numbers)]

print(solution([1, 2, 3, 4, 5, 6],5))

문제: 행렬의 덧셈

###### 문제 설명

행렬의 덧셈은 행과 열의 크기가 같은 두 행렬의 같은 행, 같은 열의 값을 서로 더한 결과가 됩니다. 2개의 행렬 arr1과 arr2를 입력받아, 행렬 덧셈의 결과를 반환하는 함수, solution을 완성해주세요.

##### 제한 조건

- 행렬 arr1, arr2의 행과 열의 길이는 500을 넘지 않습니다.

##### 입출력 예

| arr1 | arr2 | return |
| --- | --- | --- |
| [[1,2],[2,3]] | [[3,4],[5,6]] | [[4,6],[7,9]] |
| [[1],[2]] | [[3],[4]] | [[4],[6]] |

def solution(A,B):

    for i in range(len(A)) :

        for j in range(len(A[0])):

            A[i][j] += B[i][j]

    return A

print(solution([[1,2],[2,3]],[[3,4],[5,6]]))

문제 : 영어가 싫어요

###### 문제 설명

영어가 싫은 머쓱이는 영어로 표기되어있는 숫자를 수로 바꾸려고 합니다. 문자열 `numbers`가 매개변수로 주어질 때, `numbers`를 정수로 바꿔 return 하도록 solution 함수를 완성해 주세요.

---

##### 제한사항

- `numbers`는 소문자로만 구성되어 있습니다.
- `numbers`는 "zero", "one", "two", "three", "four", "five", "six", "seven", "eight", "nine" 들이 공백 없이 조합되어 있습니다.
- 1 ≤ `numbers`의 길이 ≤ 50
- "zero"는 `numbers`의 맨 앞에 올 수 없습니다.

---

##### 입출력 예

| numbers | result |
| --- | --- |
| "onetwothreefourfivesixseveneightnine" | 123456789 |
| "onefourzerosixseven" | 14067 |

---

##### 입출력 예 설명

입출력 예 #1

- "onetwothreefourfivesixseveneightnine"를 숫자로 바꾼 123456789를 return합니다.

입출력 예 #1

- "onefourzerosixseven"를 숫자로 바꾼 14067를 return합니다.

def solution(numbers):

    for num, eng in enumerate(["zero", "one", "two", "three", "four", "five", "six", "seven", "eight", "nine"]):

        numbers = numbers.replace(eng, str(num))

    return int(numbers)

print(solution("onetwothreefourfivesixseveneightnine"))

enumerate([]) -> 0, 첫번째값 1,두번째값 ...

문제 :최대공약수와 최소공배수

###### 문제 설명

두 수를 입력받아 두 수의 최대공약수와 최소공배수를 반환하는 함수, solution을 완성해 보세요. 배열의 맨 앞에 최대공약수, 그다음 최소공배수를 넣어 반환하면 됩니다. 예를 들어 두 수 3, 12의 최대공약수는 3, 최소공배수는 12이므로 solution(3, 12)는 [3, 12]를 반환해야 합니다.

##### 제한 사항

- 두 수는 1이상 1000000이하의 자연수입니다.

##### 입출력 예

| n   | m   | return |
| --- | --- | --- |
| 3   | 12  | [3, 12] |
| 2   | 5   | [1, 10] |

##### 입출력 예 설명

입출력 예 #1  
위의 설명과 같습니다.

입출력 예 #2  
자연수 2와 5의 최대공약수는 1, 최소공배수는 10이므로 [1, 10]을 리턴해야 합니다.

import math

def solution(n, m):

    su1 = math.gcd(n,m)

    su2 = n * m // su1

    return su1, su2

print(solution(3,12))

math 의 최대공약수의 함수는 gcd이고 두 수의 곱을 최대공약수로 나눈게 최소공배수이다.

문제:문자열 계산하기

###### 문제 설명

`my_string`은 "3 + 5"처럼 문자열로 된 수식입니다. 문자열 `my_string`이 매개변수로 주어질 때, 수식을 계산한 값을 return 하는 solution 함수를 완성해주세요.

---

##### 제한사항

- 연산자는 +, -만 존재합니다.
- 문자열의 시작과 끝에는 공백이 없습니다.
- 0으로 시작하는 숫자는 주어지지 않습니다.
- 잘못된 수식은 주어지지 않습니다.
- 5 ≤ `my_string`의 길이 ≤ 100
- `my_string`을 계산한 결과값은 1 이상 100,000 이하입니다.
  - `my_string`의 중간 계산 값은 -100,000 이상 100,000 이하입니다.
  - 계산에 사용하는 숫자는 1 이상 20,000 이하인 자연수입니다.
  - `my_string`에는 연산자가 적어도 하나 포함되어 있습니다.
- return type 은 정수형입니다.
- `my_string`의 숫자와 연산자는 공백 하나로 구분되어 있습니다.

---

##### 입출력 예

| my_string | result |
| --- | --- |
| "3 + 4" | 7   |

---

##### 입출력 예 설명

입출력 예 #1

- 3 + 4 = 7을 return 합니다.

def solution(my_string):
 return eval(my_string)

eval : **eval(expression)**

eval 함수는 한줄로 정리하자면  
매개변수로 받은 expression (=식)을 문자열로 받아서, 실행하는 함수 입니다.

문제 : 구슬을 나누는 경우의 수

###### 문제 설명

머쓱이는 구슬을 친구들에게 나누어주려고 합니다. 구슬은 모두 다르게 생겼습니다. 머쓱이가 갖고 있는 구슬의 개수 `balls`와 친구들에게 나누어 줄 구슬 개수 `share`이 매개변수로 주어질 때, `balls`개의 구슬 중 `share`개의 구슬을 고르는 가능한 모든 경우의 수를 return 하는 solution 함수를 완성해주세요.

---

##### 제한사항

- 1 ≤ `balls` ≤ 30
- 1 ≤ `share` ≤ 30
- 구슬을 고르는 순서는 고려하지 않습니다.
- `share` ≤ `balls`

---

##### 입출력 예

| balls | share | result |
| --- | --- | --- |
| 3   | 2   | 3   |
| 5   | 3   | 10  |

---

##### 입출력 예 설명

입출력 예 #1

- 서로 다른 구슬 3개 중 2개를 고르는 경우의 수는 3입니다. ![스크린샷 20220801 오후 41555png](https://grepp-programmers.s3.ap-northeast-2.amazonaws.com/files/production/668adf7a-38b1-4112-bbc5-4fab429168c9/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-08-01%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%204.15.55.png) 

입출력 예 #2

- 서로 다른 구슬 5개 중 3개를 고르는 경우의 수는 10입니다.

---

##### Hint

- 서로 다른 n개 중 m개를 뽑는 경우의 수 공식은 다음과 같습니다. ![스크린샷 20220801 오후 43753png](https://grepp-programmers.s3.ap-northeast-2.amazonaws.com/files/production/54c8b2b9-f88c-4a09-8956-7560ff7ea918/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-08-01%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%204.37.53.png) 

---

※ 공지 - 2022년 10월 11일 제한 사항 및 테스트케이스가 수정되었습니다.

import math

def solution(balls, share):

return math.comb(balls,share)

math 라이브러리의 comb 함수 : 경우의 수

comb(n,m) n개 중 m의 수
