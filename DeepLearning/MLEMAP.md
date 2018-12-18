# Random Variable의 Parameter를 Estimation 하는 방법 - MLE와 MAP
## Maximum Likelihood Estimation (MLE)
### 오직 주어진 데이터 또는 Observation을 토대로 Parameter Estimation 하는 방법
- Unkown Probability Density Function F<sub>0</sub>가 있다고 가정
- X = (x<sub>1</sub>, x<sub>2</sub>, x<sub>3</sub>, ... , x<sub>n</sub>)를 그 확률로 생성된 Observation
- Density function이 θ 로 parameterize된 어떤 분포의 family라고 가정
- 그러면 Observation X가 주어진다면, θ의 값만 알수 있다면 f(X|θ)를 계산 가능
- <b> Likelihood 정의 : L(θ;  x<sub>1</sub>, x<sub>2</sub>, x<sub>3</sub>, ... , x<sub>n</sub>) = L(θ; X) = f(X|θ) = f(x<sub>1</sub>, x<sub>2</sub>, x<sub>3</sub>, ... , x<sub>n</sub>|θ) </b>
-<b> Maximum Likelihood Estimation (MLE) - θ^ : Likelihood를 최대로 만드는 값을 선택 <br /> </b>
![alt text](image/MLE.PNG)

MLE - Ex) <br />
바닥에 떨어진 머리카락의 길이(x)을 보고 남녀인지 성별(y)을 판단하는 문제 <br />
남자를 y<sub>1</sub>이고 여자는 y<sub>2</sub>로 정했을 때 <br />
P(x|y<sub>1</sub>) = 남자에게서 주어진 머리카락의 길이가 나올 확률 <br />
P(x|y<sub>2</sub>) = 여자에게서 주어진 머리카락의 길이가 나올 확률 <br />

## Maximum a Posteriori Estimation (MAP)

SanghyukChun's Blog - http://sanghyukchun.github.io/58/ 참고