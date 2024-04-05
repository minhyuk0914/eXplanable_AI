# eXplanable_AI : AI의 결정 과정을 인간이 이해할 수 있는 형태로 설명하는 기술
XAI(설명가능한 인공지능)
> * **whitebox model** : Linear Regression, Decision Tree, K-Nearest Neighbors...와 같은 설명력이 있는, 이해 가능한 알고리즘 모델
> * **blackbox model** : Deep Neural Network, Random Forest, XGBoost...와 같은 복잡한 모델.     
Decision Tree기반의 RandomForest, XGBoost와 같은 모델은 기존 Decision Tree와는 다르게 설명력이 없다. 이유는, 1개의 Tree를 사용하는 것이 아닌, 100개보다 더 많은 Tree가 모여서 만드는 모델이기에, **blackbox model**에 속한다.

![image](https://github.com/minhyuk0914/eXplanable_AI/assets/90814001/3741b0f7-df3a-407a-a5bb-300220796159)

## XAI 기술 종류
#### 1. Feature importance Analysis(특성 중요도 분석): 모델의 예측에 있어서 가장 큰 영향을 미치는 특성(변수) 추출
#### 2. Decision Trees(결정 트리) : 규칙 기반의 접근 방식을 사용하여 예측을 생성
#### 3. Local Interpretable Model-agnostic Explanations, LIME : **blackbox model**과 같이 복잡한 모델의 예측을 로컬로 근사하는 간단한 모델을 생성하여, 특정 예측에 대한 모델의 작동방식을 설명
#### 4. Shapely Additive exPlanations, SHAP : SHAP는 게임 이론에서, 영감을 받은 방법으로, 각 입력 변수가 모델의 예측에 기여하는 정도를 정량화하여, 모델의 전반적인 작동 원리를 이해하는데 도움
