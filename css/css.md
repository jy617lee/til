# css

## position

- static : 일단 모든 태그들은 처음에 position: static 상태. 차례대로 왼쪽에서 오른쪽, 위에서 아래로 쌓입니다.

- relative :  기존 static이었을 때의 위치를 기준으로 top, right, bottom, left 방향으로 주어진 픽셀만큼 이동



## display

`display` 속성은 요소를 어떻게 보여줄지를 결정합니다.주로 4가지 속성값이 쓰이는데, 태그마다 기본값이 다름

- `none` : 보이지 않음

- `block` : 블록 박스. `width`, `height` 속성을 지정 할 수 있으며, block 요소 뒤에 등장하는 태그가 그 이전 block 요소에 오른쪽에 배치될 수 있어도 **항상 다음 줄**에 렌더링

- `inline` : 인라인 박스. `block` 과 달리 줄 바꿈이 되지 않고, `width`와 `height`를 지정 할 수 없습니다. word 같은 문서에서 볼드, 이탤릭, 색상, 밑줄 등 **글자나 문장에 효과를 주기 위해 존재하는 단위**

- `inline-block` : block과 inline의 중간 형태

- ### display:flex

  블록 레이아웃, 인라인 레이아웃, 테이블 레이아웃 및 위치 지정 레이아웃 모드와 더불어 CSS3에서는 보다 복잡한 블록 타입 레이아웃 모드인 flexbox 레이아웃을 지원한다. flexbox의 콘텐츠는 어떤 방향에든 위치할 수 있으며, 동적으로 변경가능한 순서를 지정할 수도 있고, 가용한 공간 내에서 크기와 위치를 자동으로 조정하기도 한다.

## 들여쓰기
- ul에 list-style-position을 outside로 주기



- document.URL 로 현재 url 가져올 수 있다. (window.으로 가져오면 firefox에서 오류가 난다고 함)