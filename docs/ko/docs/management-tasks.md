FastAPI 저장소 관리 작업
여기 팀 멤버{.internal-link target=_blank}가 FastAPI 저장소를 관리하기 위해 수행할 수 있는 작업들이 있습니다.

/// tip

이 섹션은 저장소 관리 권한이 있는 팀 멤버에게만 유용합니다. 따라서 건너뛰어도 괜찮습니다. 😉

///

...그래서, 당신은 FastAPI 팀의 멤버{.internal-link target=_blank}인가요? 와우, 정말 멋지네요! 😎

당신은 외부 기여자와 동일한 방법으로 Help FastAPI - 도움 받기{.internal-link target=_blank}에 기여할 수 있습니다. 하지만 추가로, 팀 멤버로서만 수행할 수 있는 몇 가지 작업이 있습니다.

여기에서 당신이 수행할 수 있는 작업들에 대한 일반 지침을 제공합니다.

정말 감사드립니다. 🙇

친절하세요
가장 먼저, 친절해야 합니다. 😊

당신이 팀에 추가되었다면 아마도 이미 매우 친절한 분일 가능성이 크지만, 그래도 언급할 가치가 있습니다. 🤓

상황이 어려울 때
상황이 좋을 때는 모든 것이 더 쉬우므로 별다른 지침이 필요하지 않습니다. 그러나 상황이 어려울 때는 몇 가지 지침이 있습니다.

긍정적인 면을 찾아보세요. 사람들이 불친절하지 않다면, 그들의 노력과 관심에 감사하라는 것이 기본적인 자세입니다. 심지어 논의나 PR에 동의하지 않더라도 프로젝트에 대한 관심과 어떤 일을 시도해보려는 시간과 노력을 감사하게 여겨야 합니다.

텍스트로 감정을 전달하는 것은 어려우므로 이모티콘을 활용해보세요. 😅

토론이나 PR에서 많은 경우, 사람들은 자신의 좌절감을 여과 없이 표현하고 과장하거나 불평을 하거나 당연한 듯한 태도를 보입니다. 이런 경우는 좋지 않으며, 그들의 문제를 해결하는 우리의 우선순위를 낮춥니다. 그래도 숨을 고르고 부드럽게 답변하는 것이 중요합니다.

쓴소리나 잠재적으로 수동적 공격성으로 보일 수 있는 댓글을 피하세요. 문제가 있다면 직접적으로 (되도록 부드럽게) 말하는 것이 좋습니다.

가능한 한 구체적이고 객관적으로 말하려고 노력하세요. 일반화를 피하세요.

더 어려운 대화를 해야 하는 경우, 예를 들어 PR을 거절해야 하는 상황에서는, 저에게 (@tiangolo) 직접 처리해 달라고 요청할 수 있습니다.

PR 제목 수정
PR 제목을 <a href="https://gitmoji.dev/" class="external-link" target="_blank">gitmoji</a>의 이모티콘으로 시작하도록 수정하세요.
GitHub 코드 대신 이모티콘 문자를 사용하세요. 예를 들어 :bug: 대신 🐛을 사용하세요. 이렇게 하면 GitHub 외부에서도 제대로 표시됩니다. 예를 들어 릴리스 노트에서도 제대로 나타납니다.
번역 PR에는 🌐 이모티콘(“지구본”)을 사용하세요.
제목은 동사로 시작하세요. 예를 들어 Add, Refactor, Fix 등을 사용하세요. 이렇게 하면 PR이 수행하는 작업을 설명하게 됩니다. 예를 들어 TeleportAdapter 클래스 생성 대신 텔레포팅 지원 추가와 같이 기술합니다.
제목은 명령형으로 작성하세요. 예를 들어 텔레포팅 지원을 추가 대신 텔레포팅 지원 추가라고 합니다.
제목이 PR의 목적을 잘 설명하도록 하세요. 기능일 경우, 텔레포팅 지원 추가와 같이 구체적으로 설명하고, TeleportAdapter 클래스 생성과 같이 추상적으로 쓰지 않도록 합니다.
제목 끝에 마침표(.)를 쓰지 마세요.
번역 PR의 경우 🌐로 시작한 후 Add {언어} translation for과 그 후에 번역된 파일 경로를 기술하세요. 예를 들어:
Markdown
코드 복사
🌐 Add Spanish translation for `docs/es/docs/teleporting.md`
PR이 병합되면, GitHub 액션(<a href="https://github.com/tiangolo/latest-changes" class="external-link" target="_blank">latest-changes</a>)이 PR 제목을 사용해 자동으로 최신 변경 사항을 업데이트합니다.

따라서 PR 제목을 깔끔하게 작성하면 GitHub뿐만 아니라 릴리스 노트에서도 멋지게 보입니다. 📝

PR에 라벨 추가
동일한 GitHub 액션 <a href="https://github.com/tiangolo/latest-changes" class="external-link" target="_blank">latest-changes</a>가 릴리스 노트에서 PR이 위치할 섹션을 결정하기 위해 PR에 하나의 라벨을 사용합니다.

다음 <a href="https://github.com/tiangolo/latest-changes#using-labels" class="external-link" target="_blank">latest-changes 지원 라벨 목록</a>에 있는 라벨을 사용하세요:

breaking: Breaking Changes
기존 코드가 변경 없이 버전 업데이트 시 깨질 경우. 이 라벨은 자주 사용되지 않습니다.
security: Security Fixes
보안 수정 사항, 예를 들어 취약점. 거의 사용되지 않을 것입니다.
feature: Features
새로운 기능, 기존에 없던 지원을 추가하는 경우.
bug: Fixes
기존 지원이 제대로 작동하지 않는 경우 수정하는 것. 많은 PR이 버그 수정이라고 주장하지만, 실제로는 예상치 못한 방식으로 사용하거나 지원되지 않는 경우가 많습니다. 그러나 실제 버그인 경우도 있습니다.
refactor: Refactors
코드의 내부 변경 사항이지만 동작은 변경되지 않는 경우. 유지 관리 가능성을 향상시키거나 미래 기능을 위한 준비 작업 등.
upgrade: Upgrades
프로젝트의 직접적인 의존성을 업그레이드하는 경우. 예를 들어, pyproject.toml에 있는 내용. 사용자는 버전을 업데이트할 때 이를 받게 됩니다. 하지만 개발, 테스트, 문서 작업을 위한 내부 의존성 업데이트는 internal로 표시해야 합니다.
docs: Docs
문서 변경 사항. 문서 업데이트나 오타 수정이 포함됩니다. 하지만 번역은 포함되지 않습니다.
PR의 "Files changed" 탭에서 업데이트된 파일이 docs/en/docs로 시작하는지 확인해 빠르게 감지할 수 있습니다. 문서의 원본 버전은 항상 영어로, docs/en/docs에 있습니다.
lang-all: Translations
번역에 사용합니다. PR의 "Files changed" 탭에서 업데이트된 파일이 docs/{lang}/docs로 시작하는지 확인하세요. 예를 들어 docs/es/docs 등입니다.
internal: Internal
저장소 관리에만 영향을 미치는 변경 사항에 사용합니다. 예를 들어 내부 의존성 업그레이드, GitHub Actions 또는 스크립트 변경 등이 있습니다.
/// tip

Dependabot과 같은 도구는 dependencies와 같은 라벨을 추가할 수 있지만, 이 라벨은 latest-changes GitHub 액션에서 사용되지 않으므로 릴리스 노트에서 사용되지 않습니다. 위에 언급한 라벨 중 하나가 추가되었는지 확인하세요.

///

번역 PR에 라벨 추가
번역에 대한 PR이 있는 경우, lang-all 라벨을 추가하는 것 외에도 해당 언어에 대한 라벨을 추가하세요.

언어 코드로 된 라벨이 있어야 하며, 예를 들어 스페인어의 경우 lang-es, 프랑스어의 경우 lang-fr과 같습니다.

해당 언어의 라벨을 추가하세요.
awaiting-review 라벨을 추가하세요.
awaiting-review 라벨은 번역에만 사용됩니다. GitHub 액션이 이를 감지하고 언어 라벨을 읽은 다음, 해당 언어에 대한 GitHub Discussions를 업데이트해 새 번역 검토가 필요함을 알립니다.

원어민이 검토하고 승인하면, GitHub 액션이 자동으로 awaiting-review 라벨을 제거하고 approved-1 라벨을 추가합니다.

이렇게 하면 approved-1 라벨이 있는 새 번역이 준비되었는지 확인할 수 있습니다.

번역 PR 병합
스페인어의 경우, 제가 원어민이므로 직접 최종 검토를 하고 대부분의 경우 병합하기 전에 약간의 수정을 할 것입니다.

다른 언어의 경우에는 다음을 확인하세요:

제목이 위 지침을 따르고 있는지 확인하세요.
lang-all과 lang-{언어 코드} 라벨이 있는지 확인하세요.
PR이 하나의 Markdown 파일에서 번역만 추가하는지 확인하세요.
또는 일부 경우, 같은 언어로 검토된 파일이 2개 이하인 경우.
해당 언어의 첫 번째 번역인 경우, 추가적인 mkdocs.yml 파일도 포함될 수 있습니다. 이 경우 아래 지침을 따르세요.
PR이 추가 파일이나 불필요한 파일을 추가하지 않는지 확인하세요.
번역이 원래의 영어 파일과 비슷한 구조를 가지고 있는지 확인하세요.
번역이 원래 콘텐츠를 변경하지 않는지 확인하세요. 예를 들어 명백히 추가적인 문서 섹션이 포함되지 않는지 확인합니다.
번역이 원래와 다른 Markdown 구조를 사용하지 않는지 확인하세요. 예를 들어, 원래는 없던 HTML 태그를 추가하지 않도록 합니다.
"admonition" 섹션, 예를 들어 tip, info 등이 번역되었는지 여부를 확인하세요. 예를 들어:
arduino
코드 복사
/// tip

이것은 팁입니다.

///

는 다음과 같이 보입니다:

/// tip

이것은 팁입니다.

///

...하지만 이것을 번역할 경우 정확한 tip 키워드를 유지해야 합니다. consejo로 번역된 경우:

arduino
코드 복사
/// consejo

이것은 팁입니다.

///

스타일이 기본으로 변경되어 다음과 같이 보입니다:

/// consejo

이것은 팁입니다.

///

이들은 번역할 필요는 없지만, 번역된 경우 다음과 같이 작성되어야 합니다:

arduino
코드 복사
/// tip | "consejo"

이것은 팁입니다.

///

이렇게 보입니다:

/// tip | "consejo"

이것은 팁입니다.

///

첫 번역 PR
언어에 대한 첫 번째 번역이 있는 경우, docs/{언어 코드}/docs/index.md 번역 파일과 docs/{언어 코드}/mkdocs.yml 파일이 포함될 것입니다.

예를 들어, 보스니아어의 경우:

docs/bs/docs/index.md
docs/bs/mkdocs.yml
mkdocs.yml 파일에는 다음 내용만 있을 것입니다:

YAML
코드 복사
INHERIT: ../en/mkdocs.yml
언어 코드는 보통 <a href="https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes" class="external-link" target="_blank">ISO 639-1 언어 코드 목록</a>에 있습니다.

어쨌든, 언어 코드는 <a href="https://github.com/fastapi/fastapi/blob/master/docs/language_names.yml" class="external-link" target=_blank>docs/language_names.yml</a> 파일에 있어야 합니다.

언어 코드에 대한 라벨이 아직 없을 것입니다. 예를 들어, 보스니아어의 경우 lang-bs가 없을 것입니다. 라벨을 생성하고 PR에 추가하기 전에 GitHub Discussion을 생성하세요:

<a href="https://github.com/fastapi/fastapi/discussions/categories/translations" class="external-link" target=_blank>번역 GitHub Discussions</a>로 이동하세요.
Bosnian Translations (혹은 영어로 된 해당 언어 이름) 제목으로 새 토론을 생성하세요.
다음과 같은 설명을 작성하세요:
Markdown
코드 복사
## Bosnian translations

이것은 보스니아어 문서 번역을 추적하기 위한 이슈입니다. 🚀

여기에 [라벨 `lang-bs`가 붙은 리뷰 대기 PR](https://github.com/fastapi/fastapi/pulls?q=is%3Apr+is%3Aopen+sort%3Aupdated-desc+label%3Alang-bs+label%3A%22awaiting-review%22)이 있습니다. 🤓
"Bosnian"을 새 언어로 업데이트하세요.

검색 링크를 업데이트하여 lang-bs와 같은 새 언어 라벨을 가리키도록 하세요.

그런 다음 PR로 돌아가서 lang-bs, lang-all, awaiting-review 라벨을 추가하세요.

이제 GitHub 액션이 자동으로 lang-bs 라벨을 감지하고 이 PR이 검토 대기 중임을 알리기 위해 해당 토론에 게시할 것입니다.

PR 검토
PR이 무엇을 하거나 왜 필요한지 설명하지 않는 경우, 추가 정보를 요청하세요.

PR은 해결하려는 구체적인 사용 사례가 있어야 합니다.

기능을 위한 PR일 경우, 문서가 있어야 합니다.
사용하지 않도록 권장하고 싶은 기능(예: 사용하지 않도록 권장하는 코너 케이스 지원)일 경우는 예외입니다.
문서에는 소스 예제 파일이 포함되어야 하며, 직접 Markdown에 Python 코드를 작성하지 않아야 합니다.
소스 예제가 Python 3.8, 3.9, 3.10에 대해 다른 구문을 가질 수 있다면, 파일의 다른 버전이 있어야 하며, 탭으로 구분해 문서에 표시해야 합니다.
소스 예제를 테스트하는 테스트가 있어야 합니다.
PR을 적용하기 전에 새 테스트는 실패해야 합니다.
PR을 적용한 후 새 테스트는 통과해야 합니다.
커버리지는 100%를 유지해야 합니다.
PR이 합리적으로 보이거나 우리가 논의한 후 수락해야 한다고 생각하면, PR에 커밋을 추가하여 문서, 테스트, 형식 등을 수정하거나 불필요한 파일을 제거할 수 있습니다.
PR에서 더 많은 정보를 요청하거나 변경 사항을 제안하기 위해 자유롭게 댓글을 남길 수 있습니다.
PR이 준비되었다고 생각되면, 제가 검토할 수 있도록 내부 GitHub 프로젝트에서 이동하세요.
FastAPI People PR
매달 GitHub 액션이 FastAPI People 데이터를 업데이트합니다. 이러한 PR은 다음과 같습니다: <a href="https://github.com/fastapi/fastapi/pull/11669" class="external-link" target=_blank>👥 Update FastAPI People</a>.

테스트가 통과되면 바로 병합할 수 있습니다.

외부 링크 PR
사람들이 외부 링크를 추가할 때, 이 파일을 편집합니다: <a href="https://github.com/fastapi/fastapi/blob/master/docs/en/data/external_links.yml" class="external-link" target=_blank>external_links.yml</a>.

새 링크가 올바른 카테고리(예: "Podcasts") 및 언어(예: "Japanese")에 있는지 확인하세요.
새 링크는 해당 목록의 맨 위에 있어야 합니다.
링크 URL이 작동해야 합니다(404 오류를 반환하지 않아야 합니다).
링크의 내용이 FastAPI에 관한 것이어야 합니다.
새 항목에는 다음 필드가 있어야 합니다:
author: 저자의 이름.
link: 콘텐츠가 있는 URL.
title: 링크의 제목(기사, 팟캐스트 등의 제목).
이 모든 사항을 확인하고 PR에 적절한 라벨이 있는지 확인한 후 병합할 수 있습니다.

Dependabot PR
Dependabot은 여러 항목에 대한 의존성 업데이트 PR을 생성합니다. 이 PR들은 모두 비슷해 보이지만, 일부는 더 민감한 경우도 있습니다.

PR이 직접적인 의존성에 대한 것이면, 즉 Dependabot이 pyproject.toml을 수정하고 있다면, 병합하지 마세요. 😱 먼저 제가 확인해야 합니다. 추가 수정이나 업데이트가 필요할 가능성이 높습니다.
PR이 내부 의존성 업데이트(예: requirements.txt 파일 수정 또는 GitHub Actions 버전 수정)라면, 테스트가 통과되고 PR에 표시된 릴리스 노트 요약에 명백한 잠재적 중대한 변경 사항이 없다면, 병합할 수 있습니다. 😎
GitHub Discussions 답변 표시
GitHub Discussions에서 질문에 답변이 달리면, "Mark as answer" 버튼을 클릭하여 답변을 표시하세요.

다음에서 토론을 필터링할 수 있습니다: <a href="https://github.com/tiangolo/fastapi/discussions/categories/questions?discussions_q=category:Questions+is:open+is:unanswered" class="external-link" target=_blank">Questions
