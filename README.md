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
