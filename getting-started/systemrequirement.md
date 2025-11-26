---
description: Forguncy(포건시) 빌더와 서버의 시스템 사양을 설명합니다.
---

# 시스템 요구사항

포건시 10.X 버전의 시스템 설치 요구사항 입니다.



## **빌더(Builder) 시스템 사양**

웹 페이지를 디자인하고 기능을 구현하기 위해, 사용하는 포건시 빌더 프로그램의 시스템 설치 사양을 안내합니다.

<table><thead><tr><th width="171.89220970112692">구분</th><th width="480.3333333333333">시스템 요구사항</th><th data-hidden></th><th data-hidden></th></tr></thead><tbody><tr><td>  <strong>OS</strong></td><td><p>Windows 7／8.1 update／10 / 11 </p><p>Server 2008 R2 SP1 / Server 2012 / Server 2012 R2 update / Server2016 / Server 2019</p><p>(위 시스템은 모두 64비트입니다.)<br></p><p> * Server Core 제외 <br> * Server 2008 R2 SP1에 설치된 빌더의 프로세스로 설계된 응용 프로그램은 지원되지 않습니다 .</p></td><td></td><td></td></tr><tr><td> <strong>CPU</strong></td><td>  Core™ i3 2GHz 이상</td><td><br></td><td></td></tr><tr><td> <strong>메모리</strong></td><td> 최소 4GB 이상</td><td></td><td></td></tr><tr><td><strong>설치 크기(MB)</strong></td><td> 400MB 이상<br> * Framework가 설치되어 있지 않은 경우 HDD 2GB 이상 필요</td><td></td><td></td></tr><tr><td> <strong>.NET</strong></td><td><p> - 6   (Forguncy V 10.0.4.0)</p><p>6 버전의 소프트웨어가 설치되어 있지 않으면 Forguncy 설치 시 자동으로 설치되지만 .NET Framework 3.5 SP 1이상이 설치되어 있는지 확인해야 합니다. Net Framework 3.5 SP1 이상이 설치되어 있는 경우 Forguncy를 설치하기 전에 Microsoft 웹사이트에서 다운로드하여 설치해야 합니다.</p><p>버전 6.1 이상에서만 .NET Core를 설치해야 합니다.</p><p></p><ul><li>8 (Forguncy v10.0.13.0)</li></ul><p></p></td><td></td><td></td></tr><tr><td> <strong>브라우저</strong></td><td> - Microsoft Edge 최신 버전<br> - Google Chrome 최신 버전</td><td><strong>서버 시스템 사양</strong></td><td></td></tr></tbody></table>



### **서버(Server) 시스템 사양**

포건시 빌더에서 만든 웹 페이지를 배포하기 위한, 서버 프로그램의 시스템 설치 사양을 안내합니다.

<table><thead><tr><th width="227">구분</th><th>시스템요구사항</th><th data-hidden></th></tr></thead><tbody><tr><td><strong>OS</strong></td><td><p>64 비트 시스템</p><ul><li>Windows:  7/ 8.1 / 10 / 11 / <br>Server 2008 R2 SP1 / Server 2012 / Server 2012 R2 update<br>Server 2016 / Server 2019</li><li>Linux: Ubuntu 16.04 / Ubuntu 18.04 /Ubuntu 22.04 /<br> CentOS 7(1804), RadHat 7.6 : Forguncy v10.0.4.0에서  지원/ <br> RadHat 8<br></li></ul><p> * Server Core 제외 <br> * Server 2008 R2 SP1에 프로세스 지원 애플리케이션을 게시하는 것은 지원되지 않습니다.</p></td><td></td></tr><tr><td> <strong>CPU</strong></td><td>  Core™ i3 2GHz 이상 (듀얼 코어 이상 추천)</td><td><br></td></tr><tr><td> <strong>메모리</strong></td><td> 최소 4GB 이상 (8GB 이상 추천)</td><td></td></tr><tr><td> <strong>설치 크기(MB)</strong></td><td> 300MB 이상 (80GB 이상 추천)<br> * Framework가 설치되어 있지 않은 경우 HDD 2GB 이상 필요</td><td></td></tr><tr><td>.NET</td><td><p>6 (Forguncy v10.0.4.0)<br></p><ul><li><strong>위 버전의 소프트웨어가 설치되어 있지 않은 경우 포건시 서버를 설치할 때 자동으로 설치되지만 시스템에 .Net Framework 3.5 SP1 이상이 설치되어 있는지 확인해야 합니다. Net Framework 3.5 SP1 이상이 설치되어 있는 경우, 포건시 서버를 설치하기 전에 Microsoft 웹사이트에서 다운로드하여 설치해야 합니다.</strong></li><li><strong>버전 6.1 이상에서만 .NET Core를 설치해야 합니다.</strong></li></ul><p>8 (Forguncy v10.0.13.0)</p></td><td></td></tr></tbody></table>



### 외부Database 지원

| 구분                        | 버전요구사항                                                                                                                                                         |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|  **Microsoft Access**     | MS Access DB 연결 시 Forguncy Server에 MS Access가 설치되어 있어야 합니다.                                                                                                    |
|  **Microsoft SQL Server** | <p> - 2008 R2 SP1<br> - 2012 SP3<br> - 2014 SP2 <br> - 2016 SP2 <br> - 2017<br> - 2019</p><p> - 2022</p>                                                       |
|  **Oracle Database**      | <p> - 10G<br> - 11G Release 2 (11.2)<br> - 12C Release 2 (12.2)<br> - 18C Release 3 (18.3)<br> - 19C Release 3 (19.3)<br> - 23<br>64비트 Oracle 데이터베이스 클라이언트</p> |
|  **mySQL**                | <p> - 5.6<br> - 5.7<br> - 8.0</p>                                                                                                                              |
|  **MariaDB**              |  10.3                                                                                                                                                          |
|  **PostgreSQL**           | <p> - v11<br> - v12<br> - v13<br> - v14<br> - v15<br> - V16</p>                                                                                                |
|  **Dameng**               |  v6                                                                                                                                                            |
|  AzureSynapse             | <p><br></p>                                                                                                                                                    |
| Hana Database             |                                                                                                                                                                |
| Snowflake Database        |                                                                                                                                                                |
| **ODBC 지원**               | 모든 유형의 데이터베이스에 연결할 수 있지만 다양한                                                                                                                                   |

## 클라이언트 요구 사항

클라이언트가 포건시에 접속하는 환경에 따른 브라우저 버전 요구사항은 아래와 같습니다.

| 기기    | 브라우저 버전 요구사항                                           |
| ----- | ------------------------------------------------------ |
| 윈도우   | Microsoft Edge 최신 버전(Chromium 코어), Google Chrome 최신 버전 |
| 아이폰   | Safari(최신 버전의 iOS 14.3)                                |
| 안드로이드 | Google Chrome 최신 버전                                    |
| 아이패드  | 사파리 (iOS 14.3 최신 버전)                                   |
