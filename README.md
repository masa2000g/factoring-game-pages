# 因数分解マスター

中学生向けの因数分解練習ゲームです。ブラウザだけで動作する静的サイトとして構成されています。

## 概要（OGP用）

> 中学生向けの因数分解練習ゲーム。共通因数くくり出し・展開の逆・二乗公式・たすきがけなど、レベル別に因数分解の問題に挑戦して数学力を鍛えよう！

## レベル構成

| レベル | 内容 | 例 |
|--------|------|----|
| Lv.1 | 共通因数でくくる | 6x² + 12x → 6x(x+2) |
| Lv.2 | 展開の逆 | x² + 5x + 6 → (x+2)(x+3) |
| Lv.3 | 二乗の公式・和と差の積 | x² − 9 → (x+3)(x−3) |
| Lv.4 | たすきがけ | 2x² + 7x + 3 → (2x+1)(x+3) |
| Lv.5 | 全レベルからランダム出題 | — |

## GitHub Pages での公開方法

1. このリポジトリを GitHub にプッシュする
2. リポジトリの **Settings** → **Pages** を開く
3. **Source** で `Deploy from a branch` を選択
4. **Branch** で `main` / `/ (root)` を選択して **Save**
5. 数分後に `https://<username>.github.io/<repo-name>/` で公開される

```bash
# リモート追加とプッシュの例
git remote add origin git@github.com:<username>/factoring-game.git
git push -u origin main
```

## ローカルでの確認

```bash
# Python の場合
python3 -m http.server 8000

# Node.js の場合
npx serve .
```

ブラウザで `http://localhost:8000` を開く。

## 技術構成

- **単一ファイル構成** — `index.html` のみ（HTML + CSS + JavaScript）
- 外部依存なし（CDN・ライブラリ不要）
- モバイル対応（レスポンシブデザイン）
- バックエンド不要（完全クライアントサイド）

## ライセンス

MIT
