# 安裝

```shell
scoop install fvm
```

[官網安裝步驟](https://fvm.app/documentation/getting-started/installation)

# 指令

```shell
fvm install stable    # 安裝最新穩定版
fvm use stable        # 在當前專案使用該版本
# fvm list              # 查看已安裝的版本
# fvm flutter run       # 使用指定版本執行 Flutter
# fvm global 3.22.0     # 設定全域預設版本
# fvm remove <version>  # 移除舊版本

fvm flutter doctor          # 檢查環境
fvm flutter create <my_app> # 建立新專案
fvm flutter run


# windows開發
flutter run -d windows
# web 開發
flutter run -d web-server
# android 開發
flutter emulators
flutter emulators --launch <emulator_id>
flutter run


# 打包
flutter clean    # 打包前先執行這兩行
flutter pub get
# build\app\outputs\flutter-apk\app-release.apk
flutter build apk --release
# build\windows\runner\Release\your_app.exe
flutter build windows --release
# build/ios/ipa/Runner.ipa
flutter build ipa --export-method=app-store

```

