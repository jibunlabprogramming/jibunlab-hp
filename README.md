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

## OGP画像(リンクのプレビュー)

LINEやInstagramのDMでURLを送ったときに出るカードの画像です。

- 画像: `assets/ogp.png`(1200×630)
- もとのページ: `tools/ogp.html`

文面や料金を変えたら、`tools/ogp.html` を直して撮り直してください。

```
cd /home/takashi/develop/jibunlab-hp
google-chrome --headless --no-sandbox --disable-gpu --hide-scrollbars \
  --virtual-time-budget=15000 --window-size=1200,630 \
  --screenshot=assets/ogp.png tools/ogp.html
```

フォント(Zen Maru Gothic)は `~/.local/share/fonts/jibunlab/` に入れてあります。
別のPCで作り直すときは、先に <https://github.com/google/fonts/tree/main/ofl/zenmarugothic>
から TTF を取って `fc-cache -f` で登録してください。入っていないと、別のフォントで
描かれてしまいます。

## メモ

- `<meta name="robots" content="noindex">` を入れているため、検索エンジンには載りません。検索から集客する段階になったら、この1行を消します。
- 教材を試せるデモは `05_教材/00_共通/htmlエディタ/index.html`(非公開リポジトリ側)を縮めたものです。教材を直したときは、こちらのテンプレートも見直してください。
- デザインは非公開リポジトリ側の `05_教材/00_共通/デザイン案/デザインガイド_ラボ.md` に従っています。
