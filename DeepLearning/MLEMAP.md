# Random Variable의 Parameter를 Estimation 하는 방법 - MLE와 MAP
Maximum Likelihood Estimation와 Maximum a Posteriori Estimation은 기초적인 통계분석, 회귀분석등 다양한 통계분석에서 사용됩니다.

## 1. Maximum Likelihood Estimation (MLE)
### 오직 주어진 데이터 또는 Observation을 토대로 Parameter Estimation 하는 방법
- F<sub>0</sub> : Unkown Probability Density Function 가 있다고 가정
- X = (x<sub>1</sub>, x<sub>2</sub>, x<sub>3</sub>, ... , x<sub>n</sub>)를 그 확률로 생성된 Observation
- Density function이 θ 로 parameterize된 어떤 분포의 family라고 가정
- 그러면 Observation X가 주어진다면, θ의 값만 알수 있다면 f(X|θ)를 계산 가능

<b> Likelihood 정의 : L(θ;  x<sub>1</sub>, x<sub>2</sub>, x<sub>3</sub>, ... , x<sub>n</sub>) = L(θ; X) = f(X|θ) = f(x<sub>1</sub>, x<sub>2</sub>, x<sub>3</sub>, ... , x<sub>n</sub>|θ) = f(x<sub>1</sub>|θ)f(x<sub>2</sub>|θ). . .f(x<sub>2</sub>|θ) = ∏<sup>n</sup><sub>i=1</sub>f(x<sub>i</sub>|θ)</b>
-  포아송 분포일 경우
>  f(x|λ) = \\( x(t)=\frac{-b\pm \sqrt{{b}^{2}-4ac}}{2a} \\)  

<b> Maximum Likelihood Estimation (MLE) - θ^ : Likelihood를 최대로 만드는 값을 선택 <br /> </b>
![alt text](image/MLE.PNG)

### Example of Maximum Likelihood Estimation
바닥에 떨어진 머리카락의 길이(x)을 보고 남녀인지 성별(y)을 판단하는 문제 

남자를 y<sub>1</sub>이고 여자는 y<sub>2</sub>로 정했을 때 
- P(x|y<sub>1</sub>) = 남자에게서 주어진 머리카락의 길이가 나올 확률 
- P(x|y<sub>2</sub>) = 여자에게서 주어진 머리카락의 길이가 나올 확률 

## 2. Maximum a Posteriori Estimation (MAP)
### 주어진 데이터에 대해 최대확률을 갖는 θ 를 찾는 방법


### Example of Maximum a Posteriori Estimation
바닥에 떨어진 머리카락의 길이(x)을 보고 남녀인지 성별(y)을 판단하는 문제 

남자를 y<sub>1</sub>이고 여자는 y<sub>2</sub>로 정했을 때 
P(y<sub>1</sub>|x) = 머리카락 x가 주어졌을 때, 남자일 확률
P(y<sub>2</sub>|x) = 머리카락 x가 주어졌을 때, 여자일 확률

SanghyukChun's Blog - http://sanghyukchun.github.io/58/ 참고