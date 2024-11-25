# Chapter 1

# 수학

전자기학을 배울 때 가장 중요한 수학적 요소는
수학이다. 우리는 벡터라는 것을 사용하여 전자기적 인력 척력등을 표현 할 것이고, 특정한 위치에서와 전자기적 힘의 관계를 전기장이라는 벡터장(벡터를 출력하는 함수)로 표현할 것이다.

# 벡터

## 벡터의 정의

```math
        \{ \langle a,b,c \rangle = \overrightarrow{v} | a,b,c \in \mathbb{R} \}
```

전자기학에서 쓰는 벡터의 정의는 여러 실수의 나열 이라고 본다.

---

두가지 중요한 특성이 있다.

1. ```math
   \overrightarrow{i}, \overrightarrow{j}, \overrightarrow{k} 를 각각 \langle 1,0,0 \rangle, \langle 0,1,0 \rangle, \langle 0,0,1 \rangle로 정의한다.
   ```
2. ```math
   \overrightarrow{v}가 \langle a,b,c\rangle 라고 할 때 \overrightarrow{v}를 \langle -a,-b,-c \rangle
   ```
   로 정의 한다

## 벡터장
벡터장 이란 
```math
f(x,y,z) = \overrightarrow{v}\ (\overrightarrow{v}는\ 임의의\ 벡터)
일때\ 
\newline
f를\ \overrightarrow{v}의대한\ 벡터장이라고 한다.
```
우리가 늘상 알아왔던 함수는 치역이 복소수였던 함수였다.<br>
벡터장은 벡터공간(임의의 벡터의 집합)을 치역으로 갖는 함수이다.<br>
벡터장을 좌표평면으로 나타네면 좌표마다 벡터가 대응 되는 꼴로 볼수 있고<br>
이것은 임의의 벡터를 넣었을때 그 값이 어떻게 변하는지 예측할 수 있게한다.<br>
벡터와 벡터장의 미묘한 차이가 초보자의 벽이라고 생각한다.<br>
우리는 벡터장의 대한 미분을 배울것이고 벡터와 벡터장의 차이를 아는 것은 중요하다.
## 벡터의 연산

이러한 정의에 입각해 우리는 여러가지 세로운 연산을 정의 할 것이다.

- 두벡터의 덧셈
  ```math
  \overrightarrow{a} + \overrightarrow{b} = \langle a_x + b_x, a_y + b_y, a_z + b_z \rangle
  ```
- 두벡터의 뺄셈

  ```math
  \overrightarrow{a} - \overrightarrow{b} = \overrightarrow{a} + (- \overrightarrow{b})
  ```

- 벡터와 스칼라의 곱셈

  ```math
  k \cdot \overrightarrow{a} = \langle k \cdot a_x, k \cdot a_y, k \cdot a_z \rangle
  ```

- 두 벡터의 내적(dot product)

  ```math
  \overrightarrow{a} \cdot \overrightarrow{b} = a_x \cdot b_x + a_y \cdot b_y + a_z \cdot b_z
  ```

- 두 벡터의 외적(overrightarrowtor product)
  ```math
  \overrightarrow{a} \times \overrightarrow{b} = \langle a_y \cdot b_z - a_z \cdot b_y, a_z \cdot b_x - a_x \cdot b_z, a_x \cdot b_y - a_y \cdot b_x \rangle
  ```
- 두 벡터의 크기

```math
\| \overrightarrow{a} \| = \sqrt{a_x^2 + a_y^2 + a_z^2}
```

# 미분

## 상비분

- 1차원 상미분

  ```math
  1차원\ 함수\ f(x)의 대해서
  ```
  ```math
  df = (\frac {df}{dx})dx
  ```
<br>
위식은 dx만큼 변할때 f가 얼마나 변하는지 나타낸다.

  ***

* 3차원 미분

  ```math
  3차원\ 함수\ f(x,y,z)에\ 대해서
  ```
  ```math
  df = \left( \frac{\partial f}{\partial x} \right) dx + \left( \frac{\partial f}{\partial y} \right) dy + \left( \frac{\partial f}{\partial z} \right) dz
  ```
  ```math
  위식은 dx,dy,dz 만큼
  변할\ 때\ f가\ 얼마나\
  변하는지\ 나타낸다.
  ```
***
  위식의 점곱꼴은 다음과 같다.

```math
  \langle  \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}, \frac{\partial f}{\partial z} \rangle \cdot \langle dx, dy, dz \rangle = \nabla f \cdot d\overrightarrow{r}
  ```
  ```math
  \nabla f ≡  \langle \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}, \frac{\partial f}{\partial z} \rangle
  ```
  ```math
  \nabla = \langle \frac{\partial}{\partial x}, \frac{\partial}{\partial y}, \frac{\partial}{\partial z} \rangle
  ```
## 벡터 미분
1. 기울기
```math
\nabla f = \langle \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}, \frac{\partial f}{\partial z} \rangle
```
2. 발산

```math
\nabla \cdot \overrightarrow{F} = \frac{\partial F_x}{\partial x} + \frac{\partial F_y}{\partial y} + \frac{\partial F_z}{\partial z}
```
벡터장 
3. 회전

```math
\nabla \times \overrightarrow{F} = \left| \begin{matrix} \overrightarrow{i} & \overrightarrow{j} & \overrightarrow{k} \\ \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\ F_x & F_y & F_z \end{matrix} \right|
```
