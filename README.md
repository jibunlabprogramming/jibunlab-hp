# じぶんラボ 公式サイト

個別指導プログラミング じぶんラボ の公式サイトです。GitHub Pages で配信しています。

- 公開URL: https://jibunlabprogramming.github.io/jibunlab-hp/
- 1ページ完結。`index.html` と `assets/` だけで動きます。ビルドは不要です。

## このリポジトリは公開です

**履歴を含めて誰でも見られます。** 次のものは絶対に置かないでください。

- アカウント情報、パスワード、リカバリーコード
- 本名、自宅の住所、電話番号、個人番号
- 帳簿、証憑、税務書類、生徒や保護者の情報

事業の資料はすべて、別の非公開リポジトリ `jibunlabprogramming/jibunlab` にあります。

## 直すとき

```
cd /home/takashi/develop/jibunlab-hp
# index.html を編集
git add -A
git commit -m "変更の内容"
git push
```

push すると、1〜2分で公開サイトに反映されます。

## メモ

- `<meta name="robots" content="noindex">` を入れているため、検索エンジンには載りません。検索から集客する段階になったら、この1行を消します。
- 教材を試せるデモは `05_教材/00_共通/htmlエディタ/index.html`(非公開リポジトリ側)を縮めたものです。教材を直したときは、こちらのテンプレートも見直してください。
- デザインは非公開リポジトリ側の `05_教材/00_共通/デザイン案/デザインガイド_ラボ.md` に従っています。
