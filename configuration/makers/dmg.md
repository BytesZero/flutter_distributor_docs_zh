# dmg

{% hint style="warning" %}
You can only build the DMG target on macOS machines.
{% endhint %}

## 用法

将 `distribute_options.yaml` 添加到你的项目 `macos/packaging/dmg` 目录。

```yaml
title: hello_world
contents:
  - x: 448
    y: 344
    type: link
    path: "/Applications"
  - x: 192
    y: 344
    type: file
    path: hello_world.app
```

运行：

```
flutter_distributor package --platform macos --targets dmg
```
