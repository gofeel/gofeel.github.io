---
title: "일정과 계획"
date: 2021-01-21T04:29:00+09:00
draft: false
---

일정 계획을 짜고 실행하는 것은 쉽다. 구체적인 계획을 짜고 주기[^1]에 따라서 확인하며 실행하면 된다. 마치 어린 시절 방학 시간표를 짜듯이. 그런데 보통은 실패한다. 방학 계획표처럼. 아래의 이야기들은 덜 실패하기 위한 혹은 마지막은 실패하지 않는 법에 대한 이야기이다.

### A. 실행 가능한 일정계획을 짠다

계획은 현재 수행 가능해야 한다. 계획에는 기간뿐 아니라 구성원의 역량이나 비용 등이 포함되어야 한다. 구성원의 역량을 넘어선 무리한 일정[^3]이나 미래에 합류할 사람[^2]처럼 확정되지 않은 자원이나 혹은 막 들어온 인턴처럼 일감 단위의 업무를 진행할 수 없는 인원을 계획의 일부로 포함해서는 안된다.

계획에는 목표와 기간이 있어야 한다.[^10] 계획을 짜는 데 있어 흔한 실수는 추상적이거나 실행할 수 없는 목표를 잡는 것이다. 목표는 객관적인 지표가 있고 지표로 평가되어야 한다. 제품 출시라면 제품이 가져야 할 구체적인 기능들이 명세되어 있어야 하고, 출시일이 설정되어야 한다. 목표가 추상적이면 목표에 다다르지 못해서 너무 초조해 지거나 반대로 일이 너무 늘어져서 아무도 일하지 않는 상태로 빠진다. 비정상이 일상이 된다.

큰 계획은 관리하기 쉬운 단위로 쪼개서 관리한다. 처음부터 세부일정을 한꺼번에 작성하지 않는다. 마일스톤을 주기적으로 설정하고 계획을 주기적으로 수정한다. 계획을 계속 수정하면서, 일정대로 진행이 되고 있는지를 꾸준히 확인한다. 이슈트레커를 사용한다면 한 일감은 일정 단위로 쪼개고 이를 묶어서 관리한다. 팀에 알맞는 일정 단위를 찾는 것도 중요하다. 회의를 나쁘다라고만 말하지 말고, 알맞은 주기를 찾아 일정을 같이 확인해야 한다.

비밀의 상자는 없어야 한다. 계획이 망쳐지는 흔히 상황은 해결될 것으로 예상했던 문제가 해결할 방법이 없는 경우이다. 예를 들면, 제품의 일부가 특허로 묶여 있거나, 최적화가 불가능해서 성능에 치명적인 문제가 있거나 하는 부분들이다. 물리적으로 논리적으로 불가능한 경우도 있다. 새로운 제품을 만드는 경우라면 계획을 수립하기 전에 세부적인 구현을 일정에 포함하지 않더라도 우회가 불가능한 부분들에 대해서 개념 증명(proof-of-concept)이 끝나 있어야 한다. 이런 개념 증명은 계획 단위를 벗어나더라도 우선적으로 수행되어야 한다. 제품이 카피캣인 경우의 몇 안 되는 장점은 개념 증명을 대신할 수 있다는 것이다. 만일, 비밀의 상자가 있다면 가장 우선 정리되어야 하고 계획 수립은 그 이후로 미루어져야 한다.

### B. 모든 계획은 실패한다 - 그래서, 늘 실패 가능해야 한다

계획은 실패 가능해야 한다. 작은 계획들이 계속 실패하고 수정되는 것이 당연해야 한다. 그러나 실패의 흔적이 남고 그 흔적들이 모여 도미노처럼 모든 계획을 무너트리지 않도록 하는 것이 중요하다. 실패를 시스템의 일부로 만들어야 한다. 일정과 일정 사이의 여유는 가장 기본이고, 대체 투입 가능한 자원이나, 추가 투입 가능한 자본이나, 계획의 수정까지 모든 계획의 수행에는 실패 시의 대안이 있어야 한다.

낙관하지 않는다. 외부요인에 의한 실패는 예측하기 쉽지 않다. 특정 게임의 성공으로 인한 클라우드 서비스의 자원 포화[^5], 특정 보안 문제로 인한 클라우드의 전체 시스템 성능 하락[^4] 같은 것들을 예측하는 것은 불가능하다. 태풍으로 인한 하드디스크 가격의 급등[^6]이나 암호화폐의 부흥으로 인한 그래픽 카드의 품절현상[^7]도 생길수 있다. 모두 있었던 일이다.

[Bus Factor]({{< ref "/posts/bus_factor" >}})는 2 혹은 그 이상으로 한다. 개개인에 의지하는 시스템은 무조건 붕괴한다. 하나의 작업에 대해서 대체 가능하고 대체하는 인원도 자신의 일을 대체할 수 있도록 그물처럼 연결되어야 한다. 팀 단위 업무처리나 코드리뷰와 이슈트레커 같은 시스템을 잘 사용한다면 쉽게 이러한 시스템을 구축할 수 있다.

작업자는 실패를 선언할 수 있어야 한다. 즉, 작업이 주워질 때는 작업을 언제 멈출 것인지에 대한 기준이 제공되어야 하고, 모두가 따라야 한다.[^8] 많은 조직들이 실패를 개인의 능력 부족으로 탓하는 문화를 가지고 있다. 그러나 노력을 한다고 해서 문제가 해결되는 것이 아니다. 이미 실패가 예상된 상황에서 판단을 보류하거나 외면하는 것은 일을 악화시킬 뿐이다. 진행 불가능한 상황에서는 멈추도록 그리고 이를 주변에 알리도록 해야 한다. 작업의 명세가 잘못된 경우에는 수정하고, 작업이 불가능하다면, 다른 작업자가 작업하거나, 작업을 취소할 수 있어야 한다. 이를 위해서는 개인의 업무에 대한 기록과 평가에 대한 기준과 시스템이 필요하다. 더불어 실패의 원인을 분석하고 원인을 해결하는 구조 역시 필요하다. 이런 시스템이 없으면, 누군가는 일을 끌어안기만 하고, 누군가는 문제를 해결하느니라 고생하고 저평가받는 일과 누군가는 비난으로 인해서 문제를 숨기는 일이 반복된다.

미리미리 점검한다. 다시 말하면 다시 말하면 미리 실패시킨다. 초보는 자신이 [모르는 것을 모르기]({{< ref "/posts/unknown" >}})에 상황을 알리지 않는다. 어떤 이들은 결과물이나 목표를 오독한다. 그리고 어떤 이들은 목표를 자의대로 수정하거나 문제를 은폐한다. 시간이 무작정 늘어나는 것을 방지하기 위해서는 Issue tracker를 기본으로 지표들을 주기적으로 점검하고 지속적인 대화를 통해 상황을 판단해야 한다. small talk을 이용한 over communication을 활용할 수 있다.

### C. 망했어요

모든 계획은 복구 불가능할 정도로 완전히 실패할 수도 있다. 완전한 실패 이후 팀은 무엇을 할 것인가에 대한 계획도 필요하다. 누군가 책임을 지거나 조직을 해체하거나 결과물의 일부를 이용해서 다른 일을 계획하거나 하는 다양한 선택지들이 있다. 회고, 평가, 갑작스러운 중단에 대한 보상이 이뤄져야 한다.

실패를 선언하려면, 계획은 주기적으로 평가되어야 한다. 그런데, 언제 계획은 실패했다고 말할 수 있을까? 단순히 목표에 다다르지 못한 계획은 실패한 계획인가? 제품 개발이나 개선이 계획의 목표라면 계획은 가설 검증을 위한 것이다. 가설은 보통 고객의 문제를 제품으로 해결할 수 있을 것이라는 것이고, 가설 검증은 가설을 한정된 자원으로 주어진 기간 동안에 검증할 수 있을 것이라는 기대를 기반으로 한다. 즉, 제품을 만든다는 것은 문제, 가설, 자원, 기간이라는 특징점 들을 갖는다. 그러므로 계획의 평가는 단순히 진행도가 아니라 목표를 가설 검증이라는 기준으로 가설이 검증되고 있는지 가설을 둘러싼 환경이 유지되는지를 기준으로 평가해야 한다. 그래야 계획을 정확하게 평가할 수 있다.

### 다시 쓰는 A. 모든 계획은 목표부터

모든 계획은 가설 검증 단 하나를 향해야 한다. 다시 말하면, [사소함에 사로잡히지 않아야 한다.]({{< ref "/posts/over_the_triviality" >}})  수많은 기법들, 시스템, 최신의 기술이나 도구들을 사용하는 데 있어서 기준은 언제나 가설 검증을 빠르게 하는데 도움이 되는지 여부이다. 언제나 기준이 분명하면 선택은 쉽다. 단 두 명이 일하는 상황이라면 수많은 문서를 남기는 것보다 몇 줄의 낙서가 효과적이다. 각종 시스템과 기법의 왕도에 대해서 말하기 앞서서 문제에 집중해야 한다.

계획의 각 항목(일감)에는 검증 가능한 목표, 마감일, 이유, 우선순위가 정리되어 있어야 한다. 목표와 질을 따지지 않는 흔히 말하는 ASAP업무는 사실상 하지 않아도 되는 일과 동의어이다. ASAP가 아니라 우선순위와 일정으로 말하고 마감을 지키지 못할 때의 대안에 대해서 말해야 한다. 각 작업별로 이유를 기록해야 우선순위를 설정하고 가설 검증에 도움이 되지 않을 때 폐기할 수 있다. 우선순위대로 일해야, 실패 시 우선순위가 낮은 일들을 안 하고도 실패할 수 있다.

계획의 크기는 가설과 가설을 둘러싼 환경을 기준으로 해야 한다. 가설을 둘러싼 환경이 유동적이라면 짧게, 환경 변화가 느리다면 더 크게 계획을 짤 수 있다. 일정과 관련해 사람들은 흔히 일반론을 말한다. 주기적 배포 및 출시 등이 대표적이다. 그러나, 모두가 풀고자 하는 문제가 다른 이상 계획의 크기와 관련된 일반론은 불가능하다. 주변 상황에 맞추어 알맞은 주기와 기법을 찾아야 한다.

### 마무리

이 모든 이야기는 계획을 잘 짜야한다는 이야기를 하는 것이 아니다. 회사가 푸는 문제가 명확하지 않으면 어떤 계획도 쓸모없다는 이야기다. 다시 말하면, 회사의 정체성 혹은 정의가 분명하지 않으면 아무리 제품을 잘 설계하고 계획을 아무리 잘 만들어도 실패한다. 처음 한두 번은 그냥 흘러가지만, 계획의 실패가 반복되면 아무리 둔한 사람이라도 이유 모를 불편함을 느끼기 마련이다. 패배감이 가득한 회사에서 개개인이 개인의 이익을 움직이기 시작하면 무기력함이 전염병처럼 퍼지고 회사는 끝도 없이 무너진다. 생각을 하나로 모으는 것이 제품을 만드는 팀(개발, 디자인, 기획, 등등)을 돕는 가장 쉬운 방법이다.

또, 아무리 목적이 분명해도 실행하는 이의 능력과 의지에 따라서 엉망이 될 수도 있다. 이런저런 단어들을 따라 외연을 만드는 것은 쉽다.[^12] 하지만 외연이 제품을 만들고 문제를 해결해 주는 것은 아니다. 외연의 의미에 대해서 고민하고, 실제 문제 해결에 도움이 되는 구조를 구성해야 하고, 기회가 왔을 때 잡도록 지속적으로 내부 역량을 키워야 한다.

A는 모두를 위해서 B는 계획을 관리하는 사람을 위해서 C는 의사결정권자를 위한 이야기이다. 수많은 말과 숫자로 자기를 만족시키고 서로를 속이고 남을 탓하기 전에 계속 질문해야 한다. 그래서 지금 만들고 있는 것이 무엇인가? 왜 만드는가? 모두가 다 목표에 대해서 이해하고 동의하고 있는가?

계획이 없는 시간이 무조건 무의미한 것은 아니다. 오히려 일상적인 일들을 수행하면서 기술 부채를 줄이고 내부 역량을 올리는 시간은 꼭 필요하다. 단, 계획과 계획 사이 비운 시간이 의미 있으려면, 팀이 잠시 공전하더라도 나중에는 목표를 향해 앞으로 갈 것이라는 강한 믿음이 있어야 한다.

[^1]: 주간회의, 월말회의 등등
[^2]: 예전 회사에서는 일정을 짤때 해야할 일을 나열하고 담당자를 정한 다음, 넘친 일에 대해서 담당자를 TBD(to be determined) 적어두고 탁병두씨라고 불렀다. 몇 주후 서로를 병두씨라고 부른건 덤이다.
[^3]: 크런치 타임의 상시화
[^4]: Meltdown & Spectre
[^5]: 한국에서 PUBG가 성공했을때 생긴 일이다.
[^6]: 2011 태국 태풍
[^7]: 2017년 & 2021년
[^8]: 일부만 룰을 무시하면 어떻게 되는가. 대표적으로는 이런 [사례](https://ko.wikipedia.org/wiki/대한항공_801편_추락_사고)가 있다.
[^10]: 기간을 정하는 한가지 팁은 직관적으로 예상되는 기간의 1.5~2배를 해서 계획을 짜는 것이다. 꼼꼼하게 일정을 짜는데 들어가는 노력과 예상하지 못한 상황에 일정이 늘어났을때 일정을 조율하고 조정하는 것과 대비 미리 여유를 두고 일하는 것이 유리한 경우가 많다. 특히, 외부팀과 일할때 그렇다. 대신, 중간 일정 확인은 모두 첫 기준대로 하고, 추가되는 기간은 일을 반복하면서 조정해야 한다. 여유가 있으면 편하게 일을 잘하는 것도 여유만큼 늘어지는 것도 사람이다. 그리고 한번 어겨진 마감일은 두번도 세번도 그리고 무한대로 늘어난다.
[^12]: 언론 인터뷰, 최신 기술/도구 도입, 컨퍼런스에 발표, 기술 블로그/뉴스레터 같은 홍보와 이런저런 기준의 성장률,테스트 커버리지, 이슈 마감률 같은 숫자들
