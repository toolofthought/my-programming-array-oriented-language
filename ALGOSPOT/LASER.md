# 링크 #
https://algospot.com/judge/problem/read/LASER
# 분석 #
동일 직선 상의 점이라는 것을 어떻게 확인할 수 있을까요?
## 그려보기 ##

	] data =: > ". L: 0 cutopen clipread ''
	require 'plot'
	'dot;pensize 5;aspect 1' plot ;/ |: data

![](http://i.imgur.com/UJk4QdE.png)

그림에서 6개의 점이 동일 직선상에 있는 것을 확인할 수 있습니다.
## 알고리즘 생각하기 ##
어떤 한 점을 원점으로 삼아 다른 점들과 벡터를 구한다고 해볼까요? 아니면 dialation이라는 것을 활용해서 어떤 임의의 상수 k값을 구하면 어떨까요?

# 구현 #
## J ##
