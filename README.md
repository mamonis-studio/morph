# MORPH

**一括画像フォーマット変換ツール / Batch Image Format Converter**

ブラウザで完結する画像変換。アップロードなし、制限なし、完全ローカル処理。

A privacy-first batch image converter. No uploads, no limits, runs entirely in your browser.

## Features

- **完全ローカル処理** — サーバーへのアップロード一切なし。すべてブラウザ内で完結
- **ファイル数制限なし** — 10枚でも10,000枚でも。課金も上限もなし
- **HEIC/HEIF対応** — iPhoneの写真をそのまま変換可能
- **5形式に出力** — JPEG / PNG / WebP / AVIF / BMP
- **9形式を入力** — JPEG / PNG / WebP / AVIF / GIF / BMP / TIFF / SVG / HEIC
- **品質調整** — JPEG・WebP・AVIFの圧縮率をスライダーで指定
- **リサイズ** — 幅・高さ指定、アスペクト比ロック対応
- **メタデータ制御** — EXIF・GPS情報の削除/保持を切り替え可能
- **ZIP一括ダウンロード** — 変換済みファイルをまとめてダウンロード
- **日本語/英語切り替え** — UIの即時言語切り替え対応

## Tech Stack

- Vanilla HTML / CSS / JavaScript（フレームワーク不使用）
- [heic2any](https://github.com/nicolo-ribaudo/heic2any) — HEIC/HEIFデコード
- [JSZip](https://stuk.github.io/jszip/) — ZIP生成
- [piexifjs](https://github.com/nicolo-ribaudo/piexifjs) — EXIF読み書き
- Cloudflare Pages — ホスティング

## Deploy

```bash
# 1. Clone
git clone https://github.com/mamonis/morph.git
cd morph

# 2. That's it. Open index.html or deploy to Cloudflare Pages.
```

Cloudflare Pages設定:
- ビルドコマンド: （空欄）
- 出力ディレクトリ: `/`

## Why MORPH?

既存の画像変換サービスの問題点:

| サービス | 問題 |
|---------|------|
| iLovePDF/iLoveIMG | 有料プランでもファイル数制限あり |
| Squoosh | 一括変換非対応、1枚ずつ手動 |
| CloudConvert | 無料枠が少なく、すぐ課金が必要 |
| その他オンラインツール | サーバーにファイルをアップロードする必要がある |

MORPHはこれらの問題をすべて解決する。ローカル処理で制限なし、無料。

## License

MIT

## Author

[Mamonis Studio](https://mamonis.studio)
