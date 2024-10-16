# java-calculator-precourse

> 입력한 문자열에서 숫자를 추출하여 더하는 계산기를 구현한다.

### 기능 구현
아래의 4가지 세부기능을 구현할 기능목록으로 정리함: 
1. 입력 문자열에서 숫자 추출
- 기본 구분자 기준으로 문자열 분리
  <br>기본 구분자인 쉼표 `,` 또는 콜론 `:` 을 구분자로 가지는 문자열을 전달하는 경우 이를 기준으로 문자열을 분리하는 기능
  <br>예: `"" => 0`, `"1,2" => 3`, `"1,2,3" => 6`, `"1,2:3" => 6`
- 커스텀 구분자 기준으로 문자열 분리
  <br>`//`와 `\n`의 사이에 입력되는 구분자를 커스텀 구분자로 지정하며, 이를 기준으로 문자열을 분리하는 기능
  <br>예:`"//;\n1;2;3"`과 같이 값을 입력할 경우 커스텀 구분자는 세미콜론 `;`이며, 결과 값은 6이 반환되어야 함
- 잘못된 입력값 검사
  <br>사용자가 잘못된 값을 입력할 경우 `IllegalArgumentException`을 발생시킨 후 애플리케이션 종료

2. 추출된 숫자를 더하는 계산
- 두 숫자를 더한 후 그 값을 출력예시에 맞추어 출력하는 기능

