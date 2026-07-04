# CHANGELOG

新しい更新を上（先頭）に追記します。

---

## 2026-07-05 — GitHub リモート連携と初回プッシュ、CHANGELOG 追加

### 何をしたか
- GitHub リモート `origin` を追加し、`main` ブランチを初回プッシュ。
  - リポジトリ: https://github.com/minaco6311/lesson2_agatha_timeline
- 変更記録用の `CHANGELOG.md` を追加・コミット。

### 実行したプロンプト（再現用）
1. 「git remote add origin https://github.com/minaco6311/lesson2_agatha_timeline.git」
2. 「git push -u origin main」
3. 「CHANGELOG.md お願いします」（CHANGELOG.md のコミット＆プッシュ依頼）

---

## 2026-07-05 — アガサ・クリスティ紹介ページの初回作成 (commit: 3d9ac1b)

### 何をしたか
- **index.html**: アガサ・クリスティの作品タイムライン紹介ページを新規作成。
  - `Famous works Timeline` の見出しを、タイトル上から「Agatha Christie」下の白いライン区切りの下へ移動。フォントを Cinzel（タイトルと同じ）に統一し、サイズはタイトルの約40%（`text-2xl md:text-4xl`）、字間広め・大文字で上品に調整。
  - 締めセクションに肖像写真 `images.jpeg` を追加。並び順は上から「The End」→ 写真 → 縦のグラデーション線。写真はモノクロ表示でホバー時にカラーになる演出、角丸＋影＋白細枠付き。
- **CLAUDE.md**: commit/push 時に変更要点と実行プロンプトを CHANGELOG.md へ記録するルールを追加。
- **images.jpeg**: アガサ・クリスティの肖像写真を追加。

### 実行したプロンプト（再現用）
1. 「CLAUDE.mdを作りそこに下記の内容を書き込んでください。commit、push したら、変更内容の要点を CHANGELOG.md にまとめて記録する。後で見ても、誰が見ても『何をしたか』が分かり、再現できるように記録すること。次に再現できるように、実行したプロンプトも残すこと。CHANGELOG.md は、新しい更新が上（先頭）に来るように記録する。」
2. 「Famous works Timeline を AGATHA CHRISTIE の下の白いラインが引いてある下に持ってきて。AGATHA CHRISTIE と同じフォントで文字の大きさは AGATHA CHRISTIE 40％くらいでちょっとおしゃれにして」
3. 「Agatha Christie (1890–1976) / The End の下に アガサクリスティの写真を小さく入れて」
4. 「THE END の下にして縦の棒のグラデーションはその下に」
5. 「git add .」→「git commit」
