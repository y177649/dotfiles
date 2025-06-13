# dotfiles

このリポジトリは、開発環境を構成するための設定ファイルを管理するものです。

## 概要

このリポジトリには、日常的に使用するツールやアプリケーションの設定ファイルが含まれています。<br>
新しい環境をセットアップする際や、複数のマシンで設定を同期するために使用します。

## 動作環境

* **OS:** Ubuntuでの使用を想定しています。
* **必要なコマンド:**
    * `git`
    * `mv` (ファイルの移動・名前の変更)
    * `ln -s` (シンボリックリンクの作成)
 
## セットアップ方法

リポジトリをクローンします。(ssh)
```bash
git clone git@github.com:y177649/dotfiles.git ~/dotfiles
```

元のファイルをバックアップにします。（.bashrcの場合）
```bash
mv ~/.bsshrc ~/.bashrc.bak
```

シンボリックリンクを作成します。（.bashrcの場合）
```bash
ln -s ~/dotfiles/.bashrc ~/.bashrc
```

設定を環境に適応する（.bashrcの場合）
```bash
source ~/.bashrc
```
