태그의 속성에 required 속성을 추가


* 각 요소에 대한 포커스아웃에 대한 단일 액션 수행한다(실시간검사)
* 유효성검사 언어 설정을 제공한다
* 커스텀 검사 기능을 지원한다
* 오류 표시방법  : 실시간 | alert
* 각 유효성 검사에 대한 모듈 분리 작성한다
* 

```javascript
{
  target : 'selecter',//string
  type   : 'number',  //string
  msg    : '{label}항목은 필수입력사항입니다',  //string
  pattern: '//g'      //string정규식
}
```
```html
<input type=text name=username required>
```
