# ApplePrivacyInfo
애플 개인정보 보호(PrivacyInfo) 관련 대응


# [App Store 앱 제출을 위한 개인정보 보호 관련 업데이트](https://developer.apple.com/kr/news/?id=3d8a9yyh)

2024년 02월 29일

개발자는 자신의 앱에 포함된 모든 코드에 대한 책임이 있습니다. Apple은 WWDC23에서 널리 사용되는 타사 SDK를 위한 새로운 [개인정보 보호 매니페스트 및 서명](https://developer.apple.com/kr/support/third-party-SDK-requirements/) 기능을 발표했으며, 개발자가 앱의 개인정보 보호 매니페스트에서 [일부 API 세트를 사용하는 데 대한 허용된 사유(영문)](https://developer.apple.com/documentation/bundleresources/privacy_manifest_files/describing_use_of_required_reason_api)를 선언해야 함을 공지한 바 있습니다. 이러한 변경 사항은 개발자가 타사 SDK의 데이터 사용 방식, 소프트웨어 종속성 보안, 사용자 개인정보를 위해 제공되는 추가 보호 기능 등을 파악하는 데 도움이 됩니다.

3월 13일부터: App Store Connect에 사유가 필요한 API를 사용하는 신규 앱 또는 업데이트된 앱을 업로드하는 경우, 앱의 개인정보 보호 매니페스트에 사유가 누락되면 이메일을 보내드립니다. 이 이메일은 App Store Connect의 기존 알림에 추가됩니다.

5월 1일부터: 신규 앱 또는 업데이트된 앱의 코드에 특정 API를 사용할 경우, 이를 App Store Connect에 업로드하려면 허용된 사유를 포함해야 합니다. API를 허용된 사유에 따라 사용하지 않는 경우 다른 대안을 찾아보시기 바랍니다. 또한 흔히 사용되는 타사 SDK 목록에 새로운 타사 SDK를 추가하는 경우 이러한 API, 개인정보 보호 매니페스트, 서명 요건이 해당 SDK에 적용됩니다. 개인정보 보호 매니페스트가 포함된 버전의 SDK를 사용해야 합니다. 또한 SDK가 바이너리 종속성으로 추가된 경우 서명도 필요합니다.

이 기능은 모든 앱에 유용합니다. Apple은 모든 SDK가 SDK 사용 비중이 높은 앱들을 위한 지원을 강화하기 위해 이 기능을 도입하는 것을 권장합니다.

## Overview

### Privacy Tracking Enabled
### Privacy Nutrition Labels  
- [Types of data](https://developer.apple.com/app-store/app-privacy-details/)
### Privacy Tracking Domains
### Privacy Accessed API Types  
- [Describing use of required reason API](https://developer.apple.com/documentation/bundleresources/privacy_manifest_files/describing_use_of_required_reason_api)

## Privacy report
Archive 후 Generate Privacy Report 체크  
Report의 정보들을 이용해 **Privacy Nutrition Label**에 추가

## Test
TestFlight 외부 테스터 추가 - PrivacyInfo가 포함된 빌드 버전으로 빌드 - 심사 통과 후 결과 전달 받은 내용으로 수정 or 통과

------------------------------------

## Reference
- [Describing use of required reason API](https://developer.apple.com/documentation/bundleresources/privacy_manifest_files/describing_use_of_required_reason_api)
- [Get started with privacy manifests](https://developer.apple.com/wwdc23/10060)
- [Verify app dependencies with digital signatures](https://developer.apple.com/wwdc23/10061)
- [Types of data](https://developer.apple.com/app-store/app-privacy-details/)
