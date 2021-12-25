---
description: Flutter Distributor 是一个完整的工具，用于打包和发布您的 Flutter 应用。
---

# 开始

## Distribute Options

```yaml
env:
  FIR_API_TOKEN: 'your api token'
  PGYER_API_TOKEN: 'your api token'
output: dist/
releases:
  - name: dev
    jobs:
      - name: release-dev-android
        package:
          platform: android
          target: apk
          build_args:
            target: lib/main.dart
            flavor: dev
            target-platform: android-arm,android-arm64
        publish_to: fir
      - name: release-dev-ios
        package:
          platform: ios
          target: ipa
          build_args:
            target: lib/main.dart
            flavor: dev
            export-options-plist: ios/dev_ExportOptions.plist
        publish_to: fir
```
