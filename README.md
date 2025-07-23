# blog-mura-patrol

![Java](https://img.shields.io/badge/language-Java-blue)
![Gradle](https://img.shields.io/badge/build-Gradle-02303A?logo=gradle)
![License](https://img.shields.io/badge/license-MIT-green)

## 📝 概要

このツールは [ブログ村](https://blogmura.com) に自動ログインし、指定されたURLにアクセスする Java + Selenium プログラムです。ブログの巡回やクリック処理などを自動化することが目的です。

---

## 💻 使用技術

- Java 21
- Gradle
- Selenium WebDriver
- ChromeDriver

---

## 🔧 セットアップ方法

1. **リポジトリをクローン**

   ```bash
   git clone https://github.com/IchikabuImpact/blog-mura-patrol.git
   cd blog-mura-patrol
   ```
以下の3つのテキストファイルをプロジェクトルートに置いてください。

email.txt：ログイン用メールアドレス

password.txt：パスワード

url.txt：アクセスしたいブログページのURL

ChromeDriver の準備

exe/chromedriver.exe を設置。バージョンは Google Chrome本体と一致するもの を使用してください。

※ 自動管理に切り替える予定なら WebDriverManager などの導入を検討ください。

ビルドと実行

bash
コピーする
編集する
gradle build
gradle run
📁 ディレクトリ構成
bash
コピーする
編集する
```
blog-mura-patrol/
├── app/                  # Gradleアプリ用ディレクトリ（初期テンプレート）
├── src/                  # Main.java が含まれるディレクトリ
├── exe/                  # ChromeDriver配置先
├── lib/                  # 必要に応じてjar依存を置く
├── email.txt             # メールアドレス
├── password.txt          # パスワード
├── url.txt               # 対象URL
├── build.gradle.kts      # Gradleビルド定義（Kotlin DSL）
├── settings.gradle.kts
└── README.md             # このファイル
```
⚠️ 注意事項
email.txt, password.txt, url.txt など個人情報を含むファイルはGitにコミットしないでください。

.gitignore により安全に除外されるようになっています。

📄 ライセンス
本リポジトリは MITライセンス のもとで公開されています。

🤝 貢献
バグ報告・提案・プルリクエストを歓迎します！
