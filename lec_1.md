# 2019-kookmin-lecture
2019 1학기 국민대학교 산업체특강 lec 1 </br>
</br>
-3월 18일 신임 교수 특집 : 박하명 소프트웨어학부 신임 교수님 -
</br>
## 주제: 분산 시스템을 이용하여 대규모 그래프에 존재하는 모든 삼각형 찾아내기</br>
### 1. Introduction
#### - Why Triangle Enumeration?
그래프는 어디에나 있다 친구 관계, 컴퓨터 네트워크 등등</br>
어떻게 그래프 상에서 패턴을 찾아 변칙을 찾아낼 수 있을까? (스팸 메일, DDoS 공격, ..)</br>
-> Triangle Enumeration 그래프에서 삼각형들을 뽑아낼 수 있다!
#### - Why Distributed Systems?
그래프는 거대하다 (ex 페이스북의 경우 1억이상의 유저가 있고 웹페이지의 경우 1조 이상이 존재한다.)</br>
->어떻게 이런 큰 그래프를 다룰 수 있을까? -> Distributed System(분산 시스템)을 사용한다! </br></br>
### 2. Distributed Triangle Enumeration
#### - Single Machine Triangle Enumeration
두개의 이웃한 set간의 상호 관계가 하나의 삼각형을 이룬다.
#### - Basic Distributed Algorithm
multiple machine을 이용하여 삼각형을 찾기!</br>
어떻게 일을 분산시킬 것인가?</br>
-> 랜덤하게 노드들을 색칠한다.
#### - Multi-round Algorithm
하지만 어마어마한 양의 데이터가 있을 경우는?</br>
-> subproblems을 나누어 문제를 푼다
#### - Pre-partitioning Based Algorithm
grouping하는 단계를 생략하기 위해 먼저 그래프를 부분으로 나누는 작업을 한다.
