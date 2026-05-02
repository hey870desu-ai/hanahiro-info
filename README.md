# hanahiro-info

株式会社はなひろの**対外向け資料サイト**（会社概要・各事業所PR・送迎エリアマップ等）。

公開URL: https://info.hana-hiro.com/

## ページ一覧

- `company.html` … 会社概要
- `poem-asaka.html` … poem de riha 安積店 PR資料（2026年6月OPEN）
- `sougei-area-asaka.html` … 安積店 送迎エリア対話型マップ
- `sougei-areas.html` … 全事業所の送迎エリア一覧

## 関連リポジトリ

- `hanahiro-training` … 社内研修「学びの広場」（社内専用、ドメイン分離）

## デザイン規約

- 見出しフォント: Cormorant Garamond + Noto Serif JP
- 本文フォント: Noto Sans JP
- カラー: ink #1f2933 / gold #a87827
- 印刷: A4 横ランドスケープ、各セクションを 297×210mm の独立ページに分割

## 送迎エリアマップ生成

```sh
ORS_API_KEY=eyJ... python3 tools/generate-isochrone-map.py
```

出力: `photos/sougei-area-{slug}.png`
