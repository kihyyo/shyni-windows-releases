# Shyni Windows

Windows 10 (2004 이상) / Windows 11 x64용 Shyni 클라이언트 배포 저장소입니다.

[배포 파일 받기](https://github.com/kihyyo/shyni-windows-releases/releases)

- `*-Portable.zip`을 새 폴더에 **전부** 압축 해제한 뒤 Shyni.exe를 실행하세요. 실행 파일만 따로 옮기지 마세요.
- `*-Setup.exe`는 설치형입니다.
- 자동 업데이트가 없는 이전 실행 파일은 최초 한 번 새 배포본으로 바꿔 주세요.
- 이후에는 실행 중 업데이트를 다운로드하고 **정상 종료 후** 적용합니다. 재생 중 강제 종료나 자동 재시작은 하지 않습니다.
- 기존 로그인·설정은 `%LOCALAPPDATA%\Shyni`에 보관됩니다. 이 폴더를 삭제하지 마세요.
- .NET과 재생 엔진이 포함됩니다. YouTube 부가영상에는 Microsoft Edge WebView2 Runtime이 필요합니다.

## 엔진 소스와 라이선스

앱과 함께 제공하는 mpv·FFmpeg는 GPL-only/nonfree 기능을 제외한 LGPL 구성입니다. 각 릴리스에 다음 파일을 함께 제공합니다.

- `shyni-lgpl-*-sources.zip`: 해당 엔진과 의존성의 대응 소스, 패치, 빌드 방법, 고지
- `shyni-lgpl-*-runtime.zip`: 교체 가능한 네이티브 엔진 DLL과 라이선스
- `THIRD-PARTY-NOTICES.md`: 구성요소별 고지와 LGPL 라이브러리 교체 안내
- `SHA256SUMS.txt`: 배포 파일 무결성 확인용 해시

일반 사용자는 설치형 또는 포터블만 받으면 됩니다. 소스 ZIP은 엔진을 확인하거나 재빌드하려는 사용자를 위한 파일입니다. 샤이니 앱 소스와 사용자 계정 정보는 포함하지 않습니다.

DLL은 `Shyni.exe` 옆(포터블의 `current` 폴더)에 별도 파일로 있으며 호환되는 수정 라이브러리로 교체할 수 있습니다. LGPL 수정 디버깅을 위한 역공학을 제한하지 않습니다. 자세한 조건은 배포물의 원문 라이선스와 고지를 참고하세요.
