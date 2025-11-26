# 명령 백업

배치 스크립트를 사용한 백업이 지원됩니다. 명령줄은 다음 위치에서 실행되어야 합니다.

Windows: FORGUNCY\_SERVER\_INSTALL\_DIR\WebSite\bin\
Linux: FORGUNCY\_SERVER\_INSTALL\_DIR/WebSite/bin/

예를 들면 다음과 같습니다.

Windows: C:\Program Files\ForguncyServer\WebSite\bin&#x20;

Linux: /opt/ForguncyServer/WebSite/bin

## 명령 백업&#x20;



|                    | 명령                                  | 설명                                                                                                                                                      |
| ------------------ | ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **도움말 설명서를 표시합니다** | \\? 또는 \help                        | <p><br></p>                                                                                                                                             |
| **백업**             | backup _MyApp_ _MyApp.bak_          | <p>백업은 지정된 파일에 적용하도록 지정해야 합니다. MyApp은 앱 이름이며 MyApp .bak 백업 파일 이름입니다.</p><p>명령줄 백업은 사용자가 파일 이름을 지정해야 한다는 점을 제외하면 사용자 서비스의 백업 응용 프로그램과 동일한 기능을 수행합니다.</p> |
| **복원합니다**          | restore _App App.bak_               | 파일을 지정하여 앱을 복원합니다.                                                                                                                                      |
| **모든 앱을 백업합니다**    | backupallapps "_backup file path_"  | 이 명령은 백업 파일이 저장될 위치를 지정해야 합니다.                                                                                                                          |
| **사용자 데이터를 백업합니다** | backupUserData "_backup file path"_ | <p><br></p>                                                                                                                                             |
| **사용자 데이터를 복구합니다** | restoreUserData "backup file path"  | 이 작업은 관리자 권한으로 수행해야 합니다.                                                                                                                                |
