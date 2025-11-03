# ColorOS Debloat List

## Environment
- ColorOS 16.0.0.210

## ADB Command List

```sh
# Disable
adb shell pm disable-user --user 0 com.coloros.securepay

# Suspend
adb shell pm suspend --user 0 com.coloros.findmyphone
adb shell pm suspend --user 0 com.heytap.browser
adb shell pm suspend --user 0 com.heytap.htms
adb shell pm suspend --user 0 com.heytap.market
adb shell pm suspend --user 0 com.heytap.openid
adb shell pm suspend --user 0 com.nearme.instant.platform
adb shell pm suspend --user 0 com.oplus.pay
adb shell pm suspend --user 0 com.tencent.soter.soterserver

# Uninstall
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

## Criteria
The criteria for this list were set conservatively and based on multiple factors:

- Does it not exist in OxygenOS?
- Can it be fully replaced by Google services?
- Does it display content in Chinese?
- Is it unusable for other languages or regional services?
- Is it too closely related to personal information (e.g., password, tracking)?
- Does removing/disabling it not affect system stability?
- Is it a feature exclusive to the OPPO ecosystem?


> **Note:**
> Because of these criteria, there may be apps remaining that you wish to remove. You are free to manually disable or uninstall them yourself.
