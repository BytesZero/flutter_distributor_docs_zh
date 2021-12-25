---
description: 如何使用 Flutter Distributor 的命令行界面（CLI）
---

# CLI

## 安装

```
dart pub global activate flutter_distributor
```

## 命令

{% hint style="info" %}
These commands are sorted in alphabetical order. The most commonly used are  package, publish, and release.&#x20;
{% endhint %}

### Package

将应用程序打包为特定于平台的格式，并将结果放入文件夹中。

<table><thead><tr><th>Flag</th><th>Value</th><th data-type="checkbox">Required</th></tr></thead><tbody><tr><td><code>--platform</code></td><td>Platform, e.g. <code>android</code></td><td>true</td></tr><tr><td><code>--targets</code></td><td>Comma separated list of maker names</td><td>true</td></tr></tbody></table>

示例：

```
flutter_distributor package --platform=android --targets=aab,apk
```

### Publish

<table><thead><tr><th>Flag</th><th>Value</th><th data-type="checkbox">Required</th></tr></thead><tbody><tr><td><code>--path</code></td><td>Path, e.g. <code>dist/1.0.0+1/hello_world-1.0.0+1-android.apk</code></td><td>true</td></tr><tr><td><code>--targets</code></td><td>Comma separated list of maker publishers</td><td>true</td></tr></tbody></table>

示例：

```
flutter_distributor publish --path dist/1.0.0+1/hello_world-1.0.0+1-android.apk --targets fir,pgyer
```
