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
