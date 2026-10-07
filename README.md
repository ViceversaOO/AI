> [!IMPORTANT] 내 연구 관점에서의 핵심 takeaway
> 기업의 현금 보유 수준과 향후 1년 주가 수익률의 관계를 연구하기 위한 개인 위키입니다. 원본·지식·관리 규칙을 GitHub에서 보관하고, 컴퓨터에서 복제한 폴더를 Obsidian으로 열어 읽고 수정합니다.

# 나의 경제학 연구 위키

현재 자료는 기업가치·투자를 다룬 논문 두 편이며 미래 주가 수익률의 직접 실증 근거는 아직 확인 필요입니다. 학생 확인 7개·추가 사용 허가 3개·기업가치 논문의 재현성 한계 1개를 기록했습니다.

- [전체 목차](Wiki/index.md) — Wiki 11개 페이지의 출발점.
- [연구계획 초안](research_plan.md) — 연구 질문과 미정 설계 항목.
- [위키 사용법](Wiki/위키-사용법.md) — 자료 넣기·질문하기·건강검진 및 Graph View.
- [관리 규칙](AGENTS.md) — 원본 불변·출처·학생 확인 범위.

## 내 컴퓨터에서 시작하기

1. [GitHub Desktop](https://desktop.github.com)을 설치하고 GitHub 계정으로 로그인합니다.
2. **File → Clone repository → URL**에서 `https://github.com/ViceversaOO/AI.git`를 입력하고 저장할 폴더를 정합니다. `main` 브랜치를 사용합니다.
3. [Obsidian](https://obsidian.md)에서 **Open folder as vault(폴더를 보관함으로 열기)**를 선택해 복제한 `AI` 폴더를 엽니다.
4. `Wiki/index.md`를 열고, 명령 팔레트에서 **Open graph view**를 실행합니다. Windows/Linux는 `Ctrl+P`, macOS는 `Cmd+P`입니다.
5. 그래프 검색에 `path:Wiki`를 넣습니다. 목차·로그를 숨기려면 `path:Wiki -file:index -file:log`를 사용합니다.

터미널을 사용하는 경우 처음 한 번 실행합니다.

```sh
git clone https://github.com/ViceversaOO/AI.git
cd AI
```

GitHub의 **Code → Download ZIP**으로 내려받아 Obsidian에서 열 수도 있습니다. ZIP 사본에는 Git 기록이 없으므로 지속적인 동기화에는 복제를 사용합니다.

## 수정과 동기화

1. 수정 전 GitHub Desktop에서 **Fetch origin**, 원격 변경이 있으면 **Pull origin**을 실행합니다.
2. Obsidian에서 Markdown을 수정·저장합니다. 원본 `Raw/`는 수정·삭제·이동하지 않습니다.
3. GitHub Desktop의 변경 목록을 확인하고 설명을 입력해 **Commit to main**을 누릅니다.
4. **Push origin**으로 GitHub에 저장합니다.
5. Codex의 다음 작업은 이 저장소의 `main`을 기준으로 시작합니다. 진행 중인 클라우드 작업에도 반영하려면 ‘GitHub의 최신 변경을 읽고 이어서 작업해줘’라고 알려주세요.

동시에 같은 파일을 고쳤다면 자동 덮어쓰기 대신 양쪽 내용을 비교해 충돌을 해결합니다. Obsidian 자체가 GitHub에 자동 저장하는 것은 아닙니다. 창 배치·기기별 화면 상태와 생성 ZIP은 `.gitignore`에 따라 버전 관리에서 제외합니다.

## 파일 구성과 출처

`Raw/`는 원본 PDF, `Wiki/`는 연결된 Markdown이며 두 폴더 모두 하위 폴더 없이 관리합니다. `.gitattributes`로 원본의 줄바꿈 변환을 막아 운영체제가 달라도 바이트를 보존합니다. 루트의 `LLM-Wiki-참고원문.txt`는 사용자가 제공한 Karpathy 참고문서의 바이트 보존 사본입니다.

과거 로그의 `../../attachments/...` 링크는 최초 클라우드 첨부 위치를 기록한 것으로 보존했습니다. 복제 후 참고문서를 읽을 때는 [보존 사본](LLM-Wiki-참고원문.txt)을 사용합니다. 이 링크 차이는 연구 원본이나 과거 작업 기록의 변경을 뜻하지 않습니다.

과제 2-3의 연결된 Wiki 작성은 수행했습니다. 다음은 학생의 로컬 Graph View 확인이며, 이후 추가 자료 하나의 Ingest → 여러 문서를 활용하는 Query → 전체 Lint를 진행합니다.
