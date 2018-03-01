# 프로그래머가 되는 법: 커뮤니티 버전
[//]: # (Version:1.0.0)
Robert L. Read와 커뮤니티

Copyright 2002, 2003, 2016 Robert L. Read

본 에세이는 [크리에이티브 커먼즈 저작자표시-동일조건변경허락 4.0 국제 라이선스](http://creativecommons.org/licenses/by-sa/4.0/)에 따라 사용이 허가되었다.

## 서론
좋은 프로그래머가 되는 것은 어렵고도 고상한 일이다. 어떠한 소프트웨어 프로젝트의 공통된 비전을 만들려고 할 때에 가장 힘든 점은 함께 작업하는 동료들과 고객들을 상대하는 것이다. 컴퓨터 프로그램을 작성하는 것은 중요하고 뛰어난 지능과 기술을 필요로 한다. 하지만 이런 것들은 좋은 프로그래머가 소프트웨어 시스템을 만들기 위해 반드시 해야 하는 다른 일들(자신에게 책임이 있는 고객 및 다른 많은 동료 개발자들을 만족시키는 일)에 비교하면 어린아이의 장난이나 마찬가지다. 나는 이 에세이에서, 내가 스물 한 살이었을 때 누군가 나에게 설명해 주기를 바랐던 것들을 가능한 간결하게 정리하고자 한다.

이는 매우 주관적이며, 따라서 이 에세이는 개인적인 의견에 불과하다. 그렇기에 이 에세이의 주제는 프로그래머가 업무 중에 아주 높은 확률로 맞닥뜨릴 수 있는 문제들로 국한되었다. 이 문제들과 그 해결책 중 많은 것들은 사람 간에 발생할 수 있는 너무나 일반적인 것들이어서 이 에세이가 설교처럼 보일 수도 있다. 그럼에도 불구하고 이 에세이가 유용하게 쓰이기를 바란다.

컴퓨터 프로그래밍 자체는 여러 강의를 통해 학습할 수 있다. The Pragmatic Programmer [Prag99], Code Complete [CodeC93], Rapid Development [RDev96], Extreme Programming Explained [XP99] 등의 서적은 컴퓨터 프로그래밍과 좋은 프로그래머가 되는 방법이라는 큰 주제를 가르친다. 폴 그레이엄 [PGSite] 과 에릭 레이먼드 [Hacker] 의 에세이는 반드시 이 에세이를 읽기 전이나 읽는 중에 함께 읽어야 한다. 이 에세이는 앞서 소개한 훌륭한 글들과는 달리 사회 문제를 강조하며, 꼭 필요한 기술들을 포괄적으로 요약한다.

이 에세이에서 "상사"는 당신에게 프로젝트를 배정해 주는 사람을 가리킨다. 또한 "사업", "회사", 그리고 "부족"이라는 단어는 다 같은 뜻으로 사용되었지만, 사업은 돈을 버는 것을, 회사는 현대의 직장을, 그리고 부족은 당신과 자부심을 공유하는 사람들을 의미한다.

우리 부족에 온 것을 환영한다.

## Contents

1. [초심자](1-Beginner)
	- 개인적 기술들
		- [디버깅 배우기](1-Beginner/Personal-Skills/01-Learn-To-Debug.md)
		- [문제 공간을 나누어 디버그하는 방법](1-Beginner/Personal-Skills/02-How-to-Debug-by-Splitting-the-Problem-Space.md)
		- [에러를 제거하는 방법](1-Beginner/Personal-Skills/03-How-to-Remove-an-Error.md)
		- [로그를 사용해 디버그하는 방법](1-Beginner/Personal-Skills/04-How-to-Debug-Using-a-Log.md)
		- [성능 문제를 이해하는 방법](1-Beginner/Personal-Skills/05-How-to-Understand-Performance-Problems.md)
		- [성능 문제를 해결하는 방법](1-Beginner/Personal-Skills/06-How-to-Fix-Performance-Problems.md)
		- [반복문을 최적화하는 방법](1-Beginner/Personal-Skills/07-How-to-Optimize-Loops.md)
		- [입출력 비용을 다루는 방법](1-Beginner/Personal-Skills/08-How-to-Deal-with-IO-Expense.md)
		- [메모리를 관리하는 방법](1-Beginner/Personal-Skills/09-How-to-Manage-Memory.md)
		- [드물게 발생하는 버그를 다루는 방법](1-Beginner/Personal-Skills/10-How-to-Deal-with-Intermittent-Bugs.md)
		- [설계 기술을 배우는 방법](1-Beginner/Personal-Skills/11-How-to-Learn-Design-Skills.md)
		- [실험을 수행하는 방법](1-Beginner/Personal-Skills/12-How-to-Conduct-Experiments.md)
	- 팀을 위한 기술들
		- [예측이 중요한 이유](1-Beginner/Team-Skills/01-Why-Estimation-is-Important.md)
		- [프로그래밍 시간을 예측하는 방법](1-Beginner/Team-Skills/02-How-to-Estimate-Programming-Time.md)
		- [정보를 찾는 방법](1-Beginner/Team-Skills/03-How-to-Find-Out-Information.md)
		- [사람들에게서 정보를 얻어내는 방법](1-Beginner/Team-Skills/04-How-to-Utilize-People-as-Information-Sources.md)
		- [현명하게 문서화하는 방법](1-Beginner/Team-Skills/05-How-to-Document-Wisely.md)
		- [어설픈 코드에서 작업하는 방법](1-Beginner/Team-Skills/06-How-to-Work-with-Poor-Code.md)
		- [버전 관리 시스템을 사용하는 방법](1-Beginner/Team-Skills/07-How-to-Use-Source-Code-Control.md)
		- [유닛 테스트를 수행하는 방법](1-Beginner/Team-Skills/08-How-to-Unit-Test.md)
		- [막힐 때에는 쉬어야 한다](1-Beginner/Team-Skills/09-Take-Breaks-when-Stumped.md)
		- [퇴근할 시간을 알아채는 방법](1-Beginner/Team-Skills/10-How-to-Recognize-When-to-Go-Home.md)
		- [대하기 힘든 사람을 대하는 방법](1-Beginner/Team-Skills/11-How-to-Deal-with-Difficult-People.md)
2. [중급자](2-Intermediate)
	- 개인적 기술들
		- [How to Stay Motivated](2-Intermediate/Personal-Skills/01-How-to-Stay-Motivated.md)
		- [How to be Widely Trusted](2-Intermediate/Personal-Skills/02-How-to-be-Widely-Trusted.md)
		- [How to Tradeoff Time vs. Space](2-Intermediate/Personal-Skills/03-How-to-Tradeoff-Time-vs-Space.md)
		- [How to Stress Test](2-Intermediate/Personal-Skills/04-How-to-Stress-Test.md)
		- [How to Balance Brevity and Abstraction](2-Intermediate/Personal-Skills/05-How-to-Balance-Brevity-and-Abstraction.md)
		- [How to Learn New Skills](2-Intermediate/Personal-Skills/06-How-to-Learn-New-Skills.md)
		- [Learn to Type](2-Intermediate/Personal-Skills/07-Learn-to-Type.md)
		- [How to Do Integration Testing](2-Intermediate/Personal-Skills/08-How-to-Do-Integration-Testing.md)
		- [Communication Languages](2-Intermediate/Personal-Skills/09-Communication-Languages.md)
		- [Heavy Tools](2-Intermediate/Personal-Skills/10-Heavy-Tools.md)
		- [How to analyze data](2-Intermediate/Personal-Skills/11-How-to-analyze-data.md)
	- 팀을 위한 기술들
		- [How to Manage Development Time](2-Intermediate/Team-Skills/01-How-to-Manage-Development-Time.md)
		- [How to Manage Third-Party Software Risks](2-Intermediate/Team-Skills/02-How-to-Manage-Third-Party-Software-Risks.md)
		- [How to Manage Consultants](2-Intermediate/Team-Skills/03-How-to-Manage-Consultants.md)
		- [How to Communicate the Right Amount](2-Intermediate/Team-Skills/04-How-to-Communicate-the-Right-Amount.md)
		- [How to Disagree Honestly and Get Away with It](2-Intermediate/Team-Skills/05-How-to-Disagree-Honestly-and-Get-Away-with-It.md)
	- 판단 기술
		- [How to Tradeoff Quality Against Development Time](2-Intermediate/Judgment/01-How-to-Tradeoff-Quality-Against-Development-Time.md)
		- [How to Manage Software System Dependence](2-Intermediate/Judgment/02-How-to-Manage-Software-System-Dependence.md)
		- [How to Decide if Software is Too Immature](2-Intermediate/Judgment/03-How-to-Decide-if-Software-is-Too-Immature.md)
		- [How to Make a Buy vs. Build Decision](2-Intermediate/Judgment/04-How-to-Make-a-Buy-vs-Build-Decision.md)
		- [How to Grow Professionally](2-Intermediate/Judgment/05-How-to-Grow-Professionally.md)
		- [How to Evaluate Interviewees](2-Intermediate/Judgment/06-How-to-Evaluate-Interviewees.md)
		- [How to Know When to Apply Fancy Computer Science](2-Intermediate/Judgment/07-How-to-Know-When-to-Apply-Fancy-Computer-Science.md)
		- [How to Talk to Non-Engineers](2-Intermediate/Judgment/08-How-to-Talk-to-Non-Engineers.md)
3. [Advanced](3-Advanced)
	- Technological Judgment
		- [How to Tell the Hard From the Impossible](3-Advanced/Technical-Judgment/01-How-to-Tell-the-Hard-From-the-Impossible.md)
		- [How to Utilize Embedded Languages](3-Advanced/Technical-Judgment/02-How-to-Utilize-Embedded-Languages.md)
		- [Choosing Languages](3-Advanced/Technical-Judgment/03-Choosing-Languages.md)
	- Compromising Wisely
		- [How to Fight Schedule Pressure](3-Advanced/Compromising-Wisely/01-How-to-Fight-Schedule-Pressure.md)
		- [How to Understand the User](3-Advanced/Compromising-Wisely/02-How-to-Understand-the-User.md)
		- [How to Get a Promotion](3-Advanced/Compromising-Wisely/03-How-to-Get-a-Promotion.md)
	- Serving Your Team
		- [How to Develop Talent](3-Advanced/Serving-Your-Team/01-How-to-Develop-Talent.md)
		- [How to Choose What to Work On](3-Advanced/Serving-Your-Team/02-How-to-Choose-What-to-Work-On.md)
		- [How to Get the Most From Your Team-mates](3-Advanced/Serving-Your-Team/03-How-to-Get-the-Most-From-Your-Teammates.md)
		- [How to Divide Problems Up](3-Advanced/Serving-Your-Team/04-How-to-Divide-Problems-Up.md)
		- [How to Handle Boring Tasks](3-Advanced/Serving-Your-Team/05-How-to-Handle-Boring-Tasks.md)
		- [How to Gather Support for a Project](3-Advanced/Serving-Your-Team/06-How-to-Gather-Support-for-a-Project.md)
		- [How to Grow a System](3-Advanced/Serving-Your-Team/07-How-to-Grow-a-System.md)
		- [How to Communicate Well](3-Advanced/Serving-Your-Team/08-How-to-Communicate-Well.md)
		- [How to Tell People Things They Don't Want to Hear](3-Advanced/Serving-Your-Team/09-How-to-Tell-People-Things-They-Dont-Want-to-Hear.md)
		- [How to Deal with Managerial Myths](3-Advanced/Serving-Your-Team/10-How-to-Deal-with-Managerial-Myths.md)
		- [How to Deal with Organizational Chaos](3-Advanced/Serving-Your-Team/11-How-to-Deal-with-Organizational-Chaos.md)
4. [Glossary](GLOSSARY.md)
5. [Appendix A - Bibliography/Websiteography](5-Bibliography.md)
6. [Appendix B - History (As of January 2016)](6-History.md)
6. [Appendix C - Contributions (As of January 2016)](7-Contributions.md)


<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">프로그래머가 되는 법: 커뮤니티 버전</span>은 <span xmlns:cc="http://creativecommons.org/ns#" property="cc:attributionName">Robert L. Read와 커뮤니티</span>에 의해 작성되었으며, <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">크리에이티브 커먼즈 저작자표시-동일조건변경허락 4.0 국제 라이선스</a>에 따라 사용이 허가되었다.
