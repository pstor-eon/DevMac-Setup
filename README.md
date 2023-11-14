# DevMac-Setup

### macOS 키보드 설정 스크립트 ⌨️
이 스크립트는 터미널 명령어를 사용하여 macOS에서 키보드 설정을 사용자화하는 데에 사용됩니다.

### 명령어

1. InitialKeyRepeat Delay

```bash
defaults write -g InitialKeyRepeat -int 25
```

이 명령어는 키를 누를 때 반복이 시작되기 전의 딜레이를 설정합니다. '25'라는 값은 딜레이를 나타내며, 값이 클수록 딜레이가 길어집니다.

2. KeyRepeat Interval

```bash
defaults write -g KeyRepeat -int 6
```

이 명령어는 키 반복 속도를 조절합니다. '6'이라는 값은 키 반복 간격을 나타내며, 값이 작을수록 반복이 빨라집니다.

3. Apple Press and Hold Enabled

```bash
defaults write -g ApplePressAndHoldEnabled -bool true
```

이 명령어는 Apple Press and Hold 기능을 활성화합니다. 이 기능은 키를 길게 누르면 대체 문자(예: 액센트, 특수 문자)를 표시합니다.

```bash
defaults write -g ApplePressAndHoldEnabled -bool false
```

Apple Press and Hold Enabled은 호불호가 있으므로 설정하고 마음에 들지 않는다면 위에 있는 명령어로 해지할 수 있다.


## 프로그램
### Productivity Tools
- [무비스트](https://movistprime.com/): 강력한 동영상 플레이어
- [Magnet](https://magnet.crowdcafe.com/): 창 관리 도구
- [Authy Desktop](https://authy.com/): 2단계 인증 앱
- [LogiTune](https://www.logitech.com/): 로지텍 디바이스 설정 도구
- [Obsidian](https://obsidian.md/): 메모 및 노트 테이킹 앱
- [Spoytify](https://www.spotify.com/): Spotify 데스크톱 클라이언트
- [melon](https://www.melon.com/): 멜론 음악 스트리밍 앱
- [Gimp](https://www.gimp.org/): 무료 이미지 편집기

### Office Suite
- [Pages](https://www.apple.com/pages/): Apple의 워드 프로세서
- [Keynote](https://www.apple.com/keynote/): Apple의 프레젠테이션 소프트웨어
- [Numbers](https://www.apple.com/numbers/): Apple의 스프레드시트 앱
- [Microsoft Office Suite](https://www.microsoft.com/office): 마이크로소프트 오피스 스위트
  - Word
  - Excel
  - PowerPoint
  - Outlook
- [Notion](https://www.notion.so/): 협업 및 노트 플랫폼
- [한컴오피스 한글 2014 VP](https://www.hancom.com/): 국내 한글 편집기

### Development Tools
- [Visual Studio Code](https://code.visualstudio.com/): 경량 코드 편집기
- [Parallels Desktop](https://www.parallels.com/): 가상 머신 소프트웨어
- [Xcode](https://developer.apple.com/xcode/): Apple 개발자 도구
- [iterm](https://iterm2.com/): 향상된 터미널 에뮬레이터
- [Docker](https://www.docker.com/): 컨테이너 기반 가상화 플랫폼
- [PyCharm](https://www.jetbrains.com/pycharm/): Python 개발 툴
- [GitHub Desktop](https://desktop.github.com/): GitHub 클라이언트
- [FileZilla](https://filezilla-project.org/): FTP 클라이언트
- [Android Studio](https://developer.android.com/studio): 안드로이드 개발 도구
- [VMware Fusion](https://www.vmware.com/products/fusion.html): 가상 머신 소프트웨어
- [Sourcetree](https://www.sourcetreeapp.com/): Git 그래픽 인터페이스

### Utilities
- [APP Cleaner](https://freemacsoft.net/appcleaner/): 앱 제거 및 시스템 청소 도구

### Design and Multimedia
- [HazeOver](https://hazeover.com/): 활성 창 강조 툴
- [Keka](https://www.keka.io/): 파일 압축 및 해제 도구
- [OBS Studio](https://obsproject.com/): 무료 오픈소스 브로드캐스팅 소프트웨어

### Communication
- [Discord](https://discord.com/): 음성 및 텍스트 채팅 플랫폼
- [카카오톡](https://www.kakaocorp.com/service/KakaoTalk): 대표적인 대화 앱
- [Zoom](https://zoom.us/): 비디오 회의 소프트웨어
- [Slack](https://slack.com/): 팀 협업 메시징 플랫폼
- [Skype](https://www.skype.com/): 온라인 음성 및 비디오 통화 소프트웨어

## 개발환경 설정

### iTerm2 설치 및 설정

1. **iTerm2 설치**
   - [iTerm2 공식 웹사이트](https://iterm2.com/)에서 iTerm2를 다운로드하고 설치합니다.

2. **테마 설정**
   - [Oh My Zsh](https://ohmyz.sh/)를 설치하여 터미널 테마를 쉽게 변경할 수 있습니다.
   - 다음 명령어를 실행하여 Oh My Zsh를 설치합니다.
     ```bash
     sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
     ```
   - 좋아하는 테마로 변경하려면 `~/.zshrc` 파일에서 `ZSH_THEME` 항목을 수정합니다.

3. **iTerm2 단축키 설정**
   - iTerm2의 단축키를 사용하면 터미널을 더 효과적으로 사용할 수 있습니다.
   - iTerm2 메뉴에서 `Preferences > Keys`로 이동하여 단축키를 설정합니다.

### Vim 설정

1. **Vim 설치**
   - 터미널에서 다음 명령어로 Vim을 설치합니다.
     ```bash
     brew install vim
     ```

2. **Vim 설정 파일 (`~/.vimrc`)**
   - Vim의 설정 파일은 `~/.vimrc`에 저장됩니다.
   - 간단한 예제 `.vimrc` 파일:
     ```vim
     syntax enable
     set background=dark
     set tabstop=4
     set shiftwidth=4
     set softtabstop=4
     set number
     ```

3. **Vim 플러그인 관리자 설치**
   - Vim 플러그인 관리자로 [Vundle](https://github.com/VundleVim/Vundle.vim)나 [Pathogen](https://github.com/tpope/vim-pathogen)을 사용하세요.

### 파이썬 설치

1. **Homebrew 설치**
   - [Homebrew](https://brew.sh/)를 사용하여 손쉽게 패키지를 설치합니다.
   - 터미널에서 다음 명령어를 실행하여 Homebrew를 설치합니다.
     ```bash
     /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
     ```

2. **Python 설치**
   - Homebrew를 사용하여 파이썬을 설치합니다.
     ```bash
     brew install python
     ```

3. **가상 환경 설정**
   - `virtualenv`나 `venv`를 사용하여 가상 환경을 만들어 프로젝트별로 독립적인 환경을 구축하세요.
   - 예를 들어:
     ```bash
     python3 -m venv myenv
     source myenv/bin/activate
     ```

4. **pip 업그레이드**
   - 가상 환경에서 `pip`를 최신 버전으로 업그레이드합니다.
     ```bash
     pip install --upgrade pip
     ```