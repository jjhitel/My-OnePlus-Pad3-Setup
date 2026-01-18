# OTA 플래싱 (Flash OTA)

이 섹션은 전체 OTA 패키지를 수동으로 플래싱하는 방법을 다룹니다. 부트로더가 언락되어 있어야 합니다.

### **자료 (Resources)**
* **COS 플래셔:** [Pad 2 Pro용 플래셔 템플릿](https://mega.nz/file/hc91CQLJ#50Veg8rD3tMXoLL6M60GoW6WoaTTvQjtdIJ9BgjkF9k)
* **OOS 플래셔:** [Pad 3용 플래셔 템플릿](https://mega.nz/file/kJlD2QrT#yzYPmRia8dwsIfaQetgoloNBshgr_jbsiAJ80wryaoo)
* **ROM 아카이브:** [공식 OnePlus ROM (중국)](https://yun.daxiaamu.com/OnePlus_Roms/%E4%B8%80%E5%8A%A0OnePlus%20Pad%202%20Pro/)
* **OTA 추출기:** [otaripper](https://github.com/syedinsaf/otaripper/releases)

### **플래싱 단계**

1.  플래셔 템플릿을 다운로드하고 압축을 풉니다.

2.  ROM 아카이브에서 필요한 Full OTA 파일을 다운로드합니다.

3.  OTA 추출기(`otaripper`)를 사용하여 `ota.zip`에서 모든 `.img` 파일을 추출합니다.
    ```
    otaripper -p path/to/ota.zip -o path/to/output_dir
    ```

4.  추출된 이미지 파일들을 플래셔 템플릿 폴더 내의 `OOS_FILES_HERE` (COS의 경우 `COS_FILES_HERE`) 폴더에 넣습니다.

5.  기기를 Fastboot 모드(`볼륨 감소 + 전원`)로 부팅하고 PC에 연결합니다.

6.  `OOS_Flasher.bat` 스크립트를 실행하고 화면의 지시를 따릅니다.

### **교차 플래싱**
이제 스타일러스나 OTA 문제 없이 Pad 2 Pro에 OxygenOS를 설치하거나 Pad 3에 ColorOS를 설치할 수 있습니다. 다만 방법이 변경되었으므로 [이 가이드](./unbrick.md)를 참고하세요.