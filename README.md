# ghostty-config

macOS 用の [Ghostty](https://ghostty.org/) ターミナル設定ファイル群です。

## ファイル一覧

| ファイル名 | 説明 | 元パス |
| :--- | :--- | :--- |
| **`config`** | **①と②を統合・整理した設定ファイル（推奨）** | 統合版 |
| **`config.xdg`** | ① カスタム設定（`TokyoNight` / `PlemolJP35 Console NF` / Quick Terminal / 分割移動キーバインド等） | `~/.config/ghostty/config` |
| **`config.ghostty`** | ② コメント付き基本設定（`Catppuccin Mocha` / `Menlo` / 余白・マウス・操作設定等） | `~/Library/Application Support/com.mitchellh.ghostty/config.ghostty` |

## 使い方（セットアップ）

統合版の `config` を使う場合は、`~/.config/ghostty/config` に配置します。

```bash
mkdir -p ~/.config/ghostty
cp config ~/.config/ghostty/config
```

> **Note:** macOS では `~/Library/Application Support/com.mitchellh.ghostty/config.ghostty` が存在すると、`~/.config/ghostty/config` の後に読み込まれて設定が上書きされるため、1つのファイルで管理する場合は `Application Support` 側のファイルを削除またはリネームしてください。
