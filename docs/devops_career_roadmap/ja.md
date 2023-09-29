---
marp: true
paginate: true
theme: gaia
# footer: "**2023/09/28 by @daylight55**"
---

<!--
_class: lead
-->
# DevOpsのこれからと<br>Platform Engineering

2023/09/29

---

# DevOpsとは
![bg right vertical 100% ](../img/devops/devops.png)


- 「顧客に価値を素早く届けるため、開発・運用が協力する、文化的な姿勢・取り組み」のこと [^1]
- デプロイまでの流れを高速化し、開発・運用のサイロを取り除く文化が重要
- (企業によってポジショントークがあり、定義が異なるためややこしい)

[^1]: https://www.members-devopslead.com/service

---

# DevOpsの実践度

![bg right 70% 国内企業におけるDevOpsの実践状況の推移](../img/devops/devops_graph.png)

-  IDC Japanの調査によると、DevOpsの実践率は年々伸びている。 [^2]
- 2022年の調査では **59.3%** の実践率
- しかし、結論として「**ビジネス上の効果が得られている企業は増えていない**」とある。

[^2]: https://www.idc.com/getdoc.jsp?containerId=prJPJ49999523

---

<!--
_class: lead
-->
# DevOpsの**実践**は難しい

---

# 例:DevOps に求められる技術
![bg right 40%](../img/devops/devops_roadmap.png)

学習ロードマップとして

`Programming Language, OS, VCS, Containers, Cloud Providers, Network, Serverless, IaC, CI/CD Tool, GitOps, ServiceMesh etc...`

などが挙げられている。[^3]

[^3]: https://roadmap.sh/devops

---

# つまり、DevOpsを落とし込むと、、、

エンドユーザーに届けるまでに多くの技術が関わる

![80%](../img/devops/devops_into_organization.drawio.svg)

---
<!--
_class: lead
-->
# 開発者「こんなに意識しきれない・・・」

![bg vertical right 50% ](../img/devops/sick_noiroze_man.png)
![bg 50% ](../img/devops/sick_noiroze_woman.png)

---
# よくある導入

## DevOps Team Silo [^4]
- 「DevOpsチームを新しく作ったから、DevからOpsに渡るまでのセットアップはよろしく！」
- マイクロサービスごとにセットアップを任せられる。

![bg vertical right 120%](../img/devops/devops_antipattern_1.png)

[^4]: https://owasp.org/www-pdf-archive/Zero-to-DevSecOps-OWASP-Meetup-02-19-19_-_part_1.pdf

---
<!--
_class: lead
-->
# DevOpsチーム「管理しきれない・・・」

![bg vertical right 50% ](../img/devops/sick_noiroze_man.png)
![bg 50% ](../img/devops/sick_noiroze_woman.png)

---

<!--
_class: lead
-->
# デプロイ・運用までを<br>抽象化できるPlatformが必要

---

<!--
_class: lead
-->
# **Platform Enginieering**の需要

---

## Platform Enginieeringとは

![bg right 100%](../img/devops/platform_engineering_gartner.png)

- Garthnerの「先進テクノロジのハイプ・サイクル：2022年」で登場 [^5]
- 開発者体験と生産性を向上させるためにセルフサービスで利用できるツールチェーンとワークフローを設計・構築する分野 [^6]

[^5]: https://www.gartner.co.jp/ja/newsroom/press-releases/pr-20220816
[^6]: https://speakerdeck.com/jacopen/platform-engineeringhenozhao-dai?slide=8

---

# どう変わるのか
開発者は抽象化されたセルフサービス基盤(IDP)でデプロイする [^7]

![height:400](../img/devops/platform_into_organization.drawio.svg)

[^7]: https://speakerdeck.com/jacopen/platform-engineeringhenozhao-dai?slide=18

---

<!--
_class: lead
-->
# DevOpsや共通基盤を<br>言い換えただけでは？ 🧐

---
# Platform Enginieeringは何が違うのか

- 顧客 = 開発者 として、『価値』を届けることを重視する。
  - 価値: 開発者の認知負荷を軽減する
- **Platformを製品として**捉える。 => 『Platform as a Product』
- ゴールデンパスを用意する [^8]

事例
- [開発者向けの基盤をつくる - メルカリ](https://speakerdeck.com/tcnksm/kai-fa-zhe-xiang-kefalseji-pan-wotukuru)
- [ヤフーで KaaS ベースの PaaS ができるまで](https://www.docswell.com/s/ydnjp/ZDED1L-2023-03-06-151122#p1)

[^8]: https://cloud.google.com/blog/ja/products/application-development/golden-paths-for-engineering-execution-consistency

---
<!--
_class: lead
-->
# 開発者を補助するための内部Platformを一つの製品としてデザインする

---
<!--
_class: lead
-->

#  忘れてはならない<br>**DevOpsは文化**

---

![bg width:700 height:600](image.png) [^9]

[^9]: https://x.com/jacopen/status/1706218493262323940?s=20

---

# サイロと文化を改善する

- まず**己を知る**
  - 組織文化のモデル化と測定
  - [Westrum の組織類型](https://cloud.google.com/architecture/devops/devops-culture-westrum-organizational-culture?hl=ja)
- 

---

<!--
_class: lead
-->

#  Platformで組織の連携を加速させる
(具体例はまだ思い浮かびません 😢)


---

# 「やりたいことなんてない。これから見つけられるかどうかもわからない。でもみんながやりたいことがあるならそれを援護することはできる」

*SHIROBAKO ©「SHIROBAKO」製作委員*

![opacity:.4　bg cover](../img/devops/shirobako_support.jpg)

---

<!--
_class: lead
-->

# DevOposは愛❤️

---


**※ 蛇足**
このスライドは **Marp** というMarkdownをスライドに変換出来るツールで作っています。[^1]
スライドをMarkdownで管理してみたいそこのあなた！
是非お試しを！

[^1]: https://marp.app/

![bg vertical right 80%](../img/slide_repo.png)
![bg right 80%](../img/slide_actions.png)

参考: [Marp入門〜応用｜markdownでプレゼン資料を楽に素早く作って発表しよう](https://zenn.dev/cota_hu/books/marp-beginner-advanced)