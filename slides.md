---
# You can also start simply with 'default'
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: ペチオブLT会
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# take snapshot for each slide in the overview
overviewSnapshots: true
fonts:
  # basically the text
  sans: 'Helvetica Neue,Robot'
  # use with `font-serif` css class from windicss
  local: 'Helvetica Neue'
  # for code blocks, inline code, etc.
  mono: 'Fira Code'
---

# お手元のターミナル環境を<br>お手軽にかっこよくする

2024/10/03 @ucan-lab
【ペチオブ LT 会】オフラインでわいわい LT & 交流会【YouTube 視聴もできるよ】

---

# 自己紹介

- [@ucan_lab](https://x.com/ucan_lab) (ゆうきゃん)
- 所属: ミライトデザイン
- エンジニア歴: 15年
- 好きな言語/フレームワーク: PHP/Laravel
- 趣味: HADO(OK/KO HADO公認チームに所属)

<img src="/qiita.png" class="h-50">

---
layout: image
image: /hado.jpg
---

---

# ターミナル環境について

Macのターミナル環境をデフォルトの白い画面のままで使ってないですか？

<img src="/terminal-default.png" class="h-80">

---

# ターミナルとは

![](/terminal-shell.webp)

---

# ターミナルアプリ

- 純正Terminal
- iTerm2
- Alacritty
- Hyper
- Warp
- 等々...

---
layout: image-right
image: /terminal-warp.png
backgroundSize: contain
---

## ターミナル - Warp

開発者向けに設計された次世代ターミナル！(Windowsも対応予定...)

- コマンドパレット
- コマンド履歴検索
- コマンド入力補完
- AI検索機能

![](/warp.png)

---

# シェル

- zsh
- bash
- sh
- csh
- ksh

2019年のmacOS Catalinaでbashからzshに標準シェルが変更されました。

- ~/.zshrc 設定ファイル
  - エイリアスの作成
  - 環境変数の設定
  - プラグインの導入
  - テーマの変更
  - 等々

---

# プロンプト

プロンプトはコマンド入力の際に表示されるシェルのインターフェース

```shell
ユーザー名@ホスト名 カレントディレクトリ名 % 
```

---
layout: image-right
image: /terminal-warp.png
backgroundSize: contain
---

## Warp - プロンプト

Warpのプロンプトは標準でディレクトリのパス、Gitのブランチ名、差分ファイル数を表示

![](/warp-prompt.png)

---

# フォント

- Hack (デフォルト)

Warpを使用する場合、デフォルトがHackなので拘りがなければそのままでokです。
個人的にはこちらのフォントが好きです。

- Fira Code
- 0xProto

---

## Hack

![Hack](/font-hack.png)

---

## Fira Code

![Fira Code](/font-fira-code.png)

---

## 0xProto

![0xProto](/font-0xproto.png)

---

# Warp - テーマ

Dracula
https://draculatheme.com/warp

![dracula](/theme-dracula.webp)

# その他

ターミナルがちょっと便利になるツールを紹介！

---

## Rust製ツール ripgrep

- grep → ripgrep

```
# grep
grep -r --exclude-dir={node_modules,vendor} 'TODO' .

# ripgrep (rg)
rg 'TODO'
```

ripgrepはデフォルトで.gitignoreに従う
ripgrepはデフォルトでリカーシブ検索する

```
# grep
grep --color=always 'error' logfile.txt

# ripgrep
rg 'error' logfile.txt
```

Ripgrepはデフォルトで色付きの結果を返す
また、grepよりripgrepの方が検索パフォーマンスが高いです。

---

## Rust製ツール fd

```
# find
find . -name "*.txt"

# fd
fd '*.txt'
```

- fd はカレントディレクトリ(`.`)省略可
- fd はデフォルトでファイル名検索する
- fd はデフォルトで.gitignoreに従う

fdはデフォルトで色付きの結果を返す
また、findよりfdの方が検索パフォーマンスが高いです。

---

## Rust製ツール zoxide

```
# cd
cd /Users/username/Documents/projects/laravel_app

# zoxide
z laravel
```

---
layout: center
---

# おしまい

---

# 一緒にHADOやろうze！

![](/hado.jpg)
