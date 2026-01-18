# ColorOS 기본앱 삭제

## 환경
- ColorOS 16.0.0.210

## ADB 명령어 목록

```sh
# 비활성화 (Disable)
adb shell pm disable-user --user 0 com.coloros.securepay

# 일시 중지 (Suspend)
adb shell pm suspend --user 0 com.coloros.findmyphone
adb shell pm suspend --user 0 com.heytap.browser
adb shell pm suspend --user 0 com.heytap.htms
adb shell pm suspend --user 0 com.heytap.market
adb shell pm suspend --user 0 com.heytap.openid
adb shell pm suspend --user 0 com.nearme.instant.platform
adb shell pm suspend --user 0 com.oplus.pay
adb shell pm suspend --user 0 com.tencent.soter.soterserver

# 삭제 (Uninstall)
adb shell pm uninstall --user 0 cn.wps.moffice_eng
adb shell pm uninstall --user 0 com.android.email
adb shell pm uninstall --user 0 com.android.mms
adb shell pm uninstall --user 0 com.android.mms.service
adb shell pm uninstall --user 0 com.coloros.accessibilityassistant
adb shell pm uninstall --user 0 com.coloros.sharescreen
adb shell pm uninstall --user 0 com.coloros.calendar
adb shell pm uninstall --user 0 com.coloros.codebook
adb shell pm uninstall --user 0 com.coloros.colordirectservice
adb shell pm uninstall --user 0 com.coloros.mapcom.frame
adb shell pm uninstall --user 0 com.coloros.ocrscanner
adb shell pm uninstall --user 0 com.coloros.operationManual
adb shell pm uninstall --user 0 com.coloros.phonemanager
adb shell pm uninstall --user 0 com.coloros.remoteguardservice
adb shell pm uninstall --user 0 com.coloros.sceneservice
adb shell pm uninstall --user 0 com.coloros.securityguard
adb shell pm uninstall --user 0 com.coloros.sharescreen
adb shell pm uninstall --user 0 com.oplus.aimemory
adb shell pm uninstall --user 0 com.oplus.qualityprotect
adb shell pm uninstall --user 0 com.oplus.tai.borderpresearch
adb shell pm uninstall --user 0 com.heytap.accessory
adb shell pm uninstall --user 0 com.heytap.cloud
adb shell pm uninstall --user 0 com.heytap.music
adb shell pm uninstall --user 0 com.heytap.mydevices
adb shell pm uninstall --user 0 com.heytap.reader
adb shell pm uninstall --user 0 com.heytap.speechassist
adb shell pm uninstall --user 0 com.heytap.themestore
adb shell pm uninstall --user 0 com.heytap.vip
adb shell pm uninstall --user 0 com.heytap.yoli
adb shell pm uninstall --user 0 com.hongen.app.word
adb shell pm uninstall --user 0 com.jideos.jnotes
adb shell pm uninstall --user 0 com.nearme.gamecenter
adb shell pm uninstall --user 0 com.netease.cloudmusic
adb shell pm uninstall --user 0 com.newskyer.draw
adb shell pm uninstall --user 0 com.oneplus.bbs
adb shell pm uninstall --user 0 com.oneplus.member
adb shell pm uninstall --user 0 com.oplus.aiwidgets
adb shell pm uninstall --user 0 com.oplus.acc.gac
adb shell pm uninstall --user 0 com.oplus.aiwriter
adb shell pm uninstall --user 0 com.oplus.appdetail
adb shell pm uninstall --user 0 com.oplus.appsense
adb shell pm uninstall --user 0 com.oplus.crashbox
adb shell pm uninstall --user 0 com.oplus.games
adb shell pm uninstall --user 0 com.oplus.game.empowerment.folder
adb shell pm uninstall --user 0 com.oplus.location
adb shell pm uninstall --user 0 com.oplus.onetrace
adb shell pm uninstall --user 0 com.oplus.owork
adb shell pm uninstall --user 0 com.oplus.securitypermission
adb shell pm uninstall --user 0 com.oplus.statistics.rom
adb shell pm uninstall --user 0 com.oplus.studycenter
adb shell pm uninstall --user 0 com.oplus.tips
adb shell pm uninstall --user 0 com.oplus.viewtalk
adb shell pm uninstall --user 0 com.oppo.instant.local.service
adb shell pm uninstall --user 0 com.oppo.store
adb shell pm uninstall --user 0 com.qiyi.video.pad
adb shell pm uninstall --user 0 com.sinyee.babybus.world
adb shell pm uninstall --user 0 com.sohu.inputmethod.sogouoem
adb shell pm uninstall --user 0 com.ss.android.ugc.aweme
adb shell pm uninstall --user 0 com.ted.number
adb shell pm uninstall --user 0 com.wyt.iexuetang.hd.iexuetang
adb shell pm uninstall --user 0 com.youban.xbldhw
adb shell pm uninstall --user 0 com.youku.phone
adb shell pm uninstall --user 0 net.huanci.hsjpro
```

## 선정 기준
이 리스트는 여러 요소를 고려하여 보수적으로 작성되었습니다:

- OxygenOS에 존재하지 않는 앱인가?
- Google 서비스로 완전히 대체 가능한가?
- 중국어 콘텐츠를 표시하는가?
- 다른 언어나 지역 서비스에서는 사용할 수 없는가?
- 개인 정보(예: 비밀번호, 추적)와 너무 밀접하게 연관되어 있는가?
- 제거/비활성화해도 시스템 안정성에 영향을 주지 않는가?
- OPPO 생태계 전용 기능인가?


> **참고:**
> 위 기준 때문에 삭제하고 싶지만 남아있는 앱이 있을 수 있습니다. 그런 앱들은 직접 수동으로 비활성화하거나 제거해도 무방합니다.