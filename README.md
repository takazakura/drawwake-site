# drawwake-site

MuscleFlip のアプリの公開サイト。
DrawWake の紹介ページ、プライバシーポリシー（6言語）、サポート（6言語）、利用規約。

| ページ | URL |
|---|---|
| 開発者トップ | https://takazakura.github.io/drawwake-site/ |
| DrawWake 紹介 | https://takazakura.github.io/drawwake-site/drawwake/ |
| プライバシーポリシー | https://takazakura.github.io/drawwake-site/drawwake/privacy.html |
| サポート | https://takazakura.github.io/drawwake-site/drawwake/support.html |
| 利用規約 | https://takazakura.github.io/drawwake-site/drawwake/terms.html |

## 編集方法

**このリポジトリの HTML を直接編集しないこと。** 生成物なので次回の生成で上書きされる。

本体は非公開リポジトリ `DrawWake` の `website-src/` にある。
プライバシーポリシーとサポートの文章は `docs/legal/*-multilang.md` から生成している。
そちらを直して以下を実行する。

    python3 website-src/build.py .
    bash deploy-site.sh
