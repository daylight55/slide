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

---

# DevOpsとは
![bg right vertical 100% ](../img/devops/devops.png)


- 「顧客に価値を素早く届けるため、開発・運用が協力する、文化的な姿勢・取り組み」のこと [^1]
- 企業によって全面に出す定義が異なるため

[^1]: https://www.members-devopslead.com/service

---

# DevOpsの実践度

![bg right 70% 国内企業におけるDevOpsの実践状況の推移](../img/devops/devops_graph.png)

-  IDC Japanの調査によると、DevOpsの実践率は年々伸びている。 [^1]
- 2022年の調査では **59.3%** の実践率
- しかし、結論として「**ビジネス上の効果が得られている企業は増えていない**」とある。

[^1]: https://www.idc.com/getdoc.jsp?containerId=prJPJ49999523

---

<!--
_class: lead
-->
# DevOpsの**実践**は難しい

---

# 例:DevOps に求められる技術
![bg right 40%](../img/devops/devops_roadmap.png)

学習ロードマップとして

Programming Language, OS, VCS, Containers, Cloud Providers, Network, Serverless, IaC, CI/CD Tool, GitOps, ServiceMesh etc...

などが挙げられている。[^1]

[^1]: https://roadmap.sh/devops

---

# つまり、DevOpsを現場に落とし込むと、、、

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

- 「DevOpsチームを新しく作ったから、DevからOpsに渡るまでのセットアップはよろしく！」
- マイクロサービスごとにセットアップを任せられるチームができる。

![bg vertical right 120%](../img/devops/devops_antipattern_1.png)

---
<!--
_class: lead
-->
# DevOpsチーム「数が膨大すぎる・・・」

![bg vertical right 50% ](../img/devops/sick_noiroze_man.png)
![bg 50% ](../img/devops/sick_noiroze_woman.png)

---

<!--
_class: lead
-->
# デプロイ・運用までの<br>抽象化が必要

---

<!--
_class: lead
-->
# **Platform Enginieering**の需要

---

## Platform Enginieeringとは

![bg right 100%](../img/devops/platform_engineering_gartner.png)

- Garthnerの「先進テクノロジのハイプ・サイクル：2022年」で登場 [^1]
- 開発者体験と生産性を向上させるためにセルフサービスで利用できるツールチェーンとワークフローを設計・構築する分野 [^2]

[^1]: https://www.gartner.co.jp/ja/newsroom/press-releases/pr-20220816
[^2]: https://speakerdeck.com/jacopen/platform-engineeringhenozhao-dai

---

# どう変わるのか
s

![10%](../img/devops/platform_into_organization.drawio.svg)

---


<!--
_class: lead
-->
これは避けられない気もします😭

---

# Howにこだわると危険

---

<!--
_class: lead
-->

# 組織文化

- 

---

## まとめ

- DevOpsの

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