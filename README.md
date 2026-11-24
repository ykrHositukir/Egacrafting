# Notch (Markus Persson) — Scroll Site (実画像版)

PPT(6枚)の**実画像をそのまま**縦スクロールで見るWebサイトです。
スライドの再現・作画は一切していません。

## 特徴
- 各スライド = 提供された画像を画面いっぱいに表示(追加テキストなし)
- CSSアニメーション:
  - スクロールでスライドが見えると、画像がふわっと現れゆっくりズーム(Ken Burns)
  - 画像レイヤーがスクロールに合わせてほんのり浮遊(パララックス)
  - 材料(草🟩・葉🍃・木材🪵・ダイヤ💎・金🟨・TNT🧨)が純CSSアニメーションで降り続く
  - スライド1にスクロールを促すヒント表示
- スライド間はグラデーションで境目なし
- 単一 `index.html` / 外部ライブラリ不要
- `prefers-reduced-motion` 対応

## 公開方法(GitHub Pages)
1. リポジトリの **Settings → Pages**
2. Source: **Deploy from a branch** / Branch: `main` / フォルダ: `(root)` → **Save**
3. 数分後 `https://ykrhositukir.github.io/Egacrafting/` で公開されます

## Note
6枚のスライド画像はチャットCDNのURL(期限付きトークン付き)を直接参照しています。
長期運用する場合は各画像をダウンロードして `assets/slide1.png`〜`slide6.png` などに保存し、
`index.html` 内の各 `<img class="bg">` の `src` を差し替えてください。
