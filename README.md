# ai-common

Shared AI command definitions and generators for Claude, Gemini and GitHub workflows.

## セットアップ

### 新規プロジェクトに追加する場合

```bash
git submodule add https://github.com/KobayashiYoh/ai-common.git ai-common
git submodule update --init --recursive
```

### 既存プロジェクトのサブモジュール初期化

```bash
git submodule update --init --recursive
```

## 更新方法

ai-common リポジトリが更新された場合、サブモジュール参照を同期する必要があります。

### ai-common のみを最新版に更新

```bash
git submodule update --remote ai-common
```

### メインプロジェクトとサブモジュールを同時に更新

```bash
git pull --recurse-submodules
```

## ディレクトリ構成

```
ai-common/
├── commands/        # Claude Code のカスタムコマンド定義（.md ファイル）
├── scripts/         # 実行可能なシェルスクリプト
│   └── github/      # GitHub API を利用したスクリプト
└── LICENSE
```
