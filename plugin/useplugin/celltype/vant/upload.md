# 업로드

모바일 화면에서 모던 UI를 사용하여 업로드 셀을 사용할 수 있습니다.

내장된 첨부파일업로드 버튼형 셀과비교해, 이 셀유형은 이점과 제약사항이 있습니다.

### 이점&#x20;

1. 모던UI
2. 카메라 직접 열기 허용

### 제약사항&#x20;

1. 리스트뷰에서 사용할 수 없습니다.
2. 스타일 템플릿을 지원하지 않음
3. 드래그 앤 드롭으로 파일 업로드를 지원하지 않습니다.



업로드값은 "|"로 구분된 파일 이름 그룹인 문자열이어야 합니다.



### 빌더 화면&#x20;

<figure><img src="../../../../.gitbook/assets/image (1002).png" alt=""><figcaption></figcaption></figure>

### 실행 화면 (런타임)

<figure><img src="../../../../.gitbook/assets/image (961).png" alt=""><figcaption></figcaption></figure>



### 셀속성&#x20;

<figure><img src="../../../../.gitbook/assets/image (1007).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="252">이름 </th><th>설명 </th></tr></thead><tbody><tr><td>UI 권한</td><td>다른 사용자 역할에 대해 다른 활성화/표시 상태 표시</td></tr><tr><td>제한 </td><td><p>업로드할 수 있는 최대 파일 수를 제한합니다. 기본값은 제한이 아닙니다.<br>사용자가 셀 속성 설정 명령 또는 다중 업로드로 제한보다 많은 파일을 표시하려고 하면 처음 두 파일만 업로드됩니다.</p><p>파일 수가 한도에 도달하면 업로드 영역이 숨겨집니다.</p></td></tr><tr><td>수락 </td><td>업로드 파일의 확장자를 수락합니다. 기본값은 ".jpg, .jpeg, .png"입니다.<br>사용자가 잘못된 파일을 업로드하려고 하면 업로드가 실패합니다.</td></tr><tr><td>크기 제한</td><td>업로드 파일 크기 제한, 단위는 MB, 기본값은 제한 없음<br>값을 제거하거나 값을 0으로 설정하면 제한 없음을 의미합니다<br>. 사용자가 크기 제한보다 큰 파일을 업로드하면 다음 메시지가 표시됩니다.<br><img src="https://grapecity.atlassian.net/wiki/download/attachments/2931196662/image2022-5-9_11-55-24.png?version=1&#x26;modificationDate=1652068524753&#x26;cacheVersion=1&#x26;api=v2" alt=""></td></tr><tr><td>캡쳐 </td><td><p>업로드 영역 클릭 후 동작을 나타냅니다.</p><p>1.이미지 라이브러리: 이미지 라이브러리 열기</p><p>2. 카메라: 오픈 카메라</p></td></tr><tr><td>업로드 영역 표시</td><td>업로드 영역 표시</td></tr><tr><td>업로드 아이콘</td><td>업로드 영역 아이콘을 변경합니다.</td></tr><tr><td>업로드 팁</td><td>업로드 영역의 텍스트.</td></tr><tr><td>업로드 이미지 구성</td><td><img src="../../../../.gitbook/assets/image (938).png" alt=""></td></tr><tr><td>미리보기 영역 크기</td><td>단위: 픽셀</td></tr><tr><td>미리보기이미지 맞춤 모드 </td><td><ul><li>채우기- 기본값입니다. 주어진 치수를 채우도록 이미지 크기가 조정됩니다. 필요한 경우 이미지가 크기에 맞게 늘어나거나 찌그러집니다.</li><li>포함 - 이미지는 종횡비를 유지하지만 주어진 크기에 맞게 크기가 조정됩니다.</li><li>덮기 - 이미지는 종횡비를 유지하고 주어진 치수를 채웁니다. 이미지는 크기에 맞게 잘립니다.</li><li>초기 - 이미지 크기가 조정되지 않습니다.</li><li>축소 - 이미지는 가장 작은 버전 또는 <code>none</code>  <code>contain</code></li></ul></td></tr><tr><td>클릭 시 전체 화면 이미지 미리보기 표시</td><td>클릭 시 전체 화면 이미지 미리보기 표시<br></td></tr><tr><td>삭제 가능</td><td>삭제 아이콘 표시 여부</td></tr><tr><td>다중 </td><td>다중 선택 사진 활성화 여부</td></tr><tr><td>비활성화 </td><td>비활성화 </td></tr><tr><td>읽기 전용</td><td>읽기 전용<br></td></tr></tbody></table>

