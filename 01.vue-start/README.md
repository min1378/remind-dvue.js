# 01. Vue Start

## 1. hellovuejs 분석
```html
<!DOCTYPE html>
<html lang="ko">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Hello vue.js</title>
    <script src="https://unpkg.com/vue@2.5.16/dist/vue.js"></script>
</head>

<body>
    <div id="simple">
        <h2>{{message}}</h2>
    </div>
    <script type="text/javascript">
        // 모델 객체이다. 데이터를 가지고 있다.
        var model = {
            message: '첫 번째 Vue.js 앱입니다.'
        };
        // Vue 객체이자 ViewModel 객체. Vue 객체는 HTML 요소와 데이터를 참조하고 있다.
        // data가 변경되면 ViewModel 객체는 즉시 HTML 요소에 반영시킨다.
        var simple = new Vue({
            // el 속성은 HTML요소(Element)
            el: '#simple',
            // data 속성은 모델 객체를 참조한다.
            data: model
        })
    </script>
</body>

</html>
```

- HTML 요소에서는 {{ }} 템플릿 표현식을 사용해 HTML DOM에 데이터를 렌더링 한다.

- 콧수염 모양을 닮았다고 해 콧수염 표현식(Mustache Expression), 문자열을 덧붙인다는 의미로 보간법(Interpolation) 이라 한다.

- Model을 변경하면 ViewModel 객체를 통해 HTML DOM이 즉시 변경된다.

 ![MVVM패턴] (./images/MVVM 패턴.png)





