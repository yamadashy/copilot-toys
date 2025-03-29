# CopilotToys

Copilotを利用したmarkdownベースのDevToys的なテキスト処理・変換ツールコレクション

## 概要

このリポジトリはGitHub Copilotの補完を使って、[DevToys](https://github.com/veler/DevToys) のように開発者をサポートするマークダウン形式のツール集です。

`.private/` ディレクトリなど、グローバルな `.gitignore` に含まれる非追跡ディレクトリに配置して使用することを想定しています。

## 使い方

1. このリポジトリを任意の場所にクローンするか、必要なマークダウンファイルをコピーします
2. ファイルをプロジェクトの `.private/` ディレクトリなどに配置します
   ```bash
   # 例: プロジェクトのルートディレクトリに .private ディレクトリを作成し、そこにファイルをコピー
   mkdir -p /path/to/your/project/.private
   cp -r /path/to/copilot-toys/* /path/to/your/project/.private/
   ```
3. 任意のmarkdownファイルを開き、Copilotの補完機能を使用してツールを利用します

## ツール

### translate.md
日本語⇔英語の翻訳を技術文書に最適化して行うためのテンプレートです。専門用語や技術的な文脈を考慮した翻訳を支援します。

### date-convert.md
様々な日付形式をISO 8601標準形式に変換するためのツールです。日本時間(JST)やUTCでの表記など、タイムゾーンの変換にも対応しています。

### commit-message.md
コミットメッセージを日本語から英語に翻訳するためのテンプレートです。Conventional Commitsに準拠した形式への変換をサポートします。
