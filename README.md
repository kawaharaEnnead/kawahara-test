# kawahara-test

チームで Git / GitHub の操作を練習するためのリポジトリです。

## ファイル

| ファイル | 内容 |
| --- | --- |
| `1023に朝倉さんが送ったやつ.txt` | サイネージ演出整理のメモ |
| `members.md` | 練習用の名簿（自分の名前を追加してみよう） |

## 練習の流れ

1. 最新の main を取り込む

   ```sh
   git switch main
   git pull
   ```

2. 自分用のブランチを作る（名前は `practice/自分の名前` など）

   ```sh
   git switch -c practice/yourname
   ```

3. `members.md` に自分の名前と一言を追記する

4. 変更をコミットする

   ```sh
   git add members.md
   git commit -m "members.mdに名前を追加"
   ```

5. GitHub に push する

   ```sh
   git push -u origin practice/yourname
   ```

6. GitHub でプルリクエスト（PR）を作り、レビューしてもらってからマージする

## 注意

- main に直接コミット・push しないこと（必ずブランチ → PR）
- 困ったら `git status` で今の状態を確認する
