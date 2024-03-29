---
title: Software Engineering - The Soft Parts 번역
date: "2023-04-17T01:55:00.000Z"
description: "Software Engineering - The Soft Parts 번역"
tags: ["translate"]
---

원문 - [https://addyosmani.com/blog/software-engineering-soft-parts/](https://addyosmani.com/blog/software-engineering-soft-parts/)  

**게시를 허락해주신 addy osmani에게 감사드립니다.**

오늘은 구글 크롬에서 10년간의 시간을 보내며 배운 소프트웨어 엔지니어링 "소프트 스킬" 중 일부를 공유하려고 합니다. 저는 현재 이곳에서 고급 기술 관리자로 일하고 있습니다. 10주년을 맞이하면서, 제가 배운 몇 가지 교훈에 대해 되새겨보고자 합니다. 이 글이 여러분의 경력에 도움이 되기를 바랍니다.

**좋은 엔지니어가 되는 것은 경험을 쌓는 것입니다. 작은 프로젝트일지라도 모든 프로젝트는 새로운 기술과 도구를 습득할 수 있는 기회입니다. 한 프로젝트에서 배운 기술을 다른 프로젝트에서 배운 도구와 결합하여 문제를 해결할 수 있을 때 더 큰 가치를 얻을 수 있습니다.**

이 글을 시작하기 전에, 저는 별 것 아니고 현명하지도 않고 독창적이지 않다는 말로 이 글을 시작하겠습니다. 각자의 상황과 경험에 따라 다를 수 있습니다. YMMV :)

<details>
  <summary>목차</summary>

  - 전문성 Mastery
  - 비판적 사고와 합리적인 논거 공식화 hink critically and formulate well-reasoned arguments
  - 강력한 기반 구축 **Building a strong base**
  - 이전 가능한 기술 **Transferable skills**
  - 효율성 **Efficiency**
  - 더 나은 의사 결정 **Better decision-making**
  - 사용자에 집중하면 나머지는 따라옵니다 **Focus on the User and the rest will follow**
  - 최고의 소프트웨어는 사용자와 공감하는 엔지니어에 의해 만들어집니다. **The best software is built by engineers who have empathy for their users.**
  - 기술 업그레이드 **Upgrading your skills**
  - 이달의 유행이 아닌 사용 사례에 적합한 것 선택하기 **Choose what's right for your use case and not the flavor of the month.**
  - 새로운 프로젝트를 활용해 새로운 기술을 배워보세요. **Take advantage of new projects to learn new tech.**
  - 호기심을 갖고 배움을 멈추지 마세요 **Be curious and never stop learning**
  - 배운 것에 대해 글을 작성하세요. 주제를 더 잘 이해하도록 도와줍니다. 때로는 다른 사람에게 설명을 시도할 때만 지식의 격차가 명확해지기도 합니다. 내가 쓴 글을 아무도 읽지 않아도 괜찮습니다. 혼자서 하는 것만으로도 많은 것을 얻을 수 있습니다. **Write about what you learn. It pushes you to understand topics better. Sometimes the gaps in your knowledge only become clear when you try explaining things to others. It's OK if no one reads what you write. You get a lot out of just doing it for you.**
  - 리더가 모르는 것을 인정하는 것은 큰 힘이 됩니다. **It's powerful for leaders to admit when they don't know something.**
  - 리더는 실수를 인정합니다. **Leaders also admit when they make mistakes.**
  - 소유자가 아닌 관리자가 되세요. **Be a caretaker, rather than an owner.**
  - 기술의 깊이와 넓이 **Depth and breadth of skills**
  - 경험하는 것이 곧 배우는 것입니다. **To experience is to learn**
  - **Generic vs Specific code**
  - 딥 모듈 **Deep modules**
  - 프로젝트 유지보수에서 학습하기 Learning on a maintenance project
  - 그린 필드 프로젝트에서 학습하기 **Learning on a green-field project**
  - 완료의 정의 **Definition of done**
  - 단계적 출시 **Phased roll-outs**
  - 체계적인 디버깅 **Systematic debugging**
  - 설계 문서의 중요성 **Importance of design docs**
  - 문서화 프로세스 **Documentation process**
  - 맞춤형 커뮤니케이션 **Customized communication**
  - 친절하고 배려하기 **Being kind and considerate**
  - 아니오의 힘 **The power of NO**
  - 수용과 존중 **Acceptance and respect**
  - 정보 공유 **Information sharing**
  - 유연성 **Flexibility**
  - 기록 유지 **Maintaining a record**
  - 선의 **Good faith**
  - 연공서열과 전략적 사고 **Seniority and strategic thinking**
  - 솔선수범 **Leading by example**
  - 효율성을 확장하세요 **Scale your effectiveness.**
  - 가면증후군 **Imposter syndrome**
  - 다른 사람 멘토링 **Mentoring others**
  - 조직 전반의 멘토링 **Organization-wide mentoring**
  - 멘티의 역할 **Mentee's role**
  - 신뢰 구축 **Building Trust**
  - 비즈니스 모델 이해**Understanding the business model**
  - 영향력 증대**Increase your impact**
  - 시간 관리 **Time management**  
</details>


# 새로운 것 배우기 Learning new things

다음 지침들은 주니어 또는 중견 개발자가 소프트웨어 엔지니어링 패러다임의 표준 프로세스를 따르고 새로운 모범 사례를 발견하면서 앞으로 나아가고, 변화하는 기술에 대처하고, 복잡한 시스템을 구축하는 데 도움이 될 것입니다. 가능하면 첫 번째 원칙을 적용하세요. 문제를 더 작은 조각으로 분해하는 법을 배우는 것은 인생에서 가장 중요한 기술 중 하나입니다.

### 전문성 Mastery

**기술 전문성은 근무 시간 대비 제공된 가치의 비율이 높다는 것을 의미합니다.**

즉, 가치를 더하는 작업을 식별하고 팀이 그 방향으로 에너지를 집중하도록 도와주는 능력을 의미합니다. 또한 팀과 회사에 가치를 제공하지 않는 작업을 피하는 방법을 알고 있다는 의미이기도 합니다. 최고의 엔지니어는 팀 전체를 그다지 유용하지 않은 작업에서 벗어나도록 유도할 수도 있습니다. 가장 중요한 일에 집중하세요.

"시간을 최대한 활용하고 있는지 어떻게 알 수 있나요?" 라는 질문을 자주 받습니다. 바쁘다고 '느끼기' 위해 시간을 채울 수 있는 작업이 거의 항상 있을 것입니다. 여기서 진짜 중요한 것은 올바른 작업에 집중하는 것입니다. 산을 옮기고 싶다면 그 움직임이 작더라도 바늘을 움직이는 작업에 집중하세요.

스스로에게 물어볼 수 있는 몇 가지 질문이 있습니다.

- 내 목표는 무엇인가요? 내가 집중하고 있는 작업이 그 목표와 일치하나요?
- 다른 방법이나 더 잘할 수 있는 방법이 있을까요?

스스로에게 이런 질문을 던지는 것만으로도 큰 힘이 될 수 있습니다.

### 비판적 사고와 합리적인 논거 공식화 hink critically and formulate well-reasoned arguments

**비판적 사고는 신중한 결정을 내리기 위해 인지적 능력을 사용하여 독립적으로 사고하는 능력입니다. 이 능력을 키우면 사고의 명확성을 개선할 수 있습니다.**

엔지니어로서 우리는 때때로 문제를 즉시 해결하려고 서두르는 경향이 있습니다. 그래야 진전이 있는 것처럼 느껴지거나 이해관계자들에게 잘 대응하는 것처럼 보이기 때문입니다. 그러나 원인과 결과를 충분히 고려하지 않을 경우 위험을 초래할 수 있습니다. 다시 말해, 비판적 사고는 의도적으로 생각하고 스스로 결론을 내리는 것입니다. 이러한 목적 지향적 사고는 원인과 결과를 염두에 두지 않아 발생하는 미래의 문제를 방지하는 근본적인 문제에 집중할 수 있도록 도와줍니다.

일반적으로, 나는 비판적 사고를 기반으로 다음과 같은 질문을 하곤 합니다:

- 올바른 문제를 해결하고 있는지 어떻게 알 수 있나요?
- 올바른 방식으로 문제를 해결하고 있는지 어떻게 알 수 있나요? (즉, 문제에 대한 이해와 제약 조건을 고려하여 정확성과 효율성을 균형있게 고려하는 것)
- 문제의 원인을 모르는 상황에서 어떻게 근본 원인을 찾을 수 있나요?
- 핵심 질문을 더 자세히 분석할 수 있는 작은 질문으로 세분화하려면 어떻게 해야 할까요?
- 하나 이상의 가설을 세우고 나면 이를 평가하기 위해 작업을 어떻게 구성할 수 있나요?
- 제약 조건(시간 압박)이 있는 경우 질문에 대한 분석의 엄밀성을 과도하게 손상하지 않으면서도 어떤 지름길을 택할 수 있을까요?
- 증거가 결론을 충분히 뒷받침하나요?
- 작업이 완료되었는지 어떻게 알 수 있을까요? 솔루션이 "충분하다"고 판단되는 시점은 언제인가요?
- 모든 이해관계자에게 솔루션을 명확하고 논리적으로 전달하려면 어떻게 해야 할까요?

이러한 질문이 도움이 되는 경우가 많았습니다. 때로는 문제의 증상에 대해 대응하다가 다른 증상이 발생할 수 있습니다. 나중에 더 많은 문제를 야기하는 솔루션을 빠르게 출시할 수도 있습니다. 비판적 사고의 렌즈를 통해 가정에 이의를 제기하고, 위험/이익을 자세히 살펴보고, 모순되는 증거를 찾고, 신뢰성을 평가하고, 더 많은 데이터를 찾아서 옳은 일을 하고 있다는 확신을 가질 수 있습니다.

예를 들어, 엔지니어들이 흔히 저지르는 실수 중 하나는 상관관계가 인과관계를 의미한다고 가정하는 것입니다 (즉, 두 가지가 상관관계가 있다고 해서 반드시 하나가 다른 하나를 유발한다는 의미는 아닙니다). 비판적 사고를 하는 사람이라면 이런 가정에 반발하며 왜 그런 가정을 사실이라고 믿느냐고 반문할 수 있습니다.

비판적 사고자

- 신중한 질문을 제기하여 명확하고 정확하게 공식화합니다.
- 관련 정보를 수집하고 평가하여 질문에 대한 답을 어떻게 찾을 수 있는지 검증합니다.
- 관련 기준과 표준에 따라 테스트하여 합리적인 결론과 솔루션에 도달합니다.
- 대안적인 사고 체계 내에서 열린 마음으로 사고하고 필요에 따라 가정, 의미 및 실제 결과를 인식하고 평가합니다.
- 복잡한 문제를 해결하기 위해 다른 사람들과 효과적으로 소통합니다.

참고: 비판적 사고는 '소프트 스킬'과 '하드 스킬'의 두 가지 측면을 모두 가지고 있으므로 이 글에 포함시켰습니다.

### 강력한 기반 구축 **Building a strong base**

**기초 원리를 익히고 반복적으로 적용하여 새로운 기술 습득**

기초 원리를 배우는 장기적인 가치는 이전이 가능하다는 점입니다. 단기적으로는 더 나은 의사 결정을 내릴 수 있도록 도와주고, 코드를 더 효율적으로 만들 수 있습니다.

### 이전 가능한 기술 **Transferable skills**

**이전 가능한 기술이란 프로젝트마다 가져갈 수 있는 기술을 말합니다. 이러한 이전 가능한 기술을 기초와 관련하여 이야기해 보겠습니다.**

기초 원리는 모든 소프트웨어 엔지니어링 경력의 기반입니다. 기초 원리에는 매크로와 마이크로의 두 가지 레이어가 있습니다. 매크로 레이어는 소프트웨어 엔지니어링의 핵심이며 마이크로 레이어는 구현(예: 기술 스택, 라이브러리, 프레임워크 등)입니다.

거시적 수준에서는 언어에 관계없이 대체로 적용할 수 있는 프로그래밍 개념을 배웁니다. 구문은 다를 수 있지만 핵심 아이디어는 여전히 동일합니다. 여기에는 데이터 구조(배열, 객체, 모듈, 해시), 알고리즘(검색, 정렬), 아키텍처(디자인 패턴, 상태 관리), 심지어 성능 최적화(예: 빠른 평가와 느린 평가, 메모이제이션, 캐싱, 지연 로딩 등) 등이 포함될 수 있습니다. 이러한 개념은 자주 사용하게 될 것이므로 거꾸로 알고 있으면 많은 도움이 될 수 있습니다.

마이크로 레벨에서는, 이러한 개념의 구현 방법을 배우게 됩니다. 이는 사용하는 언어(Javascript, Python, Ruby 등), 사용하는 프레임워크(React, Angular, Vue 등), 사용하는 백엔드(Django, Rails 등),  사용하는 기술 스택(Google App Engine, Google Cloud Platform 등)과 같은 것을 포함할 수 있습니다. 이러한 세부 정보는 전문성을 갖추는 데 유용할 수 있지만, 항상 이전 가능한 것은 아닙니다.

**기초 원리를 익히면 기초 원리를 무시하고 성장할 수 있는 스킬셋과 도구를 얻을 수 있습니다.**

하지만 현실적으로 경력 초기에 모든 것을 배울 시간이 있는 사람은 아무도 없습니다. 기초 원리에 지나치게 집착하지 말고 실제 업무에 필요한 애플리케이션을 구축하는 데 필요한 것을 배워야 할 시점이 있습니다. 바로 이때 **“실습을 통한 학습”** 접근 방식이 필요합니다.

### 효율성 **Efficiency**

기초 원리를 잘 이해하면 더 효율적인 코드를 작성하는 데 도움이 됩니다. 이는 시간 복잡도(코드 실행에 걸리는 시간), 메모리 사용량, 성능과 유지 관리 간의 트레이드 오프와 같은 개념을 포함합니다. 이러한 아이디어는 대규모의 애플리케이션을 구축할 때 유용한 트레이드 오프를 할 수 있게 해줍니다. 최신 애플리케이션에서는 속도가 중요하며 최종 사용자 경험에 미치는 영향이 눈에 띄게 나타납니다.

### 더 나은 의사 결정 **Better decision-making**

**매크로, 마이크로 기초 원리를 잘 이해하면 더 나은 결정을 내릴 수 있습니다.**

얻은 지식을 활용하여 프로젝트의 목표와 제약 조건에 따라 사용해야 할 기술과 피해야 할 기술에 대해 더 나은 결정을 내릴 수 있습니다. 이렇게 하면 작업에 잘못된 기술이나 잘못된 도구를 선택하는 함정을 피할 수 있습니다.

> "사용하지 말아야 할 때를 이해하기 전까지는 도구를 숙달한 것이 아닙니다." - 
@kelseyhightower
> 

소프트웨어 엔지니어링은 핵심 언어, 구현, 인프라, 도구, 사람과 같은 다양한 레이어에 대한 생각이 포함됩니다. 이러한 레이어에 대한 표면적인 이해만으로도 빠르게 구축할 수 있습니다. 그러나 기본 원리( O(n) 시간 복잡도를 포함한 )를 알고 있으면, 시간이 지남에 따라 언어와 프레임워크 환경이 변화할 때 더 멀리 갈 수 있습니다.

Related reading:

- [The value of fundamentals in Software Engineering](https://skorks.com/2010/04/on-the-value-of-fundamentals-in-software-development/)
- [Why learning the fundamentals matters](https://medium.com/@felixthedev/why-learning-the-programming-fundamentals-matters-67e5dbbdee8f)
- [Learn the fundamentals of a good developer mindset](https://www.freecodecamp.org/news/learn-the-fundamentals-of-a-good-developer-mindset-in-15-minutes-81321ab8a682/)

### 사용자에 집중하면 나머지는 따라옵니다 **Focus on the User and the rest will follow**

**사용자 경험에서 시작하여 필요한 기술로 거꾸로 작업하세요**

스티브 잡스는 "고객 경험에서 시작하여 기술로 거꾸로 작업해야 합니다. 기술부터 시작한 다음 어디에 판매할지 고민해서는 안 됩니다." 라는 유명한 말을 남겼습니다.

엔지니어로서 특정 솔루션(인기, 개발자 경험, 개인 선호도 등)을 사용하려는 마음에서 시작하여 이를 합리화하는 방법을 찾는것은 너무 쉽기 때문에 이 말이 마음에 와 닿았습니다. 대신 우리는 누구를 위해 만들고 있는지, 그들이 갖고 있는 문제가 무엇인지, 현재 사용 가능한 옵션이 어떻게 부족한지에 초점을 맞춰야 합니다.

훌륭한 사용자 경험은 고객과 기술이라는 두 가지 관점을 결합하여 만들어집니다. 고객이 원하는 것을 보여주고 고객의 의견에 귀를 기울여야 합니다. 물론 이 문제에는 엄청나게 미묘한 차이가 있습니다. 모바일 하드웨어에서 훌륭한 경험을 제공할 수 있는 엔지니어링 선택은 무엇입니까? 어떤 선택이 엔지니어링 속도, 규모, 채용에 영향을 미칩니까? 궁극적으로 고객에게 먼저 집중한 다음, 주어진 제약 조건 내에서 고객의 요구 사항을 충족할 수 있는 방법을 탐색함는 것이 좋습니다.

### 최고의 소프트웨어는 사용자와 공감하는 엔지니어에 의해 만들어집니다. **The best software is built by engineers who have empathy for their users.**

비즈니스 성공은 고객 만족에 달려 있으며, 소프트웨어의 경우 사용자 경험으로 이어지는 경우가 많습니다. 최종 사용자(End User)가 제품이나 서비스를 어떻게 경험하는지 이해해야 합니다. 귀사의 솔루션이 사용자의 효율적인 업무 수행 능력을 방해하지 않는지 확인해야 합니다. 최종 사용자와 직접 소통할 수 있는 위치에 있다면 그들의 요구 사항과 문제점을 더 잘 이해하려고 노력하세요.

### 기술 업그레이드 **Upgrading your skills**

### 이달의 유행이 아닌 사용 사례에 적합한 것 선택하기 **Choose what's right for your use case and not the flavor of the month.**

과대 광고가 난무하는 기술보다는 ‘지루한’ 기술(이미 시도하고 검증된 기술)을 사용하는 것도 괜찮습니다. 언어, 프레임워크, 라이브러리는 종종 진화합니다. 훌륭한 최종 제품을 제공하는데 도움이 되는 것을 선택하세요. 새 프로젝트를 시작할 때는 ‘지루한’ 기술(하지만 잘 알려진 기술)로 시작하세요. 그런 다음 의도적으로 그 중에서 문제에 가장 적합한 도구를 선택하도록 하세요.

배우거나 사용할 새로운 기술을 선택할 때 지루하고 뉴스에 나오지 않은 것을 선택하는것을 두려워 하지 마세요. 언어, 프레임워크, 라이브러리, 도구 등 기술에 관한 고립 공포감(FOMO)은 생산적이지 않을 수 있습니다. 무엇을 사용해야 할 지 아는것도 중요하지만, 가장 중요한 목표는 훌륭한 최종 결과물을 제공하는 것입니다. 솔루션에 가치를 더할 수 없다면 새롭고 반짝이는 기술을 쫓아다니지 마세요. 동시에, 충분히 이야기되고 있지 않다고 해서 무언가를 피하지 마세요.

### 새로운 프로젝트를 활용해 새로운 기술을 배워보세요. **Take advantage of new projects to learn new tech.**

개인 프로젝트와 해커톤 프로젝트는 동시에 새로운 기술을 배울 수 있는 좋은 기회가 될 수 있습니다. 많은 결정이 내려진 기존 코드베이스에서 작업하는 것과는 달리 완전히 새로운 것을 시작할 기회는 많지 않습니다. 이러한 프로젝트는 새로운 기술을 연구하고, 소규모로 장단점을 평가하고, 미래에 유용하게 활용할 수 있는 직접적인 지식을 쌓을 수 있는 위험 부담이 적은 방법이 될 수 있습니다.

### 호기심을 갖고 배움을 멈추지 마세요 **Be curious and never stop learning**

### 배운 것에 대해 글을 작성하세요. 주제를 더 잘 이해하도록 도와줍니다. 때로는 다른 사람에게 설명을 시도할 때만 지식의 격차가 명확해지기도 합니다. 내가 쓴 글을 아무도 읽지 않아도 괜찮습니다. 혼자서 하는 것만으로도 많은 것을 얻을 수 있습니다. **Write about what you learn. It pushes you to understand topics better. Sometimes the gaps in your knowledge only become clear when you try explaining things to others. It's OK if no one reads what you write. You get a lot out of just doing it for you.**

학습은 지속적인 과정이어야 합니다. 특정 기술에 대해 모든 것을 알고 있다고 주장하는 사람들은 전문가가 아닌 경우가 많습니다. 진정한 전문가는 해당 기술에 능숙하지만 항상 학습, 개선의 여지가 있음을 알고 있습니다. 호기심은 학습의 원동력입니다. 새로운 프레임워크에 대해 궁금한 것이 있다면 구글에서 검색하고, 문서를 읽고, 튜토리얼을 시도하고, 소스를 읽어보세요! 학습은 교실에서만 이루어질 필요는 없습니다. 학습은 언제 어디서나 일어날 수 있습니다. 매일 30분정도 시간을 내어 교과서의 한 장을 읽거나, 기술 팟캐스트를 듣거나, 개발 블로그를 읽거나, 새로운 프로그래밍 언어를 배워보세요.

### 리더가 모르는 것을 인정하는 것은 큰 힘이 됩니다. **It's powerful for leaders to admit when they don't know something.**

이러한 자신감을 가지면 시니어 엔지니어가 모든 것을 알아야 한다는 기대치가 낮아집니다. 모든 답을 알고 있을 필요는 없지만, 자신이 인간임을 인정하고 팀과 함께 문제를 해결하는 방법을 찾기 위해 노력하는 것이 중요합니다.

### 리더는 실수를 인정합니다. **Leaders also admit when they make mistakes.**

팀원들에게 겸손한 자세로 실수를 처리하는 방법과 배우고 개선하려는 열정을 가르치는 것이 중요합니다. 현실은 완벽하지 않으므로 팀에게 완벽하지 않다는 것을 보여주고 이에 대비하도록 하는 것도 괜찮습니다.

### 소유자가 아닌 관리자가 되세요. **Be a caretaker, rather than an owner.**

오픈 소스 프로젝트의 초기 단계에서는 소유자처럼 생각하는 것이 일반적입니다. 가치를 증명하고, 기능을 개발하고, 이슈에 답하고, 옹호하는 일을 직접 하는 경우가 많습니다. 이것은 무언가를 채택하는 데는 유용할 수 있지만, 나중에 인력이 변경되거나 자신의 시간이 제한될 때 프로젝트를 확장하는데는 최선의 방법이 아닐 수 있습니다.

초기 크런치 이후에 역할을 발전시키는 또 다른 방법은 소유자가 아닌 관리자가 되는 것입니다. 관리자는 스스로 확장하는데 집중할 수 있습니다. 이는 설계 문서, 코드 코멘트, 문서화된 베스트 프랙티스를 통해 다른 관리자, 기여자, 커뮤니티와 가능한 많은 지식을 공유함으로써 이루어질 수 있습니다.  또한 더 이상 참여하지 않을 때 올바른 결정을 내릴 수 있도록 충분한 컨텍스트를 갖춘 리뷰어 풀을 늘리는 데 도움이 됩니다.

이는 프로젝트가 수년 후에도 지속 가능한 상태로 유지되기 위해 필요합니다.

### 기술의 깊이와 넓이 **Depth and breadth of skills**

**모든 분야의 전문가가 되거나 한 분야의 달인이 되는 것이 자신에게 적합한지 생각해 보세요.**

여러분이 습득할 수 있는 가장 큰 기술 중 하나는 배우는 방법을 배우는 것입니다. 특정 프로그래밍 언어나 프레임워크에 대해 깊이 파고드는 것보다 우선순위를 높여야 합니다. 호기심을 유지하는 것이 도움이 됩니다. 이러한 경험을 샇고 나면 스페셜리스트가 되는 것을 목표로 해야 할지, 제너럴리스트가 되는 것을 목표로 해야 할지 고민할 수 있습니다.

저는 개인적으로 [T자형 엔지니어](https://itrevolution.com/articles/why-the-full-stack-engineer-is-problematic/)라는 개념을 좋아합니다. 이들은 한 가지 또는 소수의 기술(T의 세로 막대)에 대한 깊은 전문가이지만 제품을 만들고 실행하는 데 필요한 다른 많은 기술(가로 막대)에 대해 기본적인 이해가 있는 엔지니어 입니다. 일부 팀은 팀원을 다양한 전문 분야로 순환 배치하여 보다 많은 T자형 팀원을 구성하는 것을 선호합니다.

중대형 규모의 팀에서는 한 분야에 특화된 기술을 가지고 있으면서 필요한 경우 다른 팀원들의 역할을 대신할 수 있는 기술, 다재다능함, 협업에 대한 적성을 갖춘 사람을 배치하는 것이 효과적이라는 것을 알게 되었습니다.

### 경험하는 것이 곧 배우는 것입니다. **To experience is to learn**

**새로운 언어를 배울 때는 직접 경험해 볼 수 있는 실체적인 것을 만드는데 집중하세요.**

새로운 언어를 배우는 경우, 좋은 개발자가 되기 위해 모든 구문이나 문서를 외울 필요는 없습니다. 문제를 해결하는 방법을 아는 것이 더 중요합니다. 관련 코드를 많이 작성하거나 기존 코드에서 학습하여 경험을 쌓으세요. 그 결과 해당 언어로 효율적인 코드를 작성하는 데 도움이 될 것입니다. [여기](https://www.csc.gov.sg/articles/how-to-build-good-software)에서 언급했듯이 “소프트웨어의 주요 가치는 생산된 코드가 아니라 사람들이 축적한 지식” 입니다. 그러나 새로운 기술을 실험할 때는 프로덕션 환경에서 실험하지 마세요.

# 기술적 복잡성 **Technical Complexity**

### **Generic vs Specific code**

**당면한 문제에 대한 코드를 구체적으로 작성하되, 약간 일반적일 수 있는 부분을 찾아내세요.**

우리는 종종 가능한 한 제네릭한 코딩을 시도하다가 결국 문제 해결에 도움이 되지 않는 효과적인 코드 수프를 만들고는 합니다. 대신, 이 문제를 위해 특별히 빌드하되 조금 더 일반적으로 만들 수 있는 위치를 찾으려고 노력하면, 나중에 생각치 못한 것으로 다시 리팩토링해야 했을 시간을 없앨 수 있습니다.

설계 복잡성에 대해 일반적으로 논의되는 몇 가지 원칙이 있습니다. 익스트림 프로그래밍 세계에서 보면 다음과 같습니다.

- [YAGNI(You aren't gonna need it)](https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it) - 프로그래머는 꼭 필요할 때 까지 기능을 추가하지 말아야 합니다.
- [가능한 가장 간단한 일을 하세요.](https://ronjeffries.com/xprog/articles/practices/pracsimplest/) - 미래에 대한 계획보다는 빠른 발전을 이루기 위해.

이 두 가지 원칙은 모두 [오버 엔지니어링](https://en.wikipedia.org/wiki/Overengineering)을 방지하는 것을 목표로 합니다. 그러나 이러한 원칙은 잘 통합되지 않는 여러 가지 간단한 솔루션을 만드는데 남용될 수 있습니다.

스펙트럼의 다른 끝에는 일반화를 통해 가능한 한 코드의 중복 구조를 줄이는 것을 목표로 하는 [추상화 원칙](https://en.wikipedia.org/wiki/Abstraction_principle_(computer_programming))이 있습니다. 저는 코드를 약간 일반화하여 극단적인 추상화와 극단적인 단순화 사이의 중간 지점을 선호합니다. [AHA](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself#AHA)(성급한 추상화 피하기) 원칙도 비슷한 생각을 장려합니다.

### 딥 모듈 **Deep modules**

**다른 개발자를 위해 복잡한 문제를 해결하되, 명확한 인터페이스를 통해 기능을 노출하는 코드를 작성하세요.**

여러분이 API 디자이너나 개발자라면 다른 개발자를 위해 복잡한 기능을 단순화하는 인터페이스를 제공하는것이 여러분의 책임입니다. 인터페이스가 너무 이해하기 어렵고 인터페이스를 사용하는 프로그래머에게 비용을 부과하면 목적이 무의미해집니다. 이 아이디어는 [Deep Modules](https://medium.com/@nathan.fooo/4-notes-modules-should-be-deep-ba5671c4288c#:%7E:text=greatest%20benefit%20and%20the%20least%20cost) 개념에 반영되어 있습니다. “최고의 모듈은 가장 큰 이점과 가장 적은 비용을 가진 모듈입니다. 모듈이 제공하는 이점은 기능이고 비용은 인터페이스 입니다.”

인터페이스가 단순한것은 바람직하지만, 복잡한 문제를 해결하기 위해 복잡한 코드가 필요한 경우도 있습니다. (보편적인 룰은 아니지만 종종 그렇습니다). 이러한 복잡성은 코드에 임베드하는 것이 좋습니다. 복잡한 기능을 추상화하면 최종 사용자 혹은 인터페이스 사용자에게 제공되는 가치가 더 높아집니다.

일부 기능을 포함하는 여러 가시적 함수와 클래스가 있는 API는, 더 적은 공개 함수/클래스를 사용하여 구현된 동일한 기능을 가진 다른 API와 비교해 더 복잡하고 검색하기 어렵습니다. 새로운 함수와 클래스는 메인터넌스 프로그래머와 라이브러리 사용자의 인터페이스 비용을 증가시킵니다.

### 프로젝트 유지보수에서 학습하기 Learning on a maintenance project

**오래된 시스템의 레거시 코드에서 작업할 때 유지해야 하는 코드와 제거해야 하는 코드의 차이를 이해해야 합니다.**

모든 시니어 엔지니어는 유지해야 하는 코드와 제거해야 하는 코드의 차이점을 이해하기 위해 노력해야 합니다.

장기적으로 운영되는 대규모 푸로덕션 시스템에는 나쁜 코드나 더 이상 유지해야 할 이유가 없는 코드가 있을 수 있습니다. 어떤 코드가 존재하는 이유(나쁜 이유는 좋은 이유든)를 이해하는 것은 건전한 일입니다. 나쁜 코드는 제거하고 좋은 코드는 유지하세요.

저는 많은 회사에서 일하면서 사람들이 레거시 코드가 건드릴 수 없거나 타당한 이유 때문에 그대로 설계되어 시간의 모래 속에 사라졌다고 생각하는 경우를 많이 봤습니다. 이는 변화에 대한 두려움으로 이어져 취약한 기반에 추상화만 계속 추가하는 결과를 초래할 수 있습니다.

소프트웨어 산업은 많은 프로젝트에서 오래된 시스템이나 레거시 시트템의 유지보수 및 마이그레이션을 처리하는 단계에 이르렀습니다. 이러한 팀에 소속되어 있더라도 좌절하지 마세요. 오래된 코드를 살펴봄으로써 얻을 수 있는 도메인별 지식이 많이 있습니다. 오래된 코드/밸리데이션이 프로덕션에 존재하는 데에는 타당한 이유가 있을 수 있지만, 모든 코드가 여전히 관련성이 있다고 가정하지 않는 것이 좋습니다.

일부 소프트웨어 엔지니어는 버그가 발생할까 봐 프로덕션 환경에서 작동하는 코드를 건드리는 것을 경계합니다. 그래서 새로운 유즈 케이스를 위해 조건을 추가하고 일부 코드를 반복합니다. 이러한 해결 방법은 당장은 시간을 절약할 수 있지만 시간이 지남에 따라 유지 보수의 악몽이 됩니다. 기존 코드가 축복받았거나 전혀 틀리지 않았다고 가정하지 마세요. 이전에 간과했던 확장성이나 효율성 측면에서 해결해야 할 부분이 있을 수 있습니다.

### 그린 필드 프로젝트에서 학습하기 **Learning on a green-field project**

<aside>
💡 그린 필드 프로젝트 : 다른 프로젝트와의 인터그레이션에 대한 우려 없이 완전히 새로운 환경을 위한 시스템을 개발하는 프로젝트

</aside>

**실험하고, 혁신하고, 빠르게 실패하고, 문제 해결 능력을 향상하세요.**

시스템을 처음부터 구축해야 할 때는 학습 여정이 완전히 달라집니다. 기능을 반복적으로 프로토타이핑 하거나 구현하면서 무엇이 효과가 있고 무엇이 효과가 없는지 배우게 됩니다. 애자일 방법론과 [빠른 실패 원칙](https://asbresources.com/pros-and-cons-of-failing-fast-with-agile/)은 더 적은 리소스로 더 일찍 아이디어를 검증하는데 도움이 됩니다. 그것들은 여러분이 복잡한 문제를 세분화하고 정복할 수 있게 해줍니다.

### 완료의 정의 **Definition of done**

**완료(Done)를 정의하면 필요한 노력을 예측하고, 개발 계획을 세우고, 나중에 불필요한 수정을 피하는데 도움이 되어 시간을 절약할 수 있습니다.**

복잡성을 다룰 때 유용한 또 다른 애자일 원칙은 [완료의 정의](https://www.productplan.com/learn/agile-definition-of-done/)에 동의하는 것입니다. 여기에는 사용자 요구 사항과 승인 기준을 충족하는 것 외에도 코드 검토, 테스트, 문서화 등과 같은 다른 조건이 포함될 수 있습니다.

### 단계적 출시 **Phased roll-outs**

**하나의 대규모 릴리스는 위험도가 낮고 이해하기 쉬운 일련의 롤아웃으로 나눌 수 있습니다.**

대규모 프로덕션 시스템의 릴리스를 계획할 때 롤아웃 계획은 아키텍처와 코드 만큼이나 중요합니다. 반복적인 개발을 통한 단계적 릴리스는 대규모 변경으로 인한 위험을 더 잘 관리할 수 있습니다. 또한 개발 및 테스트 전략과 함께 릴리스 전략을 만들어 복잡한 릴리스에 대한 End to End 계획을 세울 수도 있습니다.

### 체계적인 디버깅 **Systematic debugging**

**디버깅 할 때는 모든 테스트 조건을 충족할 수 있도록 문제를 체계적이고 엄격하게 해결하도록 노력해야 합니다.**

항상 오류 메시지와 스택 트레이스를 읽어보세요. 거기에는 문제를 격리하여 해결하는데 도움이 되는 귀중한 정보가 있을 수 있습니다. 놀랍게도 많은 엔지니어가 디버깅 지원을 찾기 전에 에러 메시지가 제공하는 인사이트를 무시합니다. 코드를 조금 수정하고 계속 다시 실행하면 문제가 더 빨리 해결될 것이라고 생각하지 말고, 컴퓨터가 무엇이 잘못되었고 무엇이 맞는지 알려주고 있다고 가정하세요. 예외를 발생시키는 솔루션을 작성하면서 예외를 주의 깊게 읽지 않는다면 시간 낭비일 수 있습니다. 종종 오류, 예외 메시지는 실제로 무엇이 잘못되었는지에 대한 큰 힌트인 경우가 많습니다.

# 설계 문서 **Design Docs**

### 설계 문서의 중요성 **Importance of design docs**

**설계 문서는 나중에 생각할 것이 아니라 소프트웨어 엔지니어링 프로세스의 필수적인 부분이어야 합니다.**

설계 문서는 시스템의 일부이며 인터페이스가 필요한 동료, 다른 팀으로부터 합의를 얻는데 도움이 되는 유비쿼터스 도구입니다. 다른 사람의 피드백을 통해 부족한 부분을 파악하고 설계를 개선할 수 있습니다. 또한 설계 문서는 미래에 팀에 합류할 엔지니어에게도 귀중한 도움이 됩니다. 문제 공간과 솔루션 설계 시 고려해야하는 트레이드 오프와 대안들을 이해하는데 도움이 됩니다. 설계 문서는 문서 기록의 일부분으로 설계 및 기여에 관련된 모든 참여자를 캡처할 수 있는 공간을 제공합니다. 이는 다른 사람들이 특정 결정을 주도한 사람과 추가 설명을 위해 누구에게 연락해야 하는지 이해하는데 도움이 됩니다.

### 문서화 프로세스 **Documentation process**

**설계 문서에 대한 검토를 조율하고 설계가 발전함에 따라 원본 문서와 비교하여 모든 관련 제약 조건이 해결되고 있는지 확인합니다.**

한 사람이 설계를 문서화할 수 있지만 실제 설계 프로세스는 일련의 화이트보드 미팅, 무작위 대면 토론, 슬랙 스레드, 이메일/전화 논의를 통해 이루어집니다. 종이에 적은 후에야 모순되는 약속을 파악하고 논의했던 여러 부분이 서로 맞는지 확인할 수 있습니다. 초안을 작성한 후에는 검토를 조정하여 모든 관련 당사자가 참여할 수 있도록 합니다. 그러나 도중에 변경된 사항으로 인해 구현된 설계가 문서화된 내용과 일치하지 않을 수 있습니다.

# 커뮤니케이션 **Communication**

**겸손하고 명확하게 커뮤니케이션하며 다른 사람을 존중하세요. 친절하게 대하는 데는 비용이 들지 않지만 그 영향은 값을 매길 수 없습니다. 어떤 사람들은 좋은 소통에는 에너지와 사려 깊음이 필요하다고 말할 수 있습니다. 연민을 위한 더 많은 에너지를 쏟아야 합니다.**

커뮤니케이션은 효과적이고 생산적이며 효율적인 소프트웨어 엔지니어가 되기 위해 필요한 소프트 스킬 혹은 대인 관계 기술의 중요한 부분입니다. 잘못된 커뮤니케이션은 잘못된 기능, 호환되지 않는 코드, 공격적인 팀 역학 관계로 이어질 수 있습니다. 커뮤니케이션은 사람들이 요구 사항을 더 잘 이해하고 문제가 에스컬레이션되는 것을 방지하는 데 도움이 될 수 있습니다.

세상은 소프트웨어 엔지니어를 하루 종일 코드만 작성하는 사람이라고 생각할 수 있습니다. 그러나 우리가 만든 제품이 다른 사람들에게 도움이 되려면 팀 내 다른 사람들, 비즈니스, 사용자의 기대와 동기화하도록 노력해야 합니다. 그렇기 때문에 협업과 커뮤니케이션은 우리 업무의 중요한 축입니다.

주니어 개발자는 주로 다른 팀원, 테스트 엔지니어, 팀 리더와 소통하며 아이디어를 공유하고 문제 해결을 위한 대안을 논의합니다. 경력이 쌓여감에 따라 업무를 효과적으로 수행하기 위해 필요한 커뮤니케이션의 양이 늘어납니다. 이메일, 미팅, 공개 강연의 수가 증가합니다. 비즈니스 리더, 매니저, 이해관계자, 팀원들과 소통해야 합니다. 업무가 전문화될수록 다른 사람들이 여러분을 쉽게 이해하지 못할 위험도 커집니다.

### 맞춤형 커뮤니케이션 **Customized communication**

**청중에게 적절한 언어, 개념, 세부 사항을 사용하세요.**

문제나 상황에 대한 이해 수준이 어떻든, 우리가 다른 사람들과 논의할 때는 상대방이 관련 내용을 빠르게 파악할 수 있도록 말을 조정해야 합니다.

- 비즈니스 담당자와 대화 할 때는 여러분이 하고 있는 일이 비즈니스에 미치는 영향에 대해 얘기 하세요. 지나치게 전문적인 용어는 사용하지 마세요.
- 엔지니어링 경영진과 대화 할 때는 기술적 영향이나 도전 과제를 전달하세요.
- 의사 결정권자와 대화 할 때는 옵션의 작동 방식에 대한 세부 사항이 아니라, 사용 가능한 옵션과 그 의미, 위험에 대해 설명하세요.
- 상태 업데이트를 제공할 때는 그 밖에 어떤 일이 발생했는지, 업데이트가 프로젝트 목표와 어떻게 연관있는지 알고 있어야 합니다.

이메일을 작성하거나 더 많은 청중에게 프레젠테이션 할 때도 동일한 원칙이 적용됩니다. 메시지를 받는 사람과 관련된 내용을 작성하세요. 프레젠테이션 할 때 여러분의 아이디어를 방어해야 할 수도 있습니다. 질문과 답변은 사려 깊게 작성하세요. 즉흥적인 답변은 일반적으로 커뮤니케이션에 해가 됩니다.

### 친절하고 배려하기 **Being kind and considerate**

**친절은 초능력이에요. 휘두르세요.**

침착하고 친절하며 도움을 주는 것은 누군가를 차단하는 것보다 더 멀리 갈 수 있습니다. 팀 내 사람들에게 친절하게 대하는 것은 팀을 더 강력하고 성공적으로 만드는데 도움이 됩니다. 팀 외부의 사람들에게도 친절하게 대하세요. 조직의 모든 부서(인사, 재무, 마케팅)를 동등하게 존중하세요. 그들에게 직접적으로 도움을 주지는 못하지만 항상 그들의 업무를 이해하고 공감할 수 있습니다. 다른 사람이 잘했거나 칭찬을 받았을 때 축하하거나 감사하세요. 친절은 전염됩니다. 친절하게 대했던 사람들은 앞으로 어떤 도움 요청에도 응할 가능성이 높습니다.

**사람들에게 잘하고 있다고 자유롭게 말하세요.**

개선이 필요할 때 피드백을 제공하는것도 중요하지만, 일이 잘 진행되고 있을 때 긍정적인 피드백을 제공하는 것도 중요합니다. 이를 통해 팀은 자신이 변화를 일으키고 있고 가치를 인정받고 있다는 것을 알 수 있습니다.

### 아니오의 힘 **The power of NO**

**아니오라고 말하는 것이 지나치게 헌신하는 것보다 낫습니다.**

우리 대부분은 더 많은 일과 관련하여 “아니오”라고 말하는데 능숙하지 않습니다. “아니오”가 선택 사항이라는 것을 깨닫지 못하거나 도전을 즐기기 때문일 수 있습니다. 하지만 지나치게 많은 일을 맡기면 일이 지연될 수 있으므로 책임감을 가져야 합니다. 상대방에게 이미 해야 하는 일이 무엇인지 알려주고 소요 시간에 대한 합리적인 추정치를 제공하는 것은 존중의 표시입니다. 이는 상대방이 다른 사람에게 부탁하거나 일정을 연장하는 등 다른 선택지를 고려할 수 있는 기회를 제공합니다. 경영진은 제품의 품질에 중대한 영향을 미칠 수 있다는 것을 알고 있다면 빠른 시간 내에 무언가를 제공하도록 요구하지 않을 것입니다.  여러분이 만약 시니어 매니저라면 팀원에게 나쁜 아이디어에 대해 거절할 수 있는 [권한](https://hbr.org/2017/06/help-your-team-stop-overcommitting-by-empowering-them-to-say-no)을 부여하세요.

> 시니어 개발자(또는 생산적인 사람)는 거절하는데 능숙합니다. 사람들은 여러분이 할애할 수 있는 것보다 더 많은 시간을 요구할 것입니다. 부드럽지만 단호하게 거절하거나, 다른 사람에게 일을 맡기거나(위임), 매니저에게 더 많은 시간을 할애할 수 있는지 논의해 달라고 요청할 수 있습니다. [[1]](https://news.ycombinator.com/item?id=18131722)
> 

**모든 사람을 만족시킬 수는 없습니다. “예”와 “아니오”를 말할 때 매우 신중해야 합니다.**

모든 것에 “아니오”라고 말하는 리더의 반대는 모든 것에 “예” 라고 말하면서 명확한 경계를 설정하지 않는 것입니다. 현재 리소스로 합리적으로 실행할 수 있는 범위보다 더 많은 일을 맡게 되면 리더와 팀, 고객 모두에게 마음의 상처를 줄 수 있습니다. 사람들이 “예”라고 말하거나 부드럽게 반발해야 하는지에 대한 규범을 설정하기 위해 리더를 찾을 것이기 때문에 리더는 이러한 점을 잘 파악하는것이 특히 중요합니다.

### 수용과 존중 **Acceptance and respect**

**모르는 것이 있을 때 인정하고 주니어에게도 열린 마음으로 도움을 요청하세요.**

**모르는 것이 있으면 인정하는 것이 좋습니다. 소프트웨어에서 가장 중요한 기술 중 하나는 답을 찾고 그로부터 배울 수 있는 것입니다.**

시니어 리더는 주변의 주니어들이 프로젝트의 기술적 뉘앙스를 더 잘 알고 있을 수 있다는 사실을 받아들이는 법을 배워야 합니다. 모르는 것이 있으면 인정하고 주니어 엔지니어에게 설명하게 하는 것도 괜찮습니다. 그들은 여러분의 정직함과 배움에 대한 관심을 더 존중할 것이며, 여러분은 무슨 일이 일어나고 있는지 더 잘 파악하고 가치를 더할 것입니다. 주니어 엔지니어는 편안한 수준에 따라 공개적으로 혹은 비공개적으로 시니어에게 기술 개념을 설명해야 합니다.

### 정보 공유 **Information sharing**

**미팅과 Q&A 세션을 통해 올바른 질문을 하고 지식을 교환하며 팀에 정보를 제공하세요.**

미팅을 진행할 때 혼자만 이야기하지 마세요. 미팅은 다른 사람들이 아이디어를 공유하고 솔직한 피드백을 제공할 수 있는 기회이므로 경청하고 다른 사람들이 기여할 수 있는 공간을 만들어 주세요.

주니어 엔지니어는 너무 많은 질문을 하는 것을 부끄러워 할 수 있습니다. 여러분이 시니어 엔지니어라면 맥락을 언급하여 올바른 질문을 하도록 유도할 수 있습니다. 질문이 있을 땐 질문하는 사람에게 질문을 해줘서 고맙다고 알려주세요.

### 유연성 **Flexibility**

**여러분의 의견을 당당하게 옹호하되, 이를 반박하는 새로운 증거가 있을 때 마다 검토하세요.**

다른 의견을 경청하는 것은 커뮤니케이션의 핵심입니다. 문제에 대한 솔루션이 두 가지 이상 있을 수 있기 때문에 이는 필수적입니다. 여러분의 견해에 단호하기보다는 다른 의견을 듣고 평가하세요. 여러분이 이전에 간과했던 측면을 제시할 수도 있습니다. [Paul Saffo’s principle](https://www.saffo.com/02008/07/26/strong-opinions-weakly-held/)에 따르면 “*강한 의견은 약하게 주장하라*”는 원칙은 자신의 의견을 당당하게 옹호하되, 이를 반박하는 증거가 있을 때 마다 검토하라고 말합니다. 아이디어나 의견을 제시한 사람을 고려하지 않는 과학적 증거에 기반한 방법입니다.

### 기록 유지 **Maintaining a record**

**비공식 미팅 후 친근한 이메일을 보내면 논의 중에 이루어진 핵심 사항이나 책무를 재확인하는데 도움이 됩니다.**

구두 커뮤니케이션의 단점은 잊어버리거나 잘못 기억할 수 있다는 것입니다. 발생한 모든 일을 기록하고 관련 논의에 대해 승인을 받으면 이러한 위험을 제거할 수 있습니다. 여러분 혹은 다른 사람이 업무를 돕기로 동의한 경우, 상사를 포함한 모든 사람이 동일한 정보를 공유하고 있는지 확인하기 위해 이메일을 통해 데드라인을 확인합니다. 계획되지 않은 작업을 기록해 두는 것도 평가 논의에 도움이 됩니다.

### 선의 **Good faith**

**언제 침묵을 지키고 역학 관계를 관찰해야 하는지 알아두세요.**

일부 결정을 이해하지 못하거나 기술 및 비즈니스상의 이유로 이해 되지 않는 상황이 있을 수 있습니다. 이는 여러 팀이 참여하는 논의에서 발생할 수 있습니다. 선의로 참여하며 사람들이 공개적으로 악의적인 위험을 감수하지 않을 것이라고 가정합니다. 전체 상황을 파악하지 못했거나 우선순위가 다를 수 있습니다. 최종 결정에 대해 화를 내거나 좌절하지 말고 질문하고 의견을 말하세요.

# 연공서열 **Seniority**

우리는 우리의 역할이나 역량 면에서 경력을 성장시키기를 열망합니다. 어떤 사람은 고위 기술직에 관심이 있는 반면, 어떤 사람은 리더십이나 관리직을 희망하기도 합니다. 어떤 경우든 직급이 높은 사람들이 보이는 몇 가지 주요 특징이 있습니다. 여정 내내 여러분의 성장을 이끌어줄 멘토가 있을 수 있습니다. 다음은 시니어 롤을 준비하며 자질을 개발하기 위한 저의 접근 방식입니다.

### 연공서열과 전략적 사고 **Seniority and strategic thinking**

**불확실성이 있다고 해도 결정을 내리거나 행동하세요.**

아무것도 결정하지 않는 것보다 어떤 결정을 내리는 것이 더 낫다는 것을 자주 알게 될 것입니다. 적어도 다른 사람들이 여러분이 어떤 방향으로 기울고 있는지 알 수 있기 때문입니다. 때로는 리더로서 우리 팀이 우리가 내리기를 기대하는 의사 결정에 충분한 시간을 할애하지 않는 경우가 있습니다. 모든 사실을 100% 확신할 수 없기 때문입니다. 우리는 할 수 있는 한 자신감 있는 결정을 내리는 데 필요한 세부 사항을 최대한 완벽하게 파악할 수 있고 시도해야 하지만 이것이 항상 가능한 것은 아닙니다. (예: 시간 위기) 이로 인해 팀원들은 오랜 시간 기다리거나 불확실한 상황에 처할 수 있는데, 이 때 제한된 정보를 바탕으로 의사 결정을 내리는 방법을 능동적으로 개선하는 것이 도움이 될 수 있습니다.

**리더는 시야를 넓혀 전략적으로 사고하고 다른 사람을 위해 로드맵을 제시하는 사람입니다.**

전략적으로 사고하고 계획하며 더 넓은 범위에 적용하는 능력은, 이상적으로는 경험과 함께 성장합니다. 개인 기여자(individual contributer 이하 IC)로서 여러분은 할당된 업무 또는 현재 작업 중인 과제나 기능에 집중할 수 있습니다. 직급이 올라갈수록 업무의 영향력은 특정 업무와 프로젝트를 넘어 확장됩니다. 옵션을 검토할 때 이점과 제약 조건의 관점에서 더 큰 그림을 보는 법을 배웁니다. 소프트 스킬의 적용 범위도 넓어집니다. 예를 들어, 이전에는 팀을 위해 의사 결정을 내리거나 팀의 다른 엔지니어와 소통했다면, 성장함에 따라 여러분의 선택과 소통이 여러 팀에 영향을 미치게 됩니다.

### 솔선수범 **Leading by example**

**팀원들에게 물고기 잡는 법을 가르치세요. 항상 문제를 대신 해결해주지 말고, 팀원들이 스스로 해결하는 기술을 개발하도록 부드럽게 안내하세요.**

엔지니어링 리더는 권한을 부여합니다. 시니어가 될수록 토이를 버리고 팀원들을 코칭하고 위임하며 성공할 수 있도록 돕는 것이 도움이 됩니다. 이는 효율성을 확장하는 방법입니다. 단순히 답을 제시하는 것 이상으로 좋은 질문을 함으로써 가능합니다.

**어려운 문제를 평가할 때 모범을 보이고 누군가 솔루션을 제시하면 관련 질문을 합니다.**

기술 트랙의 시니어는 팀 안팎에서 조율, 협상, 합의를 담당합니다. 그들은 자신의 성과 뿐 아니라 팀 전체 성과를 향상시키는 데 기여합니다. 시니어 엔지니어로서 가끔 새로운 기술을 습득하거나 현장을 이해하기 위해 코딩을 할 수도 있지만, 이는 직무(JD)에 포함되지 않습니다. 대신 아키텍처 다이어그램에서 누락된 부분이 없는지, 코드에 허점이 없는지 확인하는 역할을 합니다. 여러분은 여러분의 결정이 기술적 또는 비즈니스 가치를 어떻게 제공하는지에 대한 증거나 이유를 설명할 수 있어야 합니다.

시니어 엔지니어는 소프트웨어 시스템, 인적 시스템, 팀을 설계하는 데 능숙해야 합니다. 다양한 엔지니어 그룹을 이끌고, 그들에게 작업을 위임하고, 코드 품질/성능/단순성에 관심을 갖도록 멘토링할 수 있어야 합니다. 필요한 경우 피드백을 제공하고 필요한 경우 그들을 지지할 수 있어야 합니다. 동시에 조직에서 가시성을 확보하기 위해 자신과 업무, 어려운 문제를 해결할 수 있는 능력을 홍보, 마케팅하여 가시성을 높일 수 있어야 합니다. 전반적으로, *팀원 및 경영진과의 관계를 관리할 수 있어야 합니다.*

### 효율성을 확장하세요 **Scale your effectiveness.**

세계 최고의 엔지니어링 업적은 개인이 아닌 엔지니어링 팀에 의해 이루어집니다. 따라서 더 많은 것을 달성하려고 하거나 회사에서 “시니어”가 될 준비가 되었다는 것을 보여주고 싶다면, 협업과 멘토링을 통해 효율성을 크게 증가시키세요. 이것은 자신 뿐 아니라 다른 팀원들에게도 어떻게 가치를 더하는지 보여줄 수 있어야 합니다.

저는 “나”에서 “우리”로 마인드셋을 전환해야 한다는 것을 깨달았을 때 Google의 시니어 엔지니어가 되는 길에 길에 들어선 것 같았습니다. 다른 사람들과 협업하고 제가 배운 것을 공유하고, 주변 사람들의 기술과 전문성을 향상시키는데 집중하면서 훨씬 더 많은 일을 해내기 시작했습니다.

개인 기여자(IC)로 시작할 때는 여러분이 이끄는 전담 “팀”이 없을 수도 있지만, 같은 생각을 가진 사람(아마 여러분의 목표에 얼라인하는)을 찾고 함께 협력하여 혼자서 할 수 있는 것보다 훨씬 더 많은 것을 성취할 수 있습니다. 직급이 높아질수록 이러한 생각은 팀을 구성하고 효율성을 지속적으로 성장시키는 방향으로 발전하게 됩니다.

### 가면증후군 **Imposter syndrome**

**실수를 하거나, 답을 모르거나, 조언을 구해도 괜찮다는 사실을 받아들이면 가면 증후군을 극복하는데 도움이 될 수 있습니다.**

우리 모두는 어느 시점에서 특정 역할이나 직무에 부적합하다고 느낀 적이 있습니다. *가면 증후군*은 진짜이며 매우 흔한 증상입니다. 이는 분명히 성공한 사람들에게도 영향을 미칠 수 있습니다. 다른 사람들이 여러분을 존경하고 조언을 구할 때에도 사기꾼처럼 느껴질 수 있습니다. 이 증후군은 치료할 수 없을지 모르지만, 호기심을 갖고 새로운 것을 배우도록 자극할 겁니다.

# 멘토링 **Mentoring**

### 다른 사람 멘토링 **Mentoring others**

**멘티가 완전히 잘못된 방향으로 나아가지 않고 스스로 일을 해나가며 숙달할 수 있도록 시기 적절한 정보를 제공하여 가드레일이 되어 주세요.**

여러분은 경력의 여러 시점에 멘토나 멘티 역할을 맡을 수 있습니다. 멘토링은 반드시 공식적인 과정일 필요는 없습니다. 다른 사람을 멘토링 할 기회를 찾거나 비공식적으로 멘토링을 받을 수 있습니다. 다른 사람을 멘토링하는것은 대인 관계 기술을 스스로 배울 수 있는 기회를 제공합니다. 다음은 멘토링 할 때 기억해야 할 몇 가지 핵심 사항 입니다.

멘토링은 미리 만들어진 솔루션을 제공하는 것이 아니라 사람들이 스스로 답을 찾을 수 있도록 안내하는 것입니다. 멘티가 문제를 해결할 때 실험할 수 있도록 하세요. 멘티는 위험과 이점을 평가할 수 있는 가장 좋은 위치에 있습니다. 단, 답을 찾는 데 필요한 도구를 제공하세요. 기술적인 문제라면 시도해 볼 수 있는 아이디어와 옵션을 제안하되, 실제 작업은 멘티가 직접 하도록 하세요. 그들이 생각하는 것을 공유하고 주의 깊게 듣고, 질문하고, 대화에 참여하게 하세요.

스스로 해결책을 찾지 못하는 경우, 문제에 접근하는 방법과 문제를 해결하기 위해 특정 패턴을 선택한 이유를 설명해 주세요. 결과를 분석하거나 이슈를 디버깅하는 방법을 가르쳐주세요. 문제를 진단하고, 솔루션을 시도하고, 구현하고, 디버깅하는 사고 과정을 공유하세요. 정답 뿐 아니라 문제 해결 기법을 공유하세요.

### 조직 전반의 멘토링 **Organization-wide mentoring**

**멘토링을 시니어 엔지니어의 역할에 포함시키면 다른 팀, 포지션, 조직으로 이동할 때 중요한 도메인 지식을 유지하는 데 도움이 됩니다.**

여러분이 누군가를 멘토링하는 것에 진지하고, 그것이 직무의 일부라고 가정해 봅시다. 이 경우 멘토링 활동을 위해 일정 시간을 할애해야 합니다. 그래야 멘토링 활동을 제대로 수행하고 멘티의 삶에 변화를 가져올 수 있습니다. 일부 조직에서는 경력 발전 사다리와 각 단계별 요구 사항을 기반으로 멘토/멘티 논의에 대해 정의된 프로세스가 있을 수 있습니다.

<aside>
💡 적절한 어휘가 없어서 사다리 라고 번역했지만 Career ladder 는 승진에 대한 은유입니다.

</aside>

### 멘티의 역할 **Mentee's role**

**멘토는 조언을 줄 수 있지만 자신의 경력과 성장을 관리하기 위해 주도적으로 조언을 실행할 수 있는 사람은 본인뿐입니다.**

여러분이 조직에서 성장하고 싶은 주니어 엔지니어라고 가정해 봅시다. 이 경우 조언은 한 가지 뿐입니다. 성장 사다리를 탐색하는 데 도움을 줄 수 있는 강력한 멘토를 찾으세요.

경력을 쌓는 동안 존경하는 코치, 멘토, 동료를 만나게 될 것입니다. 이들은 여러분이 기술을 개발하는 방법에 대한 조언을 할 수 있지만, 이를 행동할 수 있는 사람은 여러분입니다. 조언을 받아들일 때는 기술에 관한 포괄적은 표현을 주의하세요. 상황마다 다른 원칙(principles)이 필요하며 한 프로젝트에서 효과가 있었던 것이 다른 프로젝트에서는 효과가 없을 수 있습니다.

# 효과적인 팀 **Effective teams**

### 신뢰 구축 **Building Trust**

**관료주의는 팀원들을 분열시키지만 신뢰는 팀원들이 공동의 목표를 향해 일하도록 단결시킬 수 있습니다.**

엔지니어들이 함께 모여 열린 마음으로 편견 없이 브레인스토밍 하면 혁신을 이끄는 새로운 아이디어와 다양한 관점이 나올 수 있는 토대가 마련됩니다. 이는 매우 효율적이고 생산적인 팀으로 이어집니다. 하지만 팀원 간의 효과적인 협업은 팀원 간 소통과 관계가 건강할 때만 가능합니다. 다음은 효과적인 팀을 구성하고, 유지하고, 팀의 일원이 되기 위한 몇 가지 조언입니다.

신뢰 구축은 팀 구축의 가장 중요한 요소입니다. 업무를 빠르게 처리하고 팀이 효율적으로 운영되려면 계층 구조 전반에 걸쳐 팀원 간 신뢰가 필요합니다. 팀원들은 프로젝트 상태를 검토하기 위해 리뷰 및 테스트와 같은 다양한 소프트웨어 엔지니어링 프로세스를 사용할 수 있습니다. 하지만 이러한 프로세스는 신뢰가 없으면 지루하고 관료적이 될 수 있습니다. 예를 들어, 코드 리뷰 시 엔지니어를 신뢰한다면 코드에 대한 nitpick(중요하지 않은 세부 사항에 너무 많은 주의를 기울이는 행동)이 줄어들 것입니다.

### 비즈니스 모델 이해**Understanding the business model**

**변경이 비즈니스에 미치는 영향을 이해합니다.**

새로운 요구 사항을 받으면 그 이면에 있는 동기를 이해하세요. 요구 사항 문서의 “목적” 또는 “비즈니스 목표” 섹션을 대충 훑어보지 마세요. 비즈니스 모델과 이러한 요구 사항과의 관계를 이해하기 위해 질문 하세요. 기존 코드베이스 또는 주제별 전문가(SME)와의 대화를 통해 도메인 및 아키텍처에 대한 인사이트를 얻을 수 있습니다. 문서를 참조하거나 기능, 유즈 케이스를 시스템 프로세스 및 데이터 플로우에 매핑하세요.

> “많은 소프트웨어 엔지니어는 기술적인 챌린지로 문제를 해결하는 것을 좋아합니다. 비즈니스 측면을 이해하고 비용 효율적인 솔루션을 제시할 수 있다면 더 큰 보람을 느낄 수 있습니다. 사용자/고객도 여러분과 마찬가지로 하루 또는 일주일을 버티며 자신의 일을 하려고 노력하려는 사람이라는 것을 기억하세요. 그들의 삶을 지금보다 더 힘들게 만들지 않도록 노력하세요” [[1]](https://news.ycombinator.com/item?id=26177680)
> 

### 영향력 증대**Increase your impact**

**비즈니스-소프트웨어의 방정식에 대한 통찰력과 기민함은 업무의 영향력을 높여줍니다.**

비즈니스와 제품에 대한 360도 관점을 확보하면 팀과 프로젝트에 긍정적으로 기여하는데 도움이 됩니다. 영업 또는 마케팅 사고 방식을 이해하면 올바른 결정을 내리고 강한 임팩트의 업무를 수행할 수 있는 능력을 갖추게 됩니다. 팀의 성공에 미치는 임팩트가 커질수록 직무 만족도와 급여도 향상됩니다.  선배들은 감독(supervision)없이 독립적으로 일하고 팀, 프로젝트, 비즈니스에 적합한 일을 수행하여 전반적인 효율성을 높일 수 있는 셀프 스타터로서의 여러분의 능력을 인정할 것입니다.

# 일과 삶의 균형 **Work/life balance**

기술 능력, 인적 요소, 도메인 지식을 숙달한 사람이라면 소프트웨어 엔지니어로서의 기술이 항상 요구될 것이니다. 팀과 조직의 사람들이 여러분에게 조언을 구할 것입니다. 엔지니어링 업무 외에도 [협업 과부하](https://hbr.org/2016/01/collaborative-overload)의 희생자가 될 수 있습니다. 임시 요청은 시간을 잡아먹고 열정을 쏟고 있는 일을 방해할 수 있습니다.

### 시간 관리 **Time management**

**집중 업무에 맞게 캘린더 최적화하기**

집중 업무를 위해 캘린더에서 시간을 차단하세요. 저는 수 년간 이 방법을 사용해 왔으며, 디자인이나 전략 문서를 작성하거나 어려운 기술 문제를 해결하는데 매우 효과적이라는 것을 알게되었습니다. 집중 업무는 방해받지 않고 고도로 집중하여 짧은 시간에 많은 가치를 창출하는 작업입니다. Cal Newport’s 의 Deep Work는 이 주제를 잘 다루고 있습니다.

주의력 잔여물(Attention residue)은 Cal이 장시간 깊이 작업하는 것이 왜 유익한지에 대해 말하는 아이디어입니다. 한 작업에서 다른 작업으로 전환할 때 마다 이전 작업에 대한 주의력 잔여물이 남아있습니다. 이렇게 되면 정말 중요한 일에 필요한 집중력을 발휘하기 어렵습니다.

집중 업무는 *단일* 작업에 집중함으로써 한정된 시간에서 생산성을 극대화합니다. 방해 요소도 트위터도 채팅도 이메일도 없습니다. 집중 업무는 인지능력이 많이 필요한 작업을 위해 예약합니다. 시도해 보시길 강력히 추천합니다.

또한 위치를 바꾸는 것만으로도 집중 업무에 도움이 될 수 있다는 것을 알게되었습니다. 우리는 때때로 특정 장소(책상, 방, 건물)를 특정 종류의 작업과 연관시키는 함정에 빠질 수 있는데, 약간의 다양성을 추가하면 활력을 불어넣는데 도움이 될 수 있습니다.

**업무 시간을 쪼개서 일하지 않기**

산만함으로 인해 한 시간의 업무 시간이 몇 분으로 쪼개지면 스트레스를 받게 됩니다. 산만함의 원인(본인 또는 다른 사람)을 파악하고 이를 해결하세요. 그렇지 않으면 하루의 생산성이 떨어집니다.

**과도한 업무는 올바른 업무 윤리의 일부가 아닙니다.**

세상 모든 사람보다 더 열심히 일할 수는 없습니다. 많은 회사가 과로하는 직원을 “표준”으로 여기며 이것이 좋은 직업 윤리를 가진 것과 같다고 잘못 결론내립니다. 성공은 과로 뿐 아니라 다양한 요인에서 비롯됩니다.

**끊임없이 자신의 기준을 뛰어넘으려는 것은 비현실적입니다.**

저는 이런 잘못을 많이 했습니다. 차분함을 기르고 정신없는 업무 환경을 피하려면 충분히 익숙해져야 합니다. 매니저나 리더로서 팀원들이 이에 접근하는 방법을 주도할 수 있습니다. 충분히 만족하는 것이 모범이 될 수 있습니다.

**시간은 유한합니다. 더 많은 시간을 확보하려면 노력하는 대신 불필요한 작업을 제거하세요.**

많은 지침이 업무 재배치에 대해 얘기합니다. 진짜 문제는 처음부터 너무 많은 것을 성취하려고 하는 것입니다. 한정된 시간을 관리하려고 애쓰지 말고 불필요하고 시간 낭비적인 업무를 과감하게 제거하세요.

**모든 소식을 다 알 필요는 없습니다.**

많은 사람들이 새로운 이야기나 업데이트를 놓치는 것을 두려워합니다. 이것이 사람들이 매 시간 트위터, 래딧, 인스타그램 등을 확인하는데 집착하는 이유 중 하나입니다. 저도 이런 경험을 해봤습니다. 사실 이러한 정보의 대부분은 그다지 중요하지 않습니다. 대신 뉴스 요약 보기로 전환하거나 확인 빈도를 제한하세요.

이 주제에 대한 더 자세한 내용은 Jason Fried의 “[It doesn't have to be crazy at work](https://www.amazon.com/Doesnt-Have-Be-Crazy-Work/dp/0062874780)”에서 확인하세요.

**거절하는 법을 배우고, 멈춰야 할 때를 알고, 업무 중간에 휴식을 취할 수 있도록 계획하여 피로를 사전에 예방하는 것이 가장 좋습니다.**

시간 관리와 일과 삶의 균형 유지는 모든 레벨의 엔지니어에게 매우 중요합니다. 잦은 야근은 번아웃과 스트레스로 이어질 수 있습니다. 스트레스는 다른 신체적, 정신적 [합병증](https://www.apa.org/topics/stress/body)을 유발할 수 있습니다. 하루를 마감하기 전에 문제를 해결하고 싶은 유혹이 있을 수 있지만, 시간이 지나면 습관이 될 수 있습니다.

**여러분 자신과 팀 모두를 위한 휴식, 휴일, 휴가를 장려하세요.**

여러분의 건강과 가족은 매우 중요합니다. 시니어 엔지니어로서 이러한 사실을 깨닫고 팀원들에게 훌륭한 모범을 보인다면 전반적인 웰빙과 행복을 증진할 수 있습니다. 반면에 피로와 번아웃은 직장에서의 독성으로 이어질 수 있습니다.

**문제에 대한 이해가 향상되면 추정치 업데이트 하기**

거의 항상 고객이나 이해관계자는 프로젝트나 작업을 언제 완료할 수 있는지, 그리고 이 비용이 합당한지 알고 싶어합니다. 이는 전적으로 합리적입니다. 때로는 데드라인에 맞추기를 원하거나 계획된 엔지니어링 작업을 지원해야 하는 다른 곳에 종속성이 있을 수 있습니다.

소프트웨어 데드라인은 정확하게 예측하기 어려운 것으로 악명 높습니다. 추정치를 기반으로 한 데드라인은 프로젝트가 특정 단계에 있을 때만 제공해야 합니다. 시간이 지남에 따라 팀의 문제 해결 능력에 대해 더 많이 알게되면 추정치를 ”정보에 기반한” 추정치로 업데이트 해야 합니다. 첫 번째 추정치(”sizing”)는 종종 가장 신뢰할 수 없지만, 시간이 지남에 따라 개선될 수 있는 출발점입니다. 이 초기 추정치는 매우 보수적인 경우가 많습니다. 제품 요구 사항, UX나 종속성이 불분명할 경우 첫 번째 “size”에 대해 더 큰 보수적인 추정치가 도움이 되는 경우가 많습니다. 저는 종종 이러한 추정치를 PM과 협력적으로 접근하여 모두 같은 생각을 갖고 구체화할 때 가장 큰 성공을 거두는 경우가 많았습니다.

소프트웨어 추정의 문제점은 첫 번째 대략적인 추정이 초안이 아닌 기록된 계획으로 굳어질 때 발생합니다. 크리티컬 패스에 있는 팀에서 이를 채택했지만, 엔지니어링에 의한 문제(정보에 기반한 추정치의 1/n 단계가 아닌)로 간주하는 경우 문제가 될 수 있습니다. 프로젝트가 승인되면 세부 사항을 더 잘 파악하세요. 요구 사항을 해결하는 데 무엇이 필요한지에 대한 더 깊은 이해를 바탕으로 3개월의 예상 기간이 2개월 또는 4개월이 될 수 있습니다.

가능한 한 일정에 따라 추정치가 결정되는 것보다, 추정치가 일정을 결정하는 것이 좋습니다. 우리 팀에서는 대때로 조정할 수 없는 데드라인(예: 컨퍼런스)이 있지만 추정치가 이 날짜를 초과하는 경우 괜찮습니다. 메시지 변경(예: “프리뷰”), 프레이밍(”가까운 시일 내에 제공”), 미래로 미루는 것은 항상 경영진과 논의할 수 있는 옵션입니다. 물론 이것이 항상 사소한 문제는 아니라는 것을 인정합니다. 일정에 쫓기게 되면 반드시 해야 할 일과 하면 좋은 일(이것들은 미래의 스프린트로 옮깁니다)을 구분한 다음 반드시 해야 할 일이 데드라인을 맞출 수 있는지 검토합니다.

그래도 일정이 너무 타이트하다면 “이 프로젝트에 엔지니어를 추가할 수 있습니까?”, “범위를 크게 줄여도 제시간에 출시하는게 매력적입니까?” 등의 질문을 할 수 있습니다.

**때때로 프로젝트를 취소하는 것은 불편하지만 올바른 결정입니다.** 

저는 이것을 싫어하지만, 프로젝트를 취소하는 것이 팀과 조직을 위해 장기적으로 가장 건강한 결정일 때도 있습니다. 특히 출시 전에 취소되고, 인력을 더 이상 유지할 수 없어서 폐기될 수 있을 때 이를 취소하는 것이 특히 그렇습니다. 궁금해 하시는 분들을 위해 [Killed By Google](https://killedbygoogle.com/)를 읽었습니다. 가능한 프로젝트가 취소되는 상황을 최소화 하는 것을 목표로 하세요. 최근에 다년간 진행하던 프로젝트를 취소했는데 정말 힘들었습니다.

언제 이런 일이 발생할 수 있나요? 특정 시점에 적절한 새로운 프로젝트에 투자 결정을 내릴 수 있습니다. 그 시점에는 얼라인되어 마켓 핏, 조직적 참여, 인력 투입 약속 등 모든 조건이 맞아 떨어져 완전히 합리적일 수 있습니다. 1년이 지나면 시장, 리더십, 프로젝트의 중요성 등 상황이 바뀔 수 있습니다. **프로젝트가 시작될 때 세운 가정이 프로젝트 수명 동안 계속 유효한지 정기적으로 확인하는 것이 중요합니다.**

이러한 가정이 여전히 유효하다는 확신을 가질수록 프로젝트를 성공적으로 시작하고 지속적으로 지원될 가능성이 높습니다. 취소는 여러 가지 이유로 어렵지만, 무엇보다도 출시를 기대하며 제품을 만드는데 노력한 사람들이 있다는 것이 가장 큰 이유입니다. 리더로서 취소된 프로젝트에서 성공적으로 출시된 다른 프로젝트로 사람들을 다시 유도하는 일은 복잡하지만, 심리적 안전, 신뢰, 행복감을 회복시키기 위해서 중요합니다. 고객 측면에서는 사용자 신뢰와 장기적인 의사 결정이 어떻게 영향을 미칠 수 있는지 주의해야 합니다.

**기술 부채에 대해: 1온스의 예방이 1파운드의 치료보다 낫습니다.**

Titus Winters는 기술 부채를 “현재 우리가 가지고 있는 코드, 시스템과 우리가 갖고 싶었던 것과의 차이”로 정의하며 특정 종류의 부채가 다른 부채보다 더 큰 영향을 미친다고 말합니다. 어떤 부채는 조기에 발견하지 못한 실수(감독 소홀)로 인한 것일 수 있고, 어떤 부채는 사후에 알게 된 사실(뒤늦은 깨달음)로 인한 것일 수 있고, 어떤 부채는 기술 시스템의 환경 변화(맥락)로 인한 것일 수 있습니다.

기술부채를 해결하는 것을 지속적으로 우선시하는 것은 때로는 어려울 수 있습니다. “부채를 충분히 상환했다”는 이유로 발생하지 않은 버그나 중단 사항을 항상 정량화할 수 없기 때문입니다. 이러한 종류의 작업에 대한 팀의 관심을 유지하고 성과 평가에서 보상 하는 것도 매우 중요합니다. 그러나 시간이 지남에 따라 문제가 실제로 쌓이기 시작하면 “치료” 비용은 상당히 높아질 수 있습니다. 환경 오염과 마찬가지로, 수년에 걸쳐 기술 부채를 예방하는 것이 나중에 문제를 대처하는 것보다 더 저렴한 전략입니다.

부채가 쌓이는 것을 방지하기 위해 무엇을 할 수 있나요? 기술 리더는 새로운 기능을 개발 하는 것 외에도, 스프린트에서 정리 및 부채 상환에 시간을 정기적으로 할애해야 합니다. 리뷰어는 단기적인 속도 증가가 실제로 나중에 문제가 발생할 수 있음을 인지하고 있어야 합니다. 매니저와 디렉터는 기존 프로젝트와 중복되는 새로운 프로젝트를 승인할 때 장단점이 확실하지 않는 한(예: 기존 시스템의 부채를 해결하는 것이 새로운 것을 구축하는 것보다 가치가 없는 경우) 신중을 기해야 합니다. 이 모든 것의 추가로, 프로젝트 상태 모니터링이 매우 중요합니다.

**휴식과 일과 삶의 균형이 없으면 여러분이나 팀이 번아웃에 빠질 수 있습니다.**

번아웃은 성공적으로 관리되지 않은 직장 스트레스로 인한 탈진의 한 형태입니다. 팬데믹 기간 동안 많은 엔지니어가 업무 스트레스로 인해 번아웃에 빠지는 것을 봤지만, 번아웃은 기술 업계에서 항상 존재해 왔습니다. 저는 요즘 1on1에서 “당신의 스트레스 수준은 어떤가요? 제가 도울 수 있는게 있나요?” 라고 묻습니다.

제 경험에 따르면 번아웃은 서서히 발생하고 무관심으로 끝납니다. 업무 스트레스에 최선을 다해 대처하려고 노력하는 동안 서서히 에너지가 떨어지고, 동기가 사라지고, 지치기 시작합니다. 자신에게 문제가 있는 것은 아닌지 의심하지만, 에너지 부족을 보상하기 위해 몸이 초과 근무를 하고 있다는 사실을 깨닫지 못합니다. 계속 더 열심히 자신을 몰아붙이지만 결국에는 더 이상 할 수 있는 게 별로 없는 것처럼 느껴집니다.

저는 약 5년 전에 번아웃에 빠졌지만 다행히도 이를 극복했습니다. 원인이 무엇이었나요? 여러가지 일이 산더미처럼 쌓였습니다. 저는 수년 동안 일을 우선시 했고, 더 긴 시간 동안 일하면서 충분히 “아니오”라고 말하지 못했습니다. 충분한 휴식이나 휴가를 가져본 적이 없었습니다. 하루 평균 5시간 정도 잠을 잤습니다. 집에 있을 때 가족을 위한 충분한 에너지가 없어서 충분히 함께하지 못했습니다. 휴식을 취하고, 더 많이 자고, 일하는 시간에서 더 많은 가치를 끌어내고, 더 잘 위임하고, 일하는 시간의 “중단 시간”을 명확하게 설정하는 등 그 반대의 일을 하는 것이 “해결책”이었습니다. 

매니저로서 동료들의 번아웃을 피하기 위해서는 팀원들이 휴가를 사용하고, 휴식을 취하고, 스트레스를 받는 동료들이 잘 지내고 있는지 주기적으로 확인하도록 격려하는것이 중요하다고 생각합니다. 

**대규모 조직의 실행은 느리게 느껴질 수 있습니다. 이를 극복할 수 있는 방법이 있습니다.**

저는 엔지니어들과 “큰 조직에서 X moon-shot을 출시하는 것이 그렇게 어려운가”로 요약되는 많은 대화를 나눴습니다. 큰 조직을 [slime molds](https://komoroske.com/slime-mold/)에 비교한 Alex Komoroske의 훌륭한 비유가 있습니다. 즉, 조율의 역풍으로 인해 간단한 일이라도 실행하는 것이 예상보다 훨씬 느리게 느껴질 수 있다는 것입니다. 조직은 복잡한 시스템, 구조, 역학 관계를 가지고 있으며 프로젝트에서 조율해야 하는 사람의 수가 증가하면 역풍이 증가합니다.

여기에는 다른 사람의 작업 난이도를 과소평가하는 것(예: 의존성을 구축하는 경우)을 포함하여 많은 힘이 작용합니다. 이러한 문제는 기능 장애를 확산시킬 수 있으므로 무시해서는 안됩니다. 이러한 역풍을 헤쳐나가는 한 가지 방법은 가능한 많은 작업을 분리하여 OK 타임라인에 도달하고 결국 X를 출시하는 방향으로 수렴할 수 있도록 하는 것입니다.

처음부터 X 전체를 처리하는 대신 moon-shot(큰 위험을 감수하는 노력)만을 목표로 삼지 않고 대신 목표에 더 가까이 다가갈 수 있는 roof-shot(가치를 실현하기 위한 안전한 단계)을 정의할 수 있습니다. 이 문제가 익숙하게 느껴진다면 Alex의 deck을 읽어보시길 강력히 추천합니다.

**프로젝트가 아닌 문제에 집중**

사용자에게 해결되지 않은 요구 사항(예: 문제)이 있다고 가정해 봅시다. 특정 프로젝트에 소속된 엔지니어라면 *특정 프로젝트*가 이 문제를 어떻게 해결할 수 있는지 묻는 것이 일반적입니다. 비슷한 형태의 프로젝트가 있는 대규모 조직에서는 여러 엔지니어가 독립적으로 이러한 생각(”내 프로젝트가 이 문제를 어떻게 해결할까?”) 하는 것을 볼 수 있습니다. 하지만 여러 프로젝트 포트폴리오를 갖고 있는 경우에는 이 방법이 명확하지 않을 수 있습니다. 사용자가 여러 프로젝트를 함께 사용한다면 어떻게 될까요? 서로의 접근 방식을 모른 채 각자 조금씩 다른 방식으로 문제를 해결할 수 있습니다. 대신 “이 문제에 대한 올바른 End to End 솔루션은 무엇인가”라고 질문하고 어떤 프로젝트나 일련의 프로젝트에 대한 변경 사항이 이러한 요구를 잘 해결할 수 있는지 다시 살펴봅니다. 이를 위해서는 여러 관련 프로젝트에서 일하는 사람들이 더 깊이 협업하도록 해야 할 수 있습니다. 하지만 결국에는 사용자에게 더 나은, 덜 혼란스러운 플로우를 제공할 수 있습니다.

# 결론 **Conclusion**

> “탁월함으로 자신을 둘러싸고 자신이 하는 일에 최고인 사람들과 함께 일하세요”  - Brian Staufenbiel
> 

배울 수 있는 사람들과의 우정과 관계에 투자하세요. 그들의 지도, 멘토링, 성공과 실패에 대해 마음을 여세요. 도움이나 통찰력을 요청하는 것을 두려워하지 마세요. 대부분의 경우 그것은 단지 질문일 뿐입니다.

모든 단계에서 조직의 기술, 비즈니스 도메인, 인적 자원에 대한 숙달은 시간이 지남에 따라 배양되어야 한다는 점을 기억하세요. 다른 조직의 전문가를 고용하여 첫날부터 생산성을 기대할 수는 없습니다. 훌륭한 엔지니어라면 조직의 성장에 기여할 것입니다. 그 대가로 새로운 기술을 습득하고 스스로 성장할 수 있는 새로운 길이 열릴 것입니다.

*친절한 피드백과 기여를 해주신 Leena Sohoni, Joshua Cruz, Kara Erickson, Jeff Posnick, Houssein Djirdeh, Sriram Krishnan에게 감사드립니다.*