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

1. [Fork](https://github.com/mautic/documentation#fork-destination-box) this repository under your account so you'd have permission to edit.
2. Select a file to edit. The file structure is explained below. Now, let's edit the *README.md* file to show the principles. Click on it.
3. The content of *README.md* should be visible and the *Edit* button (the pencil icon) above as well. Hit it.
4. The content is written in [Markdown markup](https://daringfireball.net/projects/markdown/). Very simple text based formating.
5. Make a change to the file. For example add to the end `This is my first contribution`.
6. When you made a change, scroll down and notice the form called *Commit changes*. This is important. To save a change, you have to describe what you've changed and why. Write for example `A new line added for testing purposes`. Do not save yet!
7. Because the GitHub web interface does not provide all features of git, we won't have an easy way to revert our change back to the original state. We'd have to create another commit where we'd delete the added line. That would make a mess in the commit history. So instead, we create a new branch. There is a checkbox for it "Create a new branch...". The branch has to have a name. `{yourusername}-patch-1` will be prefilled. Let's change it to `{yourusername}-testing`. Click the *Propose file change* now.
8. Ok, so the change exists in your repository now. To propose the change to the official repository, you have to send a pull request (PR). You've been redirected to do just that. Here you describe your proposed change and click (please don't send the testing PRs) the *Create pull request* button.

If you want to clean after the testing, go to the *Branches* section and delete the testing branch.

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
