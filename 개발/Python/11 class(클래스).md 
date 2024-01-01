`class`는 **반복**되**는 메서드(함수), 변수를 모아**두는 것이다

```Python
class chocolate:
    def __init__(self, shape, material):
        self.shape = shape
        self.material = material
        print('이름: {0} {1}초콜릿'.format(self.shape, self.material))


chocolate_strawberry = chocolate('동그란', '딸기')
chocolate_dark = chocolate('네모난', '다크')
chocolate_milk = chocolate('네모난', '밀크')
# 이름: 동그란 딸기초콜릿
# 이름: 네모난 다크초콜릿
# 이름: 네모난 밀크초콜릿
```

## 상속

**다른 클래스의 변수를 사용**하게 해준다

```Python
class Country:
    name = '국가명'
    population = '인구'
    capital = '수도'

    def show(self):
        print('국가 클래스의 메소드입니다.')

class Korea(Country):
    def __init__(self, name):
        self.name = name

    def show_name(self):
        print('국가 이름은: ' + self.name)

kr = Korea('대한민국')
kr.show_name() #국가 이름은: 대한민국
```

---

## **메서드 오버라이딩**