# 연락처

Leads were renamed to contacts in Mautic 1.4.0.

Contacts are the central factor of a marketing automation platform. These are all the individuals who have visited your websites or interacted with you in some way.

### 연락처 유형

연락처에는 다음과 같은 2가지 유형이 있습니다:
* **방문객** (formerly anonymous leads) — visitors to your site who have not yet been identified by a form or other interaction.
  * These contacts are tracked by Mautic but typically remain hidden so as not to clutter your segment.
* **표준 연락처** — contacts which have identified themselves via a form or some other source. As a result, these contacts typically have a name, email, and other identifying fields.

#### 방문객 (formerly anonymous leads)

Anonymous leads were renamed to visitors in Mautic 1.4.0.

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
