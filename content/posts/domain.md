---
title: "서비스 도메인"
date: 2023-10-18T00:00:00+09:00
draft: false
---

이런 이야기를 굳이 남겨야 하나 싶지만, 누군가에게는 몰랐던 이야기가 될 수 있어서 몇 자 남겨둔다.

## 개발할 때 도메인은 충분히 많이

상위 도메인 하나로 모든 개발환경을 사용하는 팀들이 있다. 개발환경을 sub 도메인으로 분리라도 하면 다행인데, uri의 일부 prefix 정도로 구분하는 경우도 있다.  이런 경우 몇 가지 상황이 발생한다.

하나, 각종 브라우저 및 여러 인터넷 관련 도구들은 도메인 정확히는 eTLD - https://developer.mozilla.org/en-US/docs/Glossary/eTLD 혹은 Public Suffix를 기준으로 각종 정책을 적용한다. 대표적인 예는 브라우저의 쿠키다. 모든 개발환경에 도메인을 같이 사용하는 경우 각 환경이 이런 부분에서 서로에게 영향을 주게 된다. 또 각 환경별 도메인의 eTLD level(sub domain의 레벨, example.com = eTLD+1, sub.example.com = eTLD+2)가 달라지는 문제도 있다. 이로 인해 버그가 재현되지 않거나, 불필요한 기능을 추가하거나, 개발환경 때문에 생기는 문제를 버그로 오인할 수 있다.

둘, 개발 환경과 배포 환경 구분이 어렵다. 개발환경이라고 생각하고 실제 서비스 중인 환경에 테스트를 하거나 데이터를 삭제하는 등의 일은 가장 흔한 운영 실수다. 도메인을 분리하고 거기에 맞는 sub domain 정책을 세우면 더 쉽게 문제를 예방할 수 있다. 더불어 개발환경 도메인에 별도의 entity를 입력하고, 사내에서는 별도의 DNS를 사용하면 DNS단위의 접근제어가 가능하고 및 해킹 시도등을 탐지할 수 있다.

개발 환경용 도메인을 구입할 때는 저렴한, 그리고 차이가 크고 예측이 어려운 도메인으로 하는 것이 좋다. 애너그램을 쓰는 것도 좋은 방법이다. facebook.com이라면, cafemock.boo를 테스트도메인으로 사용할 수 있다. 이경우 도메인 길이가 달라서 생기는 문제는 피하고, 디자인 문제나 환경구분 문제가 단순해진다. 

많은 팀들이 여전히 하나의 도메인에 이메일, 회사 홈페이지, 서비스까지 사용한다. 물론 어떤 팀에서는 내부 규정 때문에 도메인 하나 구입하는데 한달, DNS 설정에 또 한달씩 걸리기도 한다. 하지만, 그런 이유가 아니라면 굳이 하나의 도메인을 고집할 이유는 전혀 없다. 요즘 몇몇 도메인은 1년에 1~3달러 정도로 충분히 저렴하다. 서비스, 회사용, 개발환경용 도메인은 분리해서 사용하는 것을 권장한다. 운영 및 domain shortening을 위한 도메인을 몇개 추가하는 것도 좋다.

## .com! .com! .com!!!!!!
서비스 도메인에 .com을 고집하는 시대는 끝났다. 그러나, .com과 다른 도메인이 같은 성능을 보이는 것은 아니다. 맞다. "성능"이 다르다. 여기에는 두가지가 있는데 하나는 속도고 하나는 안정성이다. 속도와 관련된 내용은 https://bunny.net/blog/is-your-fancy-new-domain-hurting-your-performance-gtld-benchmark/ 에 안정성에 대한 내용은 https://hackernoon.com/stop-using-io-domain-names-for-production-traffic-b6aa17eeac20 를 읽어보기 바란다.

물론, TLD name server가 서비스에 영향을 주는 경우는 매우 적다. 그러나, 신규 서비스일수록, 그리고 급하게 DNS를 바꿔야 하거나 몇 백 ms의 지연이 서비스에 치명적일 때 문제는 발생한다. 보이지 않은 도메인이라면 .com을 써라. 많은 문제가 예방되고 사라질 것이다. 또 이렇게 말할 수도 있겠다. .com이 멈춘다면, 세상이 멈춰있을 것이다.