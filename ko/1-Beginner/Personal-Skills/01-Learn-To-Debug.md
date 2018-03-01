# 디버깅 배우기
[//]: # (Version:1.0.0)
디버깅은 프로그래머가 되기 위한 초석이다. "디버그(debug)"라는 동사의 첫 번째 의미는 "오류를 제거하는 것"이지만, 실제로 중요한 의미는 프로그램을 실제로 실행하여 그 과정을 들여다보고 검사하는 것이다. 효과적으로 디버깅을 할 줄 모르는 프로그래머는 장님과도 같다.

이상주의자들은 설계, 분석, 또는 복잡도 이론 등이 디버깅보다 더 중요하다고 생각하지만, 이들은 현장의 프로그래머가 아니다. 현장의 프로그래머들은 이상적인 세계에 살고 있지 않다. 설령 완벽한 프로그래머가 존재한다고 해도, 그는 대형 소프트웨어 회사, GNU와 같은 단체, 그리고 그의 동료들이 작성한 코드들에 둘러싸여 있으며 반드시 이것들을 가지고 작업해야만 한다. 이 코드들의 상당수는 완벽하지 않으며 불완전하게 문서화되어 있다. 이 코드들의 실행 과정을 꿰뚫어 볼 투시력이 없다면 아주 사소한 문제조차 해결하지 못하고 나가떨어질 것이다. 많은 경우 이러한 투시력은 실험을 통해서만 얻어지는데, 이를 디버깅이라고 한다.

디버깅은 프로그램의 실행에 대한 것이지, 프로그램 그 자체에 대한 것이 아니다. 만약 대형 소프트웨어 회사에서 프로그램을 구매했다면, 그 프로그램의 내부는 대게 볼 수가 없다. 그럼에도 프로그램이 문서화된 내용대로 작동하지 않거나 (시스템이 프로그램과의 충돌로 인해 멈추는 경우가 가장 일반적이고 심각한 예이다), 프로그램에 문서화되지 않은 내용이 있는 경우는 여전히 존재할 것이다. 더 일반적인 예로, 오류가 발생해 코드를 살펴보아도 왜 오류가 발생했는 지 알 수 없는 경우도 존재한다. 당연하게도 이는 코드를 작성할 때 잘못된 가정을 했거나 미처 예상하지 못했던 상태가 발생한다는 것을 의미한다. 때로는 소스 코드를 뚫어지게 바라보는 것 만으로도 문제를 찾아내는 마법같은 일이 있을 수도 있다. 그렇지 않을 때에는, 디버깅을 해야만 한다.

프로그램의 실행 과정을 꿰뚫어 볼 투시력을 갖기 위해서는 그 프로그램을 실행해 보고 그에 대한 무언가를 관찰해야만 한다. 때때로 이 무언가는 스크린에 표시되는 어떤 것이거나, 두 이벤트 사이의 시간 차와 같이 눈으로 볼 수 있는 것들이다. 하지만 다른 많은 경우에는 눈으로 볼 수 없는 것을 관찰해야 한다. 코드 안에 있는 특정 변수의 상태, 코드에서 현재 실행되고 있는 위치, 또는 어떠한 검증 조건(assertion)이 복잡한 자료구조에서 지켜지고 있는지의 여부 등은 눈으로 볼 수 없다. 이렇게 볼 수 없는 것들은 볼 수 있도록 해야 한다.

실행되고 있는 프로그램의 '내부'를 보는 방법들은 일반적으로 다음과 같이 분류할 수 있다.

- 디버깅 툴을 사용하는 것
- 프린트 줄 넣기(printlining): 프로그램에 임시로 정보를 출력하는 코드를 추가하는 것
- 로그 기록 남기기(logging): 로그 형태로 프로그램의 실행 과정을 남기는 통로를 만드는 것

디버깅 툴을 사용하는 것은 오류 없이 안정적으로 사용 가능하다면 매우 좋은 방법이지만, 프린트 줄을 넣는 방법과 로그 기록을 남기는 방법이 훨씬 더 중요하다. 디버깅 툴은 개발 언어보다 뒤떨어질 때가 많아서, 언젠가는 사용할 수 없게 될 수도 있다. 게다가 디버깅 툴을 사용하는 것으로 프로그램의 실행 과정이 미묘하게 바뀔 수 있기 때문에 항상 유효한 방법은 아니다.

Debugging tools are wonderful when they are stable and available, but printlining and logging are even more important. Debugging tools often lag behind language development, so at any point in time they may not be available. In addition, because the debugging tool may subtly change the way the program executes it may not always be practical. Finally, there are some kinds of debugging, such as checking an assertion against a large data structure, that require writing code and changing the execution of the program. It is good to know how to use debugging tools when they are stable, but it is critical to be able to employ the other two methods.

Some beginners fear debugging when it requires modifying code. This is understandable - it is a little like exploratory surgery. But you have to learn to poke at the code and make it jump; you have to learn to experiment on it and understand that nothing that you temporarily do to it will make it worse. If you feel this fear, seek out a mentor - we lose a lot of good programmers at the delicate onset of their learning to this fear.

Next [How to Debug by Splitting the Problem Space](02-How-to-Debug-by-Splitting-the-Problem-Space.md)
