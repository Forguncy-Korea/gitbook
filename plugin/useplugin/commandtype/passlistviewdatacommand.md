# 리스트뷰로 데이터 전달(PassListviewDataCommand)

리스트뷰로 데이터 전달 명령을 사용하면 페이지간에 리스트뷰에서 다른 리스트뷰로  데이터를 전달할 수 있습니다.&#x20;

### 플러그인 다운로드&#x20;

버전에 맞는 플러그인을 다운로드 합니다.

<table><thead><tr><th width="139">버전 </th><th>다운로드 링크 </th></tr></thead><tbody><tr><td>v10.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V10_Plugin/PassListviewDataCommand.zip">PassListviewDataCommand.zip</a></td></tr><tr><td>v 9.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V9_Plugin/PassListviewDataCommand.zip">PassListviewDataCommand.zip</a></td></tr><tr><td>v 7. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7.1_Plugin_20211223/PassListviewDataCommand.zip">PassListviewDataCommand.zip</a></td></tr><tr><td>v 7. 0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7_Plugin_20210722/PassListviewDataCommand.zip">PassListviewDataCommand.zip</a></td></tr><tr><td>v 6. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V6.1_Plugin_20201111/PassListviewDataCommand.zip">PassListviewDataCommand.zip</a></td></tr><tr><td>v 6. 0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V6_Plugin_20200903/PassListviewDataCommand.zip">PassListviewDataCommand.zip</a></td></tr><tr><td>v 5. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V5_Plugin_20191115/PassListviewDataCommand.zip">PassListviewDataCommand.zip</a></td></tr></tbody></table>

### 사용 방법&#x20;

1. 플러그인을 다운로드합니다.
2. Forguncy Builder에서 설치하고 Forguncy Builder를 다시 실행합니다.
3. 두개의 데이터 테이블을 페이지의 리스트뷰에 바인딩합니다.&#x20;
4. 페이지에 "데이터 전달"이라는 버튼을 생성한 후, 명령 편집을 합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1724).png" alt=""><figcaption></figcaption></figure>

5\. 명령창에서 아래와 같이 설정합니다.&#x20;

* 명령 선택 : 리스트뷰로 데이터 전달&#x20;
* 대상 행 : 모든 행
* 가져오기 모드 : 추가&#x20;
* 전달할 열&#x20;

&#x20;     전송하는 원본 : C3    전달받을 대상 : 페이지1!M3&#x20;

&#x20;     전송하는 원본 : F3    전달받을 대상 : 페이지1!Q3

<figure><img src="../../../.gitbook/assets/image (396).png" alt=""><figcaption></figcaption></figure>

6\. 실행을 하고, 데이터 전달 버튼을 클릭하면 리스트뷰로 데이터가 전달되는 것을 확인할 수 있다.&#x20;

<figure><img src="../../../.gitbook/assets/image (2081).png" alt=""><figcaption></figcaption></figure>
