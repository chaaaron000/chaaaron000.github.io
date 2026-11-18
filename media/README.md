# media

포트폴리오(`index.html`)가 쓰는 영상과 이미지.

## 아직 없는 파일 (넣으면 자동으로 나타난다)

아래 이름 그대로 이 폴더에 넣고 푸시하면 페이지가 알아서 보여 준다. 파일이 없는 동안에는 그 자리에 아무것도 보이지 않는다(안내 문구나 빈 상자 없음).

| 파일 | 나타나는 곳 | 내용 | 권장 |
|---|---|---|---|
| `caldera-editor.mp4` | 첫 화면 Caldera 타일(도식 대신), Caldera 섹션 맨 위 큰 영상. 넣으면 본문의 도식 세 장도 함께 숨겨진다 | 레벨 설계 편집기: 2D에서 벽을 고치고 → T로 탑뷰 → Tab으로 1인칭 걸어 들어가기 | 10~15초, 1280px, 소리 없음, 10MB 이하 |
| `perfecther-case-editor.mp4` | PerfectHer "사건 데이터 편집 시스템" 맨 위 큰 영상 | 사건 편집기에서 노드를 고치고 웹 시안에서 바뀐 결과를 보여 주기 | 10초 안팎, 1280px |
| `perfecther-3d-background.png` | PerfectHer "AI 시안 파이프라인" 왼쪽 | Blender MCP로 만든 은신처 3D 배경 | 16:9 |
| `perfecther-title.png` | 첫 화면 PerfectHer 타일(도식 대신), "AI 시안 파이프라인" 오른쪽 | 3D 배경 + 캐릭터를 합성한 타이틀 화면 | 16:9 |

## 지금 쓰는 파일

크래프톤 제출 덱에서 꺼낸 자산이다. 이름을 바꾸면 `index.html`의 경로도 같이 바꿔야 한다.

| 파일 | 쓰는 곳 | 내용 |
|---|---|---|
| `beyond-prototype.mp4` | 화면 건너편의 너 머리 옆 영상 | 웹 프로토타입 플레이 39초 |
| `beyond-prototype-poster.jpg` | 위 영상의 대기 화면 | 프로토타입 대화 장면 |
| `beyond-inspector-before.png` | 미션 커스텀 인스펙터 Before를 누르면 열리는 원본 | 기본 Inspector(Debug 모드) |
| `beyond-inspector-after.png` | 미션 커스텀 인스펙터 After를 누르면 열리는 원본, 첫 화면 타일 | 미션 커스텀 Inspector |
| `beyond-inspector-before-crop.png`, `beyond-inspector-after-crop.png` | 미션 커스텀 인스펙터 Before, After | 위 두 원본의 왼쪽 위 780×330을 잘라 낸 것. 본문에서 글자가 읽히도록 잘랐다 |
| `greenclean-play.jpg` | 반응 영상 대기 화면(본문, 첫 화면 타일) | 3콤보 마스코트 반응 장면 |
| `greenclean-play-board.jpg` | GreenClean YouTube 대기 화면 | 반응 영상 0.4초 지점의 장면(말풍선이 뜨기 전 플레이 화면) |
| `greenclean-reaction.mp4` | 반응 테이블 에디터 "결과", 첫 화면 타일 | 3콤보 마스코트 반응 7초 |
| `greenclean-editor.jpg` | 반응 테이블 에디터 "데이터" | 반응 테이블 에디터 인스펙터 (덱 캡처에서 여백을 잘라 냄) |
| `mixterpiece-play.mp4` | MixterPiece 머리 옆 영상 | 웹 빌드 플레이 58초. 덱 원본에서 앞의 정지 타이틀 3.28초를 잘라 냈다 |
| `mixterpiece-play-poster.jpg` | 위 영상의 대기 화면 | 플레이 장면 |
| `mixterpiece-wall-editor.jpg` | 벽 시스템과 벽 에디터 "에디터" | Wall Editor, Answer Editor 인스펙터 (덱 캡처의 왼쪽 절반) |
| `mixterpiece-wall-result.jpg` | 벽 시스템과 벽 에디터 "결과" | 벽이 배치된 게임 화면 (덱 캡처의 오른쪽 절반) |
| `mixterpiece-wall-stage.jpg` | 첫 화면 타일 | 벽 스테이지 플레이 화면 |
| `nostalgia-keyart.jpg` | 첫 화면 타일 | Steam 대표 이미지 |
| `nostalgia-play-1.jpg`, `nostalgia-play-2.jpg` | Nostalgia 대표 이미지 두 장 | 플레이 화면 |
| `og.jpg` | 링크 미리보기(`og:image`) | 네 게임 화면을 1200×630으로 합친 이미지 |

## 지금은 쓰지 않는 파일

페이지 길이를 줄이면서 본문에서 뺐다. 파일은 그대로 두었고, 다시 쓰려면 `index.html`에 넣으면 된다.

| 파일 | 내용 |
|---|---|
| `beyond-prototype-briefing.jpg` | 웹 프로토타입의 조사 브리핑 화면 |
| `mixterpiece-settings.jpg` | 설정 화면 (오디오, 접근성) |

## 참고

- 로컬에서 볼 때는 저장소 루트에서 `python -m http.server`로 띄운다. `file://`로 열면 "아직 없는 파일" 확인이 막혀, 파일을 넣어도 나타나지 않는다.
- "아직 없는 파일"은 페이지가 열릴 때 있는지 한 번씩 확인한다. 그래서 파일이 없는 동안에는 브라우저 개발자 도구 콘솔에 404가 네 줄 찍힌다. 화면에는 영향이 없고, 파일을 넣으면 사라진다.
- 영상은 GitHub 저장소 용량을 생각해 짧고 가볍게 줄인다. 예: `ffmpeg -i in.mp4 -vf scale=1280:-2 -an -c:v libx264 -crf 28 -preset veryfast -movflags +faststart out.mp4`
