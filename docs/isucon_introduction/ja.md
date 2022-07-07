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

### A. 例: **RTT(往復レイテンシ)** が短いと高速なWebサービス (P.4より引用)

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

- 推測せず計測する (P.13)
  - データを出発点とすることで、理論や知識を適切に利用する
- 公平に1つずつ比較する (P.13, 14)
  - ノイズが混ざらないよう注意し、対策1つごとに計測を繰り返す
- ボトルネックだけにアプローチする (P.15)
  - 制約理論(全体のスループットはボトルネックに律速するという考え方)はWebサービスの高速化にも当てはまる
- 負荷試験と上記に基づいた分析、改善を繰り返す (P.18)

---

<!--
_class: lead
-->
## Q. **分析して改善しろ**と軽く言ってくれるけど
## どうりゃいいのよ

---

### A. まずボトルネックを**探して**、**解消する**

※ ここではコマンドの詳細については割愛します

1. ボトルネックの特定

2. 

例) MySQLの場合
1. 

---

### A. 次にボトルネックを**解消する**

---
# 参考

- [Webパフォーマンスチューニングに関する情報源まとめ（随時更新）](https://zenn.dev/sugamaan/articles/4e57703fe661bb)
- [スピードが重要な理由とは？](https://web.dev/why-speed-matters/)
- [パフォーマンスを特徴付ける条件 - IBM Documentation](https://www.ibm.com/docs/ja/zos/2.2.0?topic=tuning-how-is-performance-characterized)
- [阿部寛のサイトを高速化する - Qiita](https://qiita.com/Morix1500/items/0eac072a027d478a6b83)

---
**※ 蛇足**
因みにこのスライドは **Marp** というMarkdownをスライドに起こせるツールを使用して作りました。
VSCode拡張を使うとプレビューしながら手軽にMarkdownでのスライド作成が出来るのでオススメです。

![bg right:40% height:280](../img/marp_intro.png)

参考
- [「Marp」【レビュー】 - 窓の杜](https://forest.watch.impress.co.jp/docs/review/1422278.html)
- [sample-presentation.pdf](https://ktkr3d.github.io/images/sample-presentation.pdf)
---

**※ さらに蛇足**
また、本スライドはGithubで管理しています。
https://github.com/daylight55/slide/tree/main
GithubActionsでmarp-cliを連携すると、GithubPagesに自動でスライドを公開することも可能で、スライド運用が渋るのでオススメです。

![height:250](../img/slide_repo.png) ![height:250](../img/slide_actions.png)
