# 日付形式の変換ツール

このテンプレートはさまざまな日付形式をISO 8601標準形式に変換するためのものです。

## 変換セクション

### 元の日付形式

ここに変換したい日付を入力してください。
タイムゾーンのオフセットが付いていないものは未定義のままとなります。
例: 2023年4月1日 15時30分45秒
例: 01/04/2023 15:30:45

```text
```

### ISO 8601形式

日本時間に変換されたISO 8601形式の日付がここに出力されます。

```text
```

UTCに変換されたISO 8601形式の日付がここに出力されます。

```text
```

------

## ISO 8601形式について

ISO 8601は国際的に認められた日付と時刻の表記規格です：

- 基本形式: `YYYY-MM-DDThh:mm:ss±hh:mm`
  - YYYY: 年（4桁）
  - MM: 月（2桁）
  - DD: 日（2桁）
  - T: 日付と時刻の区切り文字
  - hh: 時（24時間形式、2桁）
  - mm: 分（2桁）
  - ss: 秒（2桁）
  - ±hh:mm: タイムゾーンオフセット（UTC基準）

- 例：
  - `2023-04-01T15:30:45+09:00`（日本標準時、JST）
  - `2023-04-01T06:30:45Z`（協定世界時、UTC）- ZはUTCを示す

## 変換ルール

Copilotを使用して以下のような変換ができます：

1. 様々な形式の日付をISO 8601形式に変換
  - 日本語の日付表記 → ISO 8601
  - 米国式の日付表記 → ISO 8601
  - 欧州式の日付表記 → ISO 8601

2. ISO 8601形式から他の形式への変換
  - ISO 8601 → 日本語の日付表記
  - ISO 8601 → 米国式の日付表記
  - ISO 8601 → 欧州式の日付表記

3. タイムゾーン調整
  - ローカル時間 → UTC
  - UTC → ローカル時間（指定したタイムゾーン）

## 使用例

### 例1: 日本の日付形式からISO 8601への変換

**入力:**
```
2023年4月1日 15時30分45秒
```

**出力:**
```
2023-04-01T15:30:45+09:00
```

### 例2: 一般的な日付形式からISO 8601への変換

**入力:**
```
01/04/2023 15:30:45
```

**出力:**
```
2023-04-01T15:30:45+09:00
```
