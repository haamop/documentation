# 연락처

Mautic 1.4.0 버전의 리드가 연락처로 이름이 변경되었습니다

연락처는 마케팅 자동화 플랫폼의 핵심 요소입니다. 이 기능은 웹사이트를 방문하거나 어떤식으로든 귀하와 상호 작용을 한 모든 개인의 정보입니다.

### 연락처 유형

연락처에는 다음과 같은 2가지 유형이 있습니다:
* **방문객** (이전 버전에는 익명의 리드) — 양식 제출이나 다른 상호 작용에 의해서 아직 확인되지 않은 방문자.
  * 이러한 연락처는 Mautic에 의해 추적되지만, 일반적으로 세그먼트의 혼란을 피하기 위해 표시하지 않음.
* **표준 연락처** — 양식 제출 또는 다른 출처를 통해 자신을 식별한 연락처입니다. 결과적으로 이러한 연락처에는 일반적인 이름, 전자메일 및 기타 식별 필드가 포함됨.

#### 방문객 (이전 버전에는 익명의 리드)

Mautic 1.4.0 버전의 익명의 리드가 방문객으로 이름이 변경되었습니다.

You can view visitors by using the 'table view' (use the "t" keyboard shortcut to view contacts in a table or "c" as cards) within the contacts section.

Visitors are worth tracking, because these could be future customers. By tracking them before they have any interaction, you can retain a log of when they visited your site, which allows you to get a picture of their activity prior to engaging with you.

##### 텍스트 검색

```
is:anonymous
```
##### 스크린샷

![](/contacts/media/contacts-anonymous.jpg)
The resulting list will be those IP addresses which have not yet provided identifying information.

#### 표준 연락처

The second type of contact is a standard contact. These contacts have identified themselves via a form or other source — you may also have more information about them from previous interactions. As a result, these contacts typically have a name, email, and other identifying information which can be associated with the contact.

The standard contact is the preferred contact within Mautic. These are contacts which may have started as a visitor, but at some point provided additional information such as a name, email address, social network handle, or other identifying characteristics. You can nurture these contacts through the Mautic marketing automation platform.

The [연락처 관리](https://www.mautic.org/docs/en/contacts/managing_contacts.html) section provides more information on what you can manage with standard contacts.
