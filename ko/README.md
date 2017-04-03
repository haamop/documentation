# Mautic 문서

### 소개
이 서적은 오픈 소스 마케팅 자동화 시스템인 [Mautic을 위한 문서](https://www.mautic.org/docs/index.html)이다. 누구나 이 정보를 개선하고 필요한 부분을 변경할 수 있습니다.

### PDF로 다운로드

이 문서들을 PDF 로 다운로드 하려면, [여기를 클릭](https://mautic.org/docs/mautic_docs_en.pdf) 하십시오.

### 문서의 배포

이 저장소는 [www.mautic.org/docs](https://www.mautic.org/docs/index.html)에 게시된 Gitbook의 소스 코드입니다. 소스 코드는 GitHub에서 공유되므로 실제 Mautic 코드를 사용하는 프로그래머와 같은 방식으로 누구나 문서 작성에 기여할 수 있습니다.

#### 문서에서 git 을 사용한 이유

- *버전*. 누구나 변경된 내역을 볼 수 있습니다.
- *원작자*. 모든 파일뿐만이 아니라, 모든 라인의 원작자가 작성한 내용을 볼 수 있습니다.
- *커뮤니티 배포자*. 같은 문서에서 작업하는 동안 다른 사람이 작업하다 삭제하는 것에 대해 걱정할 필요가 없습니다.

변경 사항을 복제, 수정, 커밋 및 푸시하는데 필요한 일부 지식이 필요하지만, GitHub 웹 인터페이스를 통해 직접 파일을 편집하는 방법이 있습니다. git을 알고 있으면 원하는 워크 플로우를 사용할 수 있습니다. 그렇지 않은 경우에도 가이드를 따라하면 쉽게 기여할 수 있는 방법이 제공됩니다.

#### 브라우저에서 문서 편집

1. [Fork](https://github.com/mautic/documentation#fork-destination-box) 귀하의 계정에 있는 저장소이므로 직접 편집할 수 있는 권한이 있습니다.
2. 편집할 파일을 선택하십시오. 파일 구조는 아래에 설명되어 있습니다. *README.md* 파일을 클릭하여 편집할 수 있습니다.
3. *README.md* 파일의 내용이 보이고, *편집* 버튼(연필 아이콘)을 선택하십시오
4. 내용은 [마크다운 마크업](https://daringfireball.net/projects/markdown/)으로 작성되어 있습니다. 매우 간단한 텍스트 기반의 서식입니다.
5. 파일 내용을 변경합니다. 예제에서는 `초기 배포본`을 마지막에 추가합니다.
6. 변경 후에는, 스크롤다운하여 *변경 적용*을 진행합니다. 이 사항은 매우 중요한 사항으로, 변경사항을 저장하고 변경된 사유를 설명할 수 있습니다. 예를 들어서 `테스트 목적으로 라인 추가함`으로 내용을 작성할 수 있습니다.
7. 왜냐하면 GitHub 웹 인터페이스는 git의 모든 기능을 제공하지 않으므로, 원본 상태를 간단하게 변경전의 상태로 복원할 수 있는 쉬운 방법이 없습니다. 또한, 추가한 라인을 지우는 또다른 커밋을 해야 합니다. 이 사항은 이력관리의 혼동이 올 수 있으므로 새로운 지표를 만들어야 합니다. "새로운 브랜치 만들기..."라는 체크박스를 사용할 수 있으며, `{yourusername}-patch-1`가 기본값으로 설정된 것을 `{yourusername}-테스팅` 변경하고 *파일 변경 목적* 을 클릭하여 적용합니다.
8. 이제 기존의 저장소에 있는 내용이 변경되었습니다. 공식 저장소를 변경할 목적이라면, pull request (PR) 을 전송합니다. 리다이렉트가 완료된 후, *Create pull request* 의 제안 내용을 변경하고 클릭하십시오. (테스트용 PR은 전송하지 마세요)
테스트가 완료된 후에는, *브랜치* 섹션으로 이동하고 테스트용 브랜치를 삭제합니다.

#### 파일 구조

이전 섹션에서 *README.md* 에 대해 작업했습니다. 이 파일은 현재 보고있는 내용과 같이 GitHub 저장소의 홈페이지에 표시됩니다. 이 사항은 Mautic 문서와 관련이 없습니다

The *SUMMARY.md* file defines the menu of the documentation. If you'll add a new page to the documentation, you'll have to also add a new line there defining the title and the link to the file. It's pretty straightforward when you'll see the current menu items.

The folders are here to group the topics together. Open for example the *asset* folder. You'll see it has its own *README.md* file. It is the main content when you click on the Asset menu item. The *manage_assets.md* file is a subitem. The *media* subfolder contains all the images used in the *md* files.

#### 링크

간혹 문서내에서 다른 링크로 연결이 필요한 경우가 있습니다. Markdown에서 링크를 표시하시려면 다음과 같습니다:

```
[링크 제목](http://example.com)
```

이렇게하면 절대 URL의 외부 링크가 생성됩니다. 내부 링크를 만들려면 다음과 같이 상대 URL 을 사용하십시오:

```
[단계](./../plugins/integration_test.html)
```
This will link to `plugins/integration_test.html` on the documentation website created from the *md* source file.

#### 이미지

As noted above, the images can be placed in the media subfolders. The images probably isn't possible to upload via the GitHub web interface, but you can upload them to any public URL and link them from there.

```
![alternative text here](http://example.com/images/apple.png "Tooltip text here")
```
Or, if you'd want to display an image already uploaded to the documentation repository, you can use relative path:

```
![alternative text here](/assets/media/assets-newcategory.png "Tooltip text here")
```
