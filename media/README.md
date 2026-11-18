# media

포트폴리오(`index.html`)의 `data-media` 자리에 들어갈 파일들. 이 이름으로 이 폴더에 넣으면 페이지가 알아서 영상·이미지로 바꿔 보여 준다. 파일이 없으면 안내 문구가 그대로 남는다.

| 파일 | 내용 | 권장 |
|---|---|---|
| `caldera-editor.mp4` | 레벨 설계 편집기: 2D에서 벽을 고치고 → T로 탑뷰 → Tab으로 1인칭 걸어 들어가기 | 10~15초, 1280px, 소리 없음, 10MB 이하 |
| `perfecther-case-editor.mp4` | 사건 편집기에서 노드를 고치고 웹 시안에서 바뀐 결과를 보여 주기 | 10초 안팎 |
| `perfecther-3d-background.png` | Blender MCP로 만든 은신처 3D 배경 | 16:9 |
| `perfecther-title.png` | 3D 배경 + 캐릭터를 합성한 타이틀 화면 | 16:9 |
| `mission-editor.png` | 「화면 건너편의 너」 Debug 인스펙터와 미션 에디터를 나란히 놓은 비교 (크래프톤 슬라이드 22쪽) | 16:9 |
| `greenclean-editor.jpg` | GreenClean 반응 테이블 에디터 캡처 (크래프톤 슬라이드 8쪽) | 16:9 |
| `mixterpiece-wall-editor.jpg` | MixterPiece Wall Editor와 결과 화면 (크래프톤 슬라이드 16쪽) | 16:10 |

## 참고

- 로컬에서 볼 때는 `python -m http.server`로 띄워야 한다. `file://`로 열면 파일 확인이 막혀 안내 문구만 보인다.
- 영상은 GitHub 저장소 용량을 생각해 짧고 가볍게 줄인다. 예: `ffmpeg -i in.mp4 -vf scale=1280:-2 -an -c:v libx264 -crf 28 -preset veryfast out.mp4`
