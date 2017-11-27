> 혹시 수식이 안보이신다면! Github With Mathjax 익스텐션을 설치하세요. [링크](https://chrome.google.com/webstore/detail/github-with-mathjax/ioemnmodlmafdkllaclgeombjnmnbima?utm_source=chrome-ntp-icon). 감사합니다.

# Monte Carlo Tree Search and Its Applications

**SEUNGWOO LEE**

- 서론

몬테카를로 트리 서치 기술은 확률적(Probabilistic) 알고리즘입니다. 경량 랜덤 시뮬레이션을 사용하여 게임 트리를 키워갑니다. 몇가지의 부분에서 몬테 카를로 나무 탐색은 성공을 거두었습니다. 여기에서는 몬테카를로 나무 탐색의 알고리즘에 관하여 알아봅니다.

**키워드**: 몬테 카를로 나무 탐색, 휴리스틱, 인공지능

- 본론

1. 글을 열며(Introduction)

1997년에 Chess 대결에서 인공지능이 인간을 이긴 사례가 있었다. 이 과정에서 브루트 포스 학습 결정트리 알고리즘을 통해서 학습을 할 수 있었다.

여기에서는 몬테 카를로 트리 시뮬레이션에 대하여 발표한다, 앞서 말했던 브루트 포스 결정트리 알고리즘에 비하여 이 몬테 카를로 트리 알고리즘은 **랜덤**으로 시행한 결과를 토대로 트리 상에 표현한 알고리즘이라고 할 수 있다. <sup>[1]</sup>

여기에서는 바둑의 사례를 들어서 설명한다, 바둑은 기계가 인간을 뛰어넘지 못한 것이라고 알려져 있다. 왜냐면 바둑의 경우의 수는 원자의 수보다 많은 2×10<sup>170</sup> 가지라고 알려져 있다 <sup>2</sup> 하지만 이것도 2016년도 말에 이세돌과 딥마인드의 알파고의 대결로 인해서 깨지게 되었다는게 흠이지만 말이다.

(논문 상에는 2009년에 기계가 최초로 인간을 이겼다고 한다. 딥블루의 빅토리처럼 말이다.)

2. 기본 지식(Background)

- 여기에서는 몬테 카를로 나무 탐색의 기본적인 작동 원리(알고리즘)을 설명한다. 몬테 카를로 나무 탐색은 기본적인 몬테 카를로 시뮬레이션에 나무 탐색(Tree Search)알고리즘을 합친 형태라고 볼 수 있다. 이 장에서는 몬테 카를로 트리 탐색의 기본적인 작동 원리를 알아본다.

	1. The Tree Structure

		- 몬테카를로 나무 탐색 알고리즘에서 트리 구조는 각 파라메터의 움직임을 부모와 자식 간의 구조로 나누어서 표시한다. 틱 텍 토 게임에서 게임의 각 단계별 진행 단계가 표시되는 것하고 비슷하다 볼 수 있다. 상황별로 노드가 연결되어 표시된다.

	2. The Four Steps of MCTS

		- 몬테 카를로 나무 탐색 기법은 선택 → 추가 → 시뮬레이션(을 통한 추가) → Back-Propagation 의 순으로 동작한다. 더 자세하게 설명하면 다음과 같다.

		- 선택: 선택 과정에서는 

	3. Upper Confidence Bound

3. 몬테 카를로 나무 탐색을 사용하여 바둑 플레이하기

	1. All Moves First

	2. Rapid Action Value Estimate

	3. Monte Carlo Rapid Action Value Estimate

	4. Go Result

- 결론

-------------

### 각주

1: 몬테 카를로 시뮬레이션과 나무 알고리즘을 합쳐놓은 것이라고 알면 된다. 랜덤화 결정을 통하는 알고리즘이다. ~~괜히 몬테 카를로라는 이름을 따온게 아닌것 같다~~

-------------

본 논문 제목: Monte Carlo Tree Search and Its Applications. Max Magnuson, University of Minnesota, Morris.