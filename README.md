# Aimstar Push Notification Sdk

## 導入ガイド

1. ライブラリの追加
xxxx-release.aarファイルををapp/libs直下に配置してください。
xxxx-release.aarファイルは本サンプルプロジェクトのapp/libsに入っております。

2. build.gradleの設定
appレベルのbuild.gradleに以下を追加する。
```
dependencies {
    :
  implementation fileTree(dir: "libs", include: ["*.jar", "*.aar"])   // ★追加
  implementation(name: 'xxxx-release', ext: 'aar')  // ★追加
    :
}
```

3. Gradleの同期
Android Studioのメニュー File -> Sync Project with Gradle Files にてGradleを同期する。
