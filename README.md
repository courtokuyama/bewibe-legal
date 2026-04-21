# bewibe-legal — ARCHIVED

⚠️ **このリポジトリは 2026-04 以降アーカイブ状態です。**

## 現状

TUUN の公開中の法的文書（Privacy Policy / Terms of Service / Support）の**正本 (canonical source)** は:

- **公開先:** `https://tuunclub.com/pages/privacy-policy` / `/terms` / `/privacy-policy-en` / `/terms-en` / `/support-en`
- **Canonical source:** `~/shopify-work/sections/tuun-*.liquid`（Shopify テーマの section ファイル）

**このリポジトリの HTML ファイルは編集しても live サイトに反映されません。** 過去に GitHub Pages で配信していた名残です。

## 更新手順（忘れないように）

```bash
# 1. ~/shopify-work/sections/tuun-<page>.liquid を編集
# 2. push
shopify theme push --theme 152211226764 --only "sections/tuun-<page>.liquid" --allow-live --force

# 3. 検証
cd /tmp && shopify theme pull --theme 152211226764 --only "sections/tuun-<page>.liquid" --nodelete
```

## このリポを消していない理由

- 過去バージョンのスナップショットとして残す（git 履歴に価値あり）
- GitHub Pages 戻す可能性がゼロではない

編集禁止。Shopify 側で完結させる。
