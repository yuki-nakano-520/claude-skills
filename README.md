# claude-skills

自作の Claude Code スキル集。

| スキル | 内容 |
|---|---|
| [marp-slides](marp-slides/SKILL.md) | Marp でスライドを作成・整形し、PNG に書き出して崩れを確認する。テーマ（`assets/career.css`）、スタイルガイド、レイアウト型カタログ付き |

## インストール

`~/.claude/skills/` にスキルのディレクトリをリンクする。

Windows（PowerShell、管理者権限不要のジャンクション）:

```powershell
New-Item -ItemType Junction -Path "$HOME\.claude\skills\marp-slides" -Target "$HOME\work\claude-skills\marp-slides"
```

macOS / Linux:

```bash
ln -s ~/work/claude-skills/marp-slides ~/.claude/skills/marp-slides
```

## marp-slides の考え方

- スタイルは「なんとなく良い感じ」ではなくルールとして決める
- レイアウトは毎回作らず、型のカタログから選ぶ
- コードが正しくても見た目が正しいとは限らないので、画像に書き出して確認する
- 中身は本人の言葉で書き、AI は構造と見た目を担当する
