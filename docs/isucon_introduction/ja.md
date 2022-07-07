---
marp: true
paginate: true
theme: gaia
footer: "**2022/07/07 by @daylight55**"
---

<!--
_class: lead
-->
# ISUCON本から学ぶ
# Webパフォーマンスチューニング
## 〜基礎編〜

---

# ISUCON本
![bg right 80% ](../img/isucon_book.jpeg)

- ISUCONを例に、実務に役立つパフォーマンスチューニング手法について解説
- モニタリング、負荷試験の方法についても解説
- DB、キャッシュ、リバプロ、OSなどそれぞれのチューニング手法で章立て
- [書籍案内｜技術評論社](https://gihyo.jp/book/2022/978-4-297-12846-3)

---
<!--
_class: lead
-->
## Q. なぜ**パフォーマンスチューニング**が必要
## なのでしょうか？

---

### A. "高速であること"は現代のWebサービスの必須要件であるから (P.2より引用)
Webサービスが高速だと、以下のメリットが得られます。

- 単位時間あたりの操作可能回数が増える
- 高いUXが得られる
- SEOに効果がある
- 高コスト効率を実現できる

---

<!--
_class: lead
-->
## Q. どうなっていると**高速なWebサービス**
## なのでしょうか？

---

### A. 例: **RTT(往復レイテンシ)** が短いWebサービス       (P.4より引用)

また、大規模なサービスになるほど、スループットを上昇させることが重要になってきます。

- **RTT** : Webサービス利用者のリクエスト送信開始 〜 Webサービス利用者のレスポンス受信完了までの所要時間)
- **レイテンシ** : 発信したデータが相手に届くまでの待機時間 (レイテンシのみだと基本的に片道を意味する)
- **スループット**: 同時並行処理性能。単位は、単位時間あたりのリクエスト処理数 rps (requests per second)

---

<!--
_class: lead
-->
![bg opacity:.3 blur:10px](../img/abe_hp.png)
## [WebPageTestを使うと詳細な計測結果](https://www.webpagetest.org/result/220706_AiDc25_6PJ/)が得られます。

---

## パフォーマンスチューニングの基本

- 

---

## A. サービス競争に優位に立てるから

- 高速は SEO に効果あり

- 
  https://web.dev/why-speed-matters/

---
<!--
_class: lead
-->
## 速くしろとか簡単に言ってくれるけど
## どうすりゃいいのさ

---

# **分析と改善**を繰り返す

例) RDBMSの場合

---
# 参考

- [Webパフォーマンスチューニングに関する情報源まとめ（随時更新）](https://zenn.dev/sugamaan/articles/4e57703fe661bb)
- [スピードが重要な理由とは？](https://web.dev/why-speed-matters/)

---
**※ 蛇足**
因みにこのスライドは **Marp** というMarkdownをスライドに起こせるツールを使用して作りました。
VSCode拡張を使うと手軽にMarkdownでのスライド作成が出来るのでオススメです。

![bg right:40% height:280](../img/marp_intro.png)

参考
- [「Marp」【レビュー】 - 窓の杜](https://forest.watch.impress.co.jp/docs/review/1422278.html)
- [sample-presentation.pdf](https://ktkr3d.github.io/images/sample-presentation.pdf)
---

**※ さらに蛇足**
本スライドはGithubで管理しています。
https://github.com/daylight55/slide/tree/main
GithubActionsでmarp-cliを連携すると、GithubPagesに自動でスライドを公開することも可能で、スライド運用が渋るのでオススメです。

![height:250](../img/slide_repo.png) ![height:250](../img/slide_actions.png)
