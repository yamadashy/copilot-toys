# コミットメッセージ翻訳ツール

このテンプレートはコミットメッセージを日本語⇔英語間で変換するためのものです。Conventional Commitsの形式に準拠した翻訳を行います。

## 変換セクション

### 日本語のコミットメッセージ
ここに日本語のコミットメッセージを入力してください
例: feat(認証): ユーザー登録フォームにパスワード強度チェックを追加

```text
```

### 英語のコミットメッセージ

ここに英語に翻訳されたコミットメッセージが表示されます
例: feat(auth): add password strength check to user registration form

```text
```

---

## Conventional Commitsについて

[Conventional Commits](https://www.conventionalcommits.org/ja/v1.0.0/) は、コミットメッセージに人間と機械が読みやすい意味を付与するための仕様です。

基本構造:
```
<type>[(scope)]: <description>

[body]

[footer(s)]
```

主な型（type）:
- `feat`: 新機能
- `fix`: バグ修正
- `docs`: ドキュメントのみの変更
- `style`: コードの意味に影響しない変更（スペース、フォーマット等）
- `refactor`: バグ修正や機能追加ではないコード変更
- `perf`: パフォーマンス向上のための変更
- `test`: テストの追加・修正
- `build`: ビルドシステムや外部依存に関する変更
- `ci`: CI設定ファイルやスクリプトの変更
- `chore`: その他の変更（補助ツール、ドキュメント生成など）

## コミットメッセージの参考ログ

`git log --oneline` の一部:

```
4b628e1 chore(website): Add .tool-versions to specify Node.js version for Cloudflare Pages
76d625e feat: enhance repository name validation and expose validation function
429081b docs(readme): add Gitingest as an alternative tool for Python users
9ecb902 docs(readme): Improve Discord section and add icons to headings in README
76904c9 feat(website): Add configurable token count encoding and change default to o200k_base
a40b2d7 feat(fileSearch): use config.cwd instead of process.cwd() for better testability
5ce74ca feat(website): Swap navigation link positions for better visibility
3d7ffbe Merge pull request #249 from yamadashy/feat/website-include-pattern
42401bb feat(cli): Add CLI flags for controlling output sections and content processing
b453f3d fix(instruction): use current working directory for instruction file path
```

## 翻訳のポイント

1. **型（type）と範囲（scope）の維持**:
  - `feat(auth)` → `feat(auth)` のように型と範囲は翻訳せず維持
  - 範囲は英語の場合は小文字で、日本語の場合はそのまま

2. **簡潔さの維持**:
  - 英語の場合、通常は命令形の動詞で始める（add, update, fix, remove など）
  - 日本語の場合、体言止め（「追加」「更新」「修正」「削除」など）も可

3. **一貫性**:
  - リポジトリの既存のコミットスタイルに合わせる
  - 参考ログのパターンを分析して同様の表現を使う
