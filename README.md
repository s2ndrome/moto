# NINE 캐릭터 카드

`index.html` 하나로 이루어진 페이지입니다. GitHub에서 이 파일을 열고 연필(✎) 아이콘을 눌러 바로 수정할 수 있어요.

## 텍스트 수정

`<!-- 이름 -->`, `<!-- 외형 -->`, `[성격]`, `[OFF TRACK]` 등 주석이 달린 부분을 찾아 안의 글자만 바꾸면 됩니다.

## 사진 교체

- **메인 프로필 사진**: `<!-- 메인 프로필 사진 -->` 바로 아래 `<img src="...">`의 주소를 원하는 이미지 주소로 바꾸세요.
- 이미지는 [postimg.cc](https://postimg.cc/) 같은 무료 이미지 호스팅에 올린 뒤 "직접 링크(Direct link)" 주소를 복사해서 붙여넣으면 됩니다. 이 저장소의 `img/` 폴더에 파일을 올리고 `img/파일명.png`처럼 상대 경로로 넣어도 됩니다.

## 스티커 위치/크기/회전 조절

스티커는 총 4장이고, 각각 `<!-- 스티커 1 : 왼쪽 위 -->`처럼 주석으로 표시되어 있습니다. `src`로 사진을 바꾸고, `style=""` 안의 값을 아래처럼 조절하세요.

```html
<img class="ninecard-sticker" src="여기에 이미지 주소"
     style="top: -18px; left: -8px; width: 100px; transform: rotate(-12deg);">
```

- `top` / `left` / `right` / `bottom`: 위치(px). 왼쪽 스티커는 `left`를, 오른쪽 스티커는 `right`를 씁니다. 위쪽은 `top`, 아래쪽은 `bottom`. 숫자가 음수(-)일수록 카드 바깥쪽으로 더 튀어나옵니다.
- `width`: 스티커 크기.
- `transform: rotate(각도deg)`: 회전 각도. 마이너스는 반시계 방향, 플러스는 시계 방향입니다.

## GitHub Pages로 공개하기

저장소 **Settings → Pages**에서 Source를 `main` 브랜치, 폴더는 `/ (root)`로 설정하면 `index.html`이 웹페이지로 바로 열립니다.
