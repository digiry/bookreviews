<!-- markdownlint-disable MD025 MD036 MD041 -->

![Practical Obejct Oriented In Ruby](cover.jpg)

# 한줄평

객체지향 설계 디자이너를 위한 실용서.

# 책소개

`루비로 배우는 객체지향 디자인` 이 책의 부제는 지속가능한 소프트웨어를 만드는 방법이다. 원제는 번역된 문구와 비슷하지만 부제는 다르다. 원제는 `Practical Object-Oriented Design in Ruby`이고 부제는 `AN AGILE PRIMER`이다. 원제를 직역하면 "루비로 된 실용적인 객체지향 디자인: 애자일 초보"라고 할 수 있는데 지속가능한 소프트웨어를 만드는 방법이라는 국문판 부제가 원서 부제보다 내용에 잘 어울린다고 생각한다.

2013년도에 원서가 출판되었고 번역서는 1년 뒤인 2014년도에 출판되었다. 저자는 샌디 메츠(Sandi Metz)님이다. 저자의 홈페이지([샌디메츠 홈페이지](https://www.sandimetz.com/about))에 보면 직업을 선생님, 작가, 컨설턴트로 소개하는데 직업들을 보니 저자가 설명을 잘하는게 수긍이 된다. 번역도 잘되어 매끄럽게 읽히는 것 같다. 번역은 박건한님이다.

# 감상평

책 제목만 보고 루비를 모르면 이해하기 힘들겠다고 생각했는데 충분히 이해할 수 있게 구성되어 있다. 직설적으로 말하는 듯한 글이라 더 와닿는 느낌이었다. 또한 책의 내용 구성도 문제에 부딪히고 그걸 해결해 가는 과정을 보여줌으로서 주제를 이해하는데 큰 도움이 된다. 하나 더 좋았던 점은 문제나 해결방안을 바라보는 사고과정이나 그 안에 담겨 있던 생각들이 자주 나온다. 건조하게 해결법과 근거만을 설명하는게 아니라 머릿속에서 생각의 흐름을 알 수 있게 해 줘서 더 빠르게 책에 몰입하게 해 줬다.

> 디자인은 나중에 디자인할 수 있는 여지를 남겨 놓기 위한 것이고, 그 최종 목표는 변화의 비용을 최소화하는 것이다.

이 주장이 저자가 핵심적으로 하고 싶은 말이라고 볼 수 있다. 그리고 읽다 보면 저자가 이 내용을 자주 언급해서 자연스럽게 이게 저자가 하고 싶은 말이었다는 걸 알게 된다.

이 책은 객체지향을 고민하는 사람이거나 입문하는 사람에게 적극 추천한다. 그리고 이 책과 더불어 `객체지향의 사실과 오해`를 읽는다면 이 책에서 말하는 `메시지`, `역할`, `책임`의 이해를 넓힐 수 있다고 생각한다. 특히 이 책은 코드 사례를 효과적으로 활용하면서 설명하기 때문에 실제 코딩할 때도 도움이 많이 될 것 같다.

# 각장 요약

## 1장 객체지향 디자인

* 객체지향 소프트웨어는 이 세계를 객체 사이의 자발적인 상호연관의 연속으로 파악한다.
* 디자인은 나중에 디자인할 수 있는 여지를 남겨 놓기 위한 것이고, 그 최종 목표는 변화의 비용을 최소화하는 것이다.
* 애자일 작업방식은 변화를 보장한다. 그리고 코드를 수정할 수 있는 우리의 능력은 애플리케이션의 디자인에 달려있다.
* 애자일은 디자인을 거부하지 않는다. 디자인을 필요로 한다. 디자인을 필요로 할 뿐 아니라, 진자 좋은 디자인을 필요로 한다. 우리가 만들 수 있는 최상의 디자인이 필요하다.  간단하고 유연하며 내 마음대로 조작할 수 있는 코드가 꼭 필요하다.
* 경험이 부족한 프로그래머라면 지나치게 미래를 많이 예상하고 이런 예상을 담은 디자인을 만들 것이다. 이런 디자인에 들은 노력은 결코 그 값어치를 하지 않는다.
* 능력 있는 디자이너가 오늘 아침에 조심스럽게 작성한 코드는 오늘 저녁의 개발 비용을 낮출 수 있을 것이다.
* 대부분의 프로그래머는 이 두 극단 사이 어딘가에 위치해 있다.
* 변화를 손쉽게 받아들일 수 있도록 코드를 배치하는 일, 이것이 디자인이다. 디자인에서 가장 눈에 띄는 요소는 원칙과 패턴이다. 하지만 원칙을 올바르게 적용하고 적절한 패턴을 사용해도 수정하기 쉬운 애플리케이션을 만들었다고 확신할 수는 없다.

## 2장 단일 책임 원칙을 따르는 클래스 디자인하기

* 어떤 클래스를 만들어야 할까? 몇 개나 만들어야 할까? 어떤 행동을 구현해야 할까? 하나의 클래스는 다른 클래스에 대해 얼마나 알고 있어야 할까? 다른 클래스에게는 어느 정도까지 열려있어야 할까? . . . 현재 시점에서 우리가 해야 하는 일은 일단 깊게 심호흡을 한 번 하고, 클래스는 다순해야 한다는 마을 명심하는 것이다.
* 우리는 이런 질문들에 압도 당한다. 모든 결정은 위험으로 가득 차 있고 한번 결정한 것은 되돌릴 수 없을 것 같다. 하지만 두려워 말자. 현재 시점에서 우리가 해야 하는 일은 일단 깊게 심호흡을 한 번 하고, **클래스는 단순해야 한다**는 말을 명심하는 것이다.
* `데이터 구조를 들여다보던 작업`을 `객체에 대한 메시지를 전송`으로 대체한다.
* 최종적인 디자인을 모르는데도 이런 리팩터링을 해야 하는 걸까? 필요하다. 리팩터링은 디자인이 명확하기 때문에 필요한 것이 아니라 오히려 디자인이 불명확하기 때문에 필요한 것이다.
* 여러 메서드가 각각 하나의 책임을 질 때 다음과 같은 이득을 얻을 수 있다.
  * 예전에 몰랐던 특성이 드러난다.
  * 주석을 넣어야 할 필요가 없어진다.
    * 주석은 실행되는 코드가 아니기 때문에 시간이 지나면 바스러지는 종이문서 같다.
    * (-> 이 말에 엄청 공감된다.)
  * 재사용을 유도한다.
  * 다른 클래스로 옮기기 쉽다.

## 3장 의존성 관리하기

* 서로 협업하려면 객체는 다른 객체에 대한 지식이 있어야 한다. `지식은 의존성을 만들어 낸다.`
* 의존성을 줄이는 작업은 곧 불필요한 본드가 무엇인지 알고 그것을 제거하는 과정이다.
* (-> 모든 본드를 제거할 순 없을 것이다. 불필요한 본드가 무엇인지 아는게 중요하다.)
* 추상화의 훌륭한 점은 일반적이고 안정적인 성질을 지닌다는 점이다.
* 절대로! 어떤 상황에서든 수정하고 싶지 않게 만든다. 모두가 이 클래스를 수정하기를 꺼려하기 때문에 우리의 애플리케이션은 영원히 코칠 수 없는 문제를 안고 간다.
* `자기 자신보다 덜 변하는 것들에 의존하라`는 이번 절에서 검토한 생각을 종합해 줄 수 있는 격언이다.
* 의존성 관리의 핵심은 그 방향을 관리하는 것이다. 평온한 유지보수라는 궁극의 목표를 향한 길은 자기 자신보다 덜 변하는 것에 의존하는 클래스들로 덮여있다.

## 4장 유연한 인터페이스 만들기

* 애플리케이션은 클래스로 구성되어 있지만 메시지를 통해 정의된다. 소스 코드 레포지토리에 무엇이 들어갈지를 결정하는 것은 클래스지만 애플리케이션의 움직임을 반영하는 것은 메시지이며 이 메시지가 애플리케이션을 살아 움직이게 한다.
* 클래스의 퍼블릭 인터페이스를 구성하는 메서드는 바깥 세상을 향한 클래스의 얼굴이다. 이런 메서드는,
  * 클래스의 핵심 책임(Primary responsibility)을 드러낸다.
  * 다른 객체에 의해 호출될 수 있다.
  * 쉽게 변경되지 않는다.
  * 다른 객체가 안정적으로 의존할 수 있다.
  * 테스트를 통해 꼼꼼하게 문서화되어 있다.
* 그 외의 메서드는 프라이빗 인터페이스의 한 부분이다. 이런 메서드는,
  * 세부적인 구현을 담당한다.
  * 다른 객체에 의해 호출되지 않는다.
  * 필요에 따라 언제든 변경할 수 있다.
  * 다른 객체가 의존하기에는 위험하다.
  * 테스트에서 다루지 않을 수도 있다.
* 자신보다 덜 변화하는 것에 의존해야 한다는 생각은 클래스 내부에도 적용된다.
* 언제나 디자인 목표는 당장의 요구사항을 처리하기에 충분한 코드를 작성하면서 나중에 수정할 수 있는 여지를 최대한 확보하는 것이다.
* `객체를 가지고 있기 때문에 메시지를 보내는 것이 아니다. 메시지를 전송하기 때문에 객체를 갖게 된 것이다.`

## 5장 오리 타임으로 비용 줄이기

* 오리 타입은 특정 클래스에 종속되지 않는 퍼블릭 인터페이스이다.
* 오리 타입은 이 퍼블릭 인터페이스를 글래스로부터 분리해 낸다. 그리고 '객체가 누구인지'가 아니라 '객체가 무엇을 하는지'에 따라 가상의 타입을 만들어 낸다.
* **폴리모피즘(polymorphism)** 일바적인 정의는 다음과 같다.
* "Morph는 형태를 뜻하는 그리스어이다. morphism은 형태를 가지고 있는 상태를 뜻하며 polymorphism은 여러 형태를 가지고 있는 상태를 의미한다. 생물학자들이 이 단어를 사용한다. 다윈의 저 유명한 핀치새류는 폴리모픽하다. 하나의 종이 여러 형태를 가지고 있다."
* 객체지향 프로그래밍에서 사용하는 폴리모피즘은 같은 메시지에 반응할 수 있는 여러 객체의 능력을 의미한다. 결국 하나의 메시지가 여러 개의(poly) 형태(morphs)를 갖게 된다.
* `kind_of`, `is_a`, `reponds_to` 그리고 클래스에 따라 변경되는 case 구분은 모두 숨겨진 오리 타입이 있다고 말해준다. 이 모든 경우 코드는 이렇게 말하고 있다. "나는 네가 누구인지 알고 있고, 그렇기 때문에 네가 무엇을 하는지도 알고 있다." 이 지식은 협업하는 객체에 대한 믿음이 부족하다는 사실을 말해 줄 뿐이고 부족한 믿음은 협업 객체가 운신할 수 있는 폭을 줄인다. 그리고 코드를 수정하기 어렵게 만드는 의존성을 불러온다.

## 6장 상속을 이용해 새로운 행동 얻기

* 기본적으로 상속이란 자동화된 메시지 전달(automatic message delegation) 시스템이다.
* 리팩터링 전략을 선택할 때, 물론 일반적으로 디자인 전략을 선택할 때도 마찬가지인데, 다음과 같은 질문을 전져 보면 좋다. "내가 실수하면 어떤 일이 벌어질까?" 비어 있는 상위클래스를 만들고 추상화 코드를 위로 올리는 전략을 취할 때 발생할 수 있는 최악의 경우는 무엇일까? 추상화할 수 있는 코드를 하나도 찾지 못하는 것이다.
* 기본 구조를 상위클래스가 정의하고 상위클래스에서 메시지를 전송하여 하위클래스의 특수한 값을 얻는 기술을 `템플릿 메서드(template method)` 패턴이라고 부른다.
* 하위클래스가 알고리즘을 알고 있고 super를 전송하는 대신 `훅(hook)`메시지를 전송할 수 있다. 훅 메시지는 정해진 메서드 구현을 통해 하위클래스가 정보를 제공할 수 있도록 만들어 주는 메시지이다. 이 방법을 사용하면 하위클래스는 알고리즘에 대해 몰라도 되며, 상위클래스가 모든 권한을 가질 수 있게 된다.

```ruby
class Bicycle
    attr_reader :size, :chain, :tire_size
    
    def initialize(args={})
        @size = args[:size]
        @chain = args[:chain] || defualt_chain
        @tire_size = args[:tire_size] || default_tire_size
        post_initialize(args)
    end

    def spares
        { tire_size: tire_size,
          chain: chain}.merge(local_spares)
    end

    def default_tire_size
        raise NotImplementedError
    end

    # 하위클래스가 재정의 할 수 있다.
    def post_initialize(args)
        nil
    end

    def local_spares
        {}
    end

    def default_chain
        '10-speed'
    end
end

class RoadBike < Bicycle
    attr_reader :tape_color

    def post_initialize(args)
        @tape_color = args[:tape_color]
    end

    def local_spares
        {tape_color: tape_color}
    end

    def default_tire_size
        '23'
    end
end

class MountainBike < Bicycle
    attr_reader :front_shock, :rear_shock

    def post_initialize(args)
        @front_shock = args[:front_shock]
        @rear_shock = args[:rear_shock]
    end

    def local_spares
        {rear_shock: rear_shock}
    end

    def default_tire_size
        '2.1'
    end
end
```

* RoadBike와 MountainBike는 구체적인 구현만 가지고 있기 때문에 훨씬 읽기 쉽다. 한눈에 훑어봐도 이 클래스가 어떤 일을 하는지 알 수 있고 Bicycle의 특수한 형태라는 것도 명확하다.
* 새로운 하위 클래스는 탬플릿 메서드만 구현하고 있으면 된다. 마시작 예시는 애플리케이셔에 익숙하지 않은 사람에게도 새로운 하위클래스를 만드는 것이 얼마나 간단한지 보여준다. RecumbentBike클래스는 Bicycle의 새로운 형태, 특수한 형태이다.

```ruby
class RecumbentBike < Bicycle
    attr_reader :flag

    def post_initialize(args)
        @flag = args[:flag]
    end

    def local_spares
        {flag: flag}
    end

    def defulat_chain
        "9-speed"
    end

    def default_tire_size
        '28'
    end
end

bent = RecumbentBike.new(flag: 'tall and orange')
bent.spares
# -> {:tire_size => "28",
#     :chain     => "10-speed",
#     :flag      => "tall and orange"}
```

* 이번 장의 간단한 예시는 두 개의 클래스르 가지고 작업했지만 실생활에서는 세 개의 타입이 제공하는 충분한 정보를 얻을 때까지 기다리는 것이 더 좋을 수 있다.

## 7장 모듈을 통한 역할 공유

* 어떤 문제들은 이 문제를 해결하기 위해서가 아니라면 별로 연관이 없는 개체들이 공통의 행동을 공유하게 만든다. 이런 공통의 행동은 클래스와 아무런 상관이 없다. 이 행동은 객체가 수행하는 **역할(role)** 이다.
* 메서드를 추가하기 위해서는 실제 코드를 작성해야 하고, 이 코드를 어디에 작성할지 고민할 수밖에 없다. 우리는 두 가지를 결정해야 한다. 코드가 무엇을 해야 하는지, 그리고 코드를 어디에 두어야 하는지. 일을 시작하기 가장 좋은 출발점은 이 두 결정을 분리해서 다루는 것이다.
* 이번 장은 '고전적 상속'과 '모듈을 통한 코드 공유' 사이의 구분을 유지하기 위해 노력해왔다. 상속인 것과 상속처럼 행동하는 것의 차이는 분명 중요하다.

`메서드 탐색(method lookup)에 대한 거의 완벽한 설명`

```plain
             Object (Object 클래스에서 정의된 메서드)
                |
             modules (Bicycle 클래스에 인클루드된 모듈에서 정의된 메서드)
                |
             Bicycle (Bicycle 클래스에서 정의된 메서드)
                |
             modules (MountainBike 클래스에 인크루드된 모듈에서 정의된 메서드)
                |
           MountainBike (MountainBike 클래스에서 정의된 메서드)
                |
             modules (MountainBike의 인스턴스에 익스텐든된 모듈에서 정의된 메서드)
                |
           singleton class (단 하나의 MountainBike 인스턴스가 전의하고 있는 메서드)
                |
메세지 --> a mountain bike
```

* 우리의 목표는 이 기술로부터 도망치는 것이 아니라 꼭 필요할 때, 올바른 곳에서, 제대로 사용하는 법을 배우는 것이다.
* 모든 하위클래스가 아니라 몇몇 하위클래스에게만 적용되는 코드가 상위클래스에 포함되어 있으면 안 된다. 이 원칙은 모듈에도 적용될 수 있다. 모듈에 포함되어 있는 코드는 이 모듈을 사용하는 모든 객체에게 적용되어야 한다.
* 하위 클래스가 상송받은 메서드를 재정의해서 `나는 이런 것을 하지 않습니다`라고 말하고 있다면 사실은 `나는 이런 것이 아닙니다`라고 말하는 것과 별반 다르지 않다. 여기서 좋은 결과가 나올 리 없다. 추상화 해야 할 내용을 잘 찾지 못하겠다면 그럴 만한 내용이 없는 뜻일 수도 있다. 그리고 공통으로 사용할 만한 추상화된 코드가 없다면 주어진 디자인 이슈의 해결채은 상속이 아니다.
* 템플릿 메서드는 알고리즘의 변경되는 지점들을 표현하고, 이 템플릿 메서드를 만드는 것을 통해 우리는 어떤 내용이 변하는 것이며 어떤 것이 변하지 않는 내용인지 명시적으로 선택하게 된다.
* (->이게 템플릿 메서드의 특징인거 같다. 변하는 것과 변하지 않는 것을 제공한다.)
* 같은 역할을 수행하는 객체가 행동을 공유해야 할 때 이들은 루비의 모듈을 사용한다. 모듈에 정의된 코드는 어떤 객체에든 추가할 수 있다. 클래스의 인스턴스든 클래스 그 자체든 또는 다른 모듈이든 상관없다.
* 리스코프 치원 원칙의 수학적 의미는 '상위타입은 자신의 하위타입으로 치환될 수 있다.'는 뜻이고, 루비의 언어로 표현하자면 '객체는 자기 자신이 누구라고 밝힌 그대로 행동해야 한다.'는 뜻이다.

## 8장 조합을 이용해 객체 통합하기

* **상속의 결과 받아들이기**
  * `상속의 이점`
    * 메서드를 변경하면 그 여파가 상속 관계를 따라 저 아래에까지 미친다. 때문에 제대로 구조화된 상속 관계는 매우 **적절하다(reasonable).** 코드의 작은 한 부분만 수정해도 행동의 변화를 크게 이끌어 낼 수 있다.
    * 코드에 상속을 적용한 결과를 **열려있고-닫혀있다(open-closed)** 고 표현할 수 있다. 상속 관계는 확장에 열려있고, 동시에 수정에는 닫혀있다. 기존 상속구조에 새로운 클래스를 추가하려 할 때 기존 코드를 전혀 수정하기 않아도 된다. 그렇기 때문에 상속관계는 **사용가능(usable)** 하다.
    * 주어진 패턴을 따라하기도 쉽다. 새로운 하위클래스를 만들려는 프로그래머는 기존 코드를 자연스럽게 참조할 수 있다. 때문에 상속 관계는 **모범이 된다(exemplary).**
    * 상위클래스와 하위클래스 사이의 '무엇이다 관계(is-a relationship)'는 매우 자연스럽다.
  * `상속의 비용`
    * 상속을 사용하는 데 따르는 우려는 크게 두 가지다. 첫째, 상속이 어울리지 않는 문제를 해결하는 데 상속을 사용할 수 있다. 구조 자체가 잘못되어 있기 때문에 새로운 행동이 끼어들 자리가 없다. 어쩔 수 없이 코드의 중복을 허용하거나 코드를 다시 작성하게 된다.
    * 둘째, 상속이 문제를 해결하기 위한 적절한 방법일지라도 다른 프로그래머가 우리가 작성한 코드를 우리가 바라지 않는 방식으로 사용할 수 있다.
    * **적절하고(reasonable), 사용가능하고(usable), 모범이 되는(exemplary) 것.** 이런 가치들은 동전 양면의 한쪽과 같은 것들이다.
      * **적절함(reasonable)** 의 반대편에는 잘못된 상속 관계 속에서 코드를 수정할 때 매우 큰 비용이 발생한다는 문제가 있다. 작은 수정 하나가 모든 것을 엉망으로 만들어 버린다.
      * **사용가능성(usable)** 의 반대쪽에는 새로운 행동을 도저히 추가할 수 없는 상황이 있다. 두 클래스의 특성을 하나의 객체 속에 묶어내지 못한다. 이미 만들어 놓은 행동을 수정하지 않고는 다시 사용할 수 없는 것이다.
      * **모범이 됨(exemplary)** 의 반대편에는 초보 프로그래머가 잘못된 상속 관계를 확장하려 했을 때 만들어 내는 엄청난 혼란이 숨어 있다. 적용할 수 없는 상속 관계를 발견했다면 확장하지 말고 리팩터링해야 한다.
  * 상속은 "내가 실수하면 어떤 일이 벌어질까?라는 질문을 매우 중요하게 고려해야 한다.
  * 객체를 상속받아야만 행동을 가져올 수 있는 프레임워크를 만드는 것은 좋지 않다. 누군가의 애플리케이션은 이미 자신의 상속 관계를 가지고 있기 때문에 우리가 만든 프레임워크를 상속받는 것 자체가 불가능할 수도 있다.
* **조합의 결과 받아들이기**
  * `조합의 이점`
    * 작은 객체들은 하나의 책임만을 갖고 있고, 자신의 행동을 직접 명시하고 있다. **투명한(transparent)** 객체들이다.
    * 조합된 객체는 자신의 부분들을 인터페이스를 통해 관리하기 때문에 한 부분을 새로 추가하는 것이 쉽다. 조합된 객체의 관점에서 보자면 이미 있던 한 부분의 변형된 형태를 추가한다는 것은 충분히 말이 되는, **적절한(reasonable)** 것이며 자기 내부의 코드는 수정하지 않아도 된다.
    * 조합에 관여하는 객체들은 본질적으로 그 크기가 작다. 구조적으로 독립되어 있고 잘 정의된 인터페이스를 가지고 있다. 잘 조합된 객체는 새로운 환경에서도 손쉽게 **사용할(usable)** 수 있다.
  * `조합의 비용`
    * 조합된 객체는 여러 부분들과 관계를 맺고 있다. 각각의 부분이 작고 쉽게 이해할 수 있더라도, 이 부분들이 모여 전체가 작동하는 방식은 훨씬 불명확할 수 있다. 개별 부분들은 충분히 **투명(transparent)** 하더라도 전체는 그렇지 않을 수 있다.
    * 구조로부터 독립성은 자동화된 메시지 전달을 포기하면서 얻은 것이다. 조합된 객체는 누구에게 어떤 메시지를 전달해야 할지 명확하게 알고 있어야 한다.
* **올바른 관계 선택하기**
  * `무엇이다(is-a) 관계에서 상속 사용하기`
    * 현실세계에서 볼 수 있는 물체 중에서 고정적이고 일반-특수의 상속 관계가 뚜렷한 것은 고전적 상속으로 구조화하기 좋은 대상이다.
    * 모든 샥(shock: 자전거의 충격완충장치)은 조금씩 달라도 전부 샷(shocks)이다. 부품의 '샥-다룸(shock-ness)'이 샥의 핵심을 이룬다. 다양한 샥에 대한 가장 정확하고 상세한 설명은 '이것은 샥이다(it is-a shock)' 정도가 될 것이다.
  * `무엇처럼 행동하는(behaves-like-a) 관계에는 오리 타입을 사용하라`
    * 어떤 문제는 여러 개의 객체가 같은 역할을 수행해야 하는 상황을 만든다.
    * 역할을 이해하기 위한 좋은 방법 중 하나는 외부의 관점에서 생각해 보는 것이다. 역할을 수행하는 객체의 관점이 아니라, 역할을 부여하는 객체의 관점에서 생각해 보는 것이다.
  * `가지고 있는(has-a) 관계에서 조합 사용하기`
    * 자전거는 부품들(parts)을 가지고 있다. 하지만 자전거 자체는 부품들의 묶음 이상의 것이다. 자전거는 부품들의 행동과는 전혀 다른, 그리고 부품들의 행동보다 더 나아간 그 고유의 행동을 가지고 있다.
    * (-> 부품 자체의 행동은 고정하거나, 회전하는 등의 행동을 가진다. 하지만 자전거는 사람, 물건을 이동시키고, 운송하는 등의 고유의 행동을 가진다.)
    * 객체가 많은 부분을 가지고 있을수록 조합을 사용해서 객체를 디자인하는 것이 더 어울린다. 개별 부품들 속으로 관심을 옮겨갈수록 몇 가지 변형된 형태만을 갖는 특정 부품들을 만날 가능성이 높아진다. 이것들은 상속을 사용하기 좋은 대상들이다.
* 조합, 고전적 상속, 모듈을 통한 행동 공유는 서로 대립되는 코드 재배치 기술이다. 각각은 나름의 비용과 이익을 제공한다. 이런 차이가 미묘하게 다른 문제를 해결하는 데 특정 기술의 우위를 보장해준다. 이런 기술들은 하나의 도구일 뿐 그 이상이 아니다. 그리고 기술들을 모두 연마하면 보다 나은 디자이너가 될 수 있다. 각각을 제대로 사용하는 것은 경험과 판단력의 문제이다. **경험을 쌓는 가장 좋은 방법은 직접 실수를 통해 배우는 것이다.**

```ruby
class Bicycle
    attr_reader :size, :parts

    def initialize(args={})
        @size = args[:size]
        @parts = args[:parts]
    end

    def spares
        parts.spares
    end
end

require 'forwardable'
class Parts
    extend Forwardable
    def_delegators :@parts, :size, :each
    include Enumerable

    def initialize(parts)
        @parts = parts
    end

    def spares
        select {|part| part.needs_spare}
    end
end

require 'ostruct'
module PartsFactory
    def self.build(config, parts_class = Parts)
        parts_class.new(
            config.collect {|part_config|
                create_part(part_config)})
    end

    def self.create_part(part_config)
        OpenStruct.new(
            name: part_config[0],
            description: part_config[1],
            needs_spare: part_config.fetch(2, true))
    end
end

road_config =
    [['chain', '10-speed'],
     ['tire_size', '23'],
     ['tape_color', 'red']]

mountain_config =
    [['chain', '10-speed'],
     ['tire_size', '2.1'],
     ['front_shock', 'Manitou', false],
     ['rear_shock', 'Fox']]
```

```ruby
road_bike =
    Bicycle.new(
        size: 'L',
        parts: PartsFactory.build(road_config))

road_bike.spares
# -. [#<OpenStruct PartsFactory::Part name="chain", etc ...

mountain_bike =
    Bicycle.new(
        size: 'L',
        parts: PartsFactory.build(mountain_config))

mountain_bike.spares
# -> [#<OpenStruct PartsFactory::Part name="chain", etc ...
```

* 새로운 자전거 만들기: 리컴벤트 자전거

```ruby
recumbent_config =
    [['chain', '9-speed'],
     ['tire_size', '28'],
     ['flag', 'tall and orange']]

recumbent_bike =
    Bicycle.new(
        size: 'L',
        parts: PartsFactory.build(recumbent_config))

recumbent_bike.spares
# -> [#<OpenStruct PartFactory::Part
#         name="chain",
#         description="9-speed",
#         needs_spare=true>,
#     #<OpenStruct PartFactory::Part
#         name="tire_size",
#         description="28",
#         needs_spare=true>,
#     #<OpenStruct PartFactory::Part
#         name="flag",
#         description="tall and orange",
#         needs_spare=true>]
```

## 9장 비용-효율적인 테스트 디자인하기

* 수정하기 쉬운 코드를 작성하는 일은 예술적인 작업이며 세 가지 기술이 필요하다.
  * 첫째, 객체지향 디자인을 이해하고 있어야 한다.
    * 쉽게 바꿀 수 있는 코드가 곧 잘 디자인된 코드이다.
  * 둘째, 코드를 리팩터링하는 법을 익혀야 한다.
    * 리팩터링은 소프트웨어 시스템을 수정하는 과정이다. 이 과정은 코드의 외적인 작동방식을 변경하지 않으면서도, 그 내부 구조를 발전시킨다.
  * 마지막으로, 수정 가능한 코드를 작성하려면 높은 수준의 테스트를 짤 수 있어야 한다. 테스트는 지속적인 리팩터링에 안정감과 확신을 준다.
* 테스트를 통해 좋은 가치를 얻기 위해서는 테스트의 의도를 명확히 하는 것, 무엇을 언제 그리고 어떻게 테스트를 해야 할지 알아야 한다.
* **테스트 의도를 알기**
  * `버그 찾아내기`
    * 개발 초기 단계에서 버그를 찾아내면 큰 이득을 얻을 수 있다.
  * `문서를 제공하기`
    * 테스트만이 디자인에 대한 믿을 수 있는 문서를 제공한다.
    * 미래의 우리가 기억상실증에 걸릴 것이라 예상하고 테스트를 작성하자. 우리가 언젠가는 잊게 된다는 사실을 기억하자. 한때 우리가 알고 있던 이야기를 다시 들려줄 수 있는 테스트를 작성하자.
  * `디자인 결정을 미루기`
    * 테스트는 디자인 결정을 안전하게 미룰 수 있도록 해준다.
    * 언젠가는 구체적인 여러 경우를 하나로 추상화하는 코드를 만들겠지만 지금은 이 추상화를 그려내기 위한 충분한 정보를 가지고 있지 않다.
    * 의도적으로 인터페이스에 의존하는 테스트를 작성하면 아무런 대가를 치르지 않고도 안전하게 디자인 결정을 미룰 수 있다.
  * `추상화를 돕기`
    * 드디어 새로운 정보를 얻었고 이제 디자인 결정을 내려야 하는 시점이 왔을 때 우리의 작업은 코드의 추상화 정도(level)를 높이게 된다.
    * 추상화된 코드는 아주 유연한 디자인 요소지만, 디자인이 발전하기 위해서는 하나의 작은 대가를 지불해야만 한다. 그 대가란 '추상화된 코드 각각은 이해하기 쉽지만 코드 속에 전체의 작동을 명확하게 보여주는 지점이 없다'는 것이다.
  * `디자인의 결점 드러내기`
    * 테스트의 또 다른 이점은 디자인의 결정을 드러내 준다는 점이다. 테스트를 작성하기 위한 준비 작업이 너무 힘겹다면 코드에 너무 많은 맥락(context)이 있다는 뜻이다.
    * 테스트는 탄관 속의 카나리아 같은 존재다. 디자인이 나쁠 때 테스트는 힘들어진다.
* 대부분의 프로그래머들은 테스트를 너무 많이 짠다.
* 테스트에서 더 나은 가치를 얻기 위한 방법 중 하나는 테스트를 덜 짜는 것이다.
* 자신의 밖으로 나가는 메시지의 상태를 테스트할 필요도 없고 테스트해서도 안 된다. 객체는 오직 자신의 퍼블릭 인터페이스에 속하는 메시지의 상태만 검증해야 한다.
* 들어오는 메시지에 대해서는 메시지가 반환하는 상태를 테스트한다. 밖으로 나가는 커맨드 메시지에 대해서는 이 메시지가 제대로 전송되었는지 테스트해야 한다.
* 테스트를 먼저 작성하는 것이 좋다.
* 불행히도 초보 디자이너가 테스트를 먼저 작성해도 좋은 상황인지 아닌지를 판단하는 일은 쉽지 않기 때문에 이런 조언은 별 도움이 안 된다.
* 아직 훈련이 덜 되었기 때문에 테스트를 먼저 작성하는 것이 당황스럽고 힘들겠지만 꾸준히 수련한다면 언젠가는 테스트할 수 있는 코드를 작성할 수 있게 될 것이며 이는 테스트 작성 훈련을 통해서만 얻을 수 있다.
* 만약 이 책을 읽는 독자가 초보 디자이너이고 지나치게 복잡안 애플리케이션에 맞닥뜨린 상황에 처해있다면 테스트의 가치를 계속 믿는 것이 중요하다.
* 테스트는 꼭 필요하다. 잘 디자인된 애플리케이션은 매우 추상적이고, 계속 변경된다. 테스트가 없다면 이해할 수도 없고 안전하게 수정할 수도 없을 것이다. 최상의 테스트는 실제 코드와 느슨하게 결합되어 있어야 한다. 그리고 모든 코드를 한 번만, 제대로 된 장소에서 테스트해야 한다. 이런 테스트는 코드 작성 비용을 높이지 않으면서도 새로운 가치를 제공한다.
* 잘 디자인된 애플리케이션이 섬세하게 다듬어진 테스트 묶음을 가지고 있다면 이 애플리케인션은 바라보기만 해도 기쁘고 확장하는 작업도 즐겁다. 모든 새로운 상황에 적응할 수 있으며 예상치 못했던 그 어떤 요구사항에도 대처할 수 있다.

**역할을 문서화하기 위한 테스트**

```ruby
module DiameterizableInterfaceTest
    def test_implements_the_diameterizable_interface
        assert_respond_to(@object, :width)
    end
end

class WheelTest < MiniTest::Unit::TestCase
    include DiameterizableInterfaceTest

    def setup
        @wheel = @object = Wheel.new(26, 1.5)
    end

    def test_calculates_diameter
        # . . .
    end
end
```

**테스트 더블(Test Double) 또는 가짜 객체 주입하여 의존성 끊기와 테스트 더블이 인터페이스를 따르는지 검증**

```ruby
class DiameterDouble
    def diameter
        10
    end
end

# 테스트 더블이 올바른 인터페이스를 따르고 있는지 검증한다.
class DiameterDoubleTest < MiniTest::Unit::TestCase
    include DiameterizableInterfaceTest

    def setup
        @object = DiameterDouble.new
    end
end

class GearTest < MiniTest::Unit::TestCase
    def test_calculates_gear_inches
        gear = Gear.new(
            chainring: 52,
            cog: 11,
            wheel: DiamterDouble.new)

        assert_in_delta(47.27,
                        gear.gear_inches,
                        0.01)
    end
end
```

**상속 받은 코드 테스트하기**

```ruby
module BicycleInterfaceTest
    def test_responds_to_defualt_tire_size
        assert_respond_to(@object, :default_tire_size)
    end

    def test_responds_to_default_chain
        assert_respond_to(@object, :default_chain)
    end

    def test_responds_to_chain
        assert_respond_to(@object, :chain)
    end

    def test_responds_to_size
        assert_respond_to(@object, :size)
    end

    def test_responds_to_tire_size
        assert_respond_to(@object, :tire_size)
    end

    def test_responds_to_spares
        assert_repond_to(@ojbect, :spares)
    end
end

class BicycleTest < MiniTest::Unit:TestCase
    include BicycleInterfaceTest

    def setup
        @bike = @object = Bicycle.new({tire_size: 0})
    end

    # 상위클래스의 요구사항 검증하기
    def test_forces_subclasses_to_implement_default_tire_size
        assert_raises(NotImplementedError) {@bike.default_tire_size}
    end
end

class RoadBikeTest < MiniTest::Unit::TestCase
    include BicycleInterfaceTest

    def setup
        @bike = @object = RoadBike.new(tape_color: 'red')
    end

    # 구체적인 하위 클래스의 행동 테스트하기
    def test_puts_tape_color_in_local_spares
        assert_equal 'red', @bike.local_spares[:tape_color]
    end
end
```

**하위 클래스의 책임 명확히 하기**

```ruby
module BicycleSubclassTest
    def test_responds_to_post_initialize
        assert_respond_to(@object, :post_initialize)
    end

    def test_responds_to_local_spares
        assert_respond_to(@object, :local_spares)
    end

    def test_responds_to_default_tire_size
        assert_respond_to(@object, :default_tire_size)
    end
end

class RoadBikeTest < MiniTest::Unit::TestCase
    include BicycleInterfaceTest
    include BicycleSubclassTest

    def setup
        @bike = @object = RoadBike.new
    end
end

class MountainBikeTest < MiniTest::Unit::TestCase
    include BicycleInterfaceTest
    include BicycleSubclassTest

    def setup
        @bike = @object = MountainBike.new
    end
end
```

**추상화된 상위클래스의 행동 테스트하기**

```ruby
class StubbedBike < Bicycle
    def default_tire_size
        0
    end

    def local_spares
        {saddle: 'painful'}
    end
end

class BicycleTest < MiniTest::Unit::TestCase
    include BicycleInterfaceTest

    def setup
        @bike = @object = Bicycle.new({tire_size: 0})
        @stubbed_bike = StubbedBike.new
    end

    # 상위클래스의 요구사항 검증하기
    def test_forces_subclasses_to_implement_default_tire_size
        assert_raises(NotImplementedError) {@bike.default_tire_size}
    end

    def test_includes_local_spares_in_spares
        assert_equal @stubbed_bike.spares,
                    { tire_size: 0,
                      chain: '10-speed',
                      saddle: 'painful' }
    end
end

# 테스트 더블이 이 테스트가 요구하는 인터페이스를 충실히 따르고 있다는 것을 확인한다.
class StubbedBikeTest < MiniTest::Unit::TestCase
    include BicycleSubclassTest

    def setup
        @object = StubbedBike.new
    end
end
```