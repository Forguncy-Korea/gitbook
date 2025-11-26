# UserInfo 인터페이스

사용자에 대한 정보입니다. getUserInfo 메서드에 사용됩니다.



| 속성                      | 형식                                                                                                    | 설명                                                                                        |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| UserName                | string                                                                                                | 사용자 이름입니다.                                                                                |
| FullName                | string                                                                                                | 사용자의 전체 이름입니다.                                                                            |
| Email                   | string                                                                                                | 사용자 사서함입니다.                                                                               |
| Role                    | string                                                                                                | 사용자 역할 이름입니다. 사용자에게 둘 이상의 역할이 있는 경우 역할 간에 "Administrator, 관리자"와 같은 구분이 사용됩니다.             |
| OrganizationSuperior    | string                                                                                                | 사용자의 조직 상위입니다. 사용자에게 여러 조직 상위가 있는 경우 조직 상위 간에 \| 사용됩니다. \[Administrator\| 관리자]와 같은 구분입니다. |
| Properties              | [UserExtendProperties\[\]](https://help.grapecity.com.cn/pages/viewpage.action?pageId=72364509)       | 사용자의 사용자 지정 속성입니다.                                                                        |
| OrganizationLevelValues | [OrganizationLevelValueInfo\[\]](https://help.grapecity.com.cn/pages/viewpage.action?pageId=72364503) | 사용자의 조직 수준 정보입니다.                                                                         |
| HasPicture              | boolean                                                                                               | 아바타가 있습니까?                                                                                |
