---
layout: page
title: COVID-19
permalink: /COVID19/
---


感染者数の推移を可視化 

Visualization to feel the impact of measures on COVID-19.

**このページの図や動画，Mathematicaのファイルは自由に使ってください．何か内容に間違いがあればメールやツイッターで教えてください．**

# **対数坂の玉**

- **傾斜角一定**の坂に感染者数（または死者数）を表す数字が**対数スケール**で刻まれている．


- **なぜ対数スケールか？** \\
人流や接触頻度が変わらず同じペースで感染者が増えていく状況を**指数関数**的な増加という．\\
つまり，ある時間間隔で2, 4, 8, 16 と倍々で増えていく．\\
感染者数を表す目盛が対数スケールなら，この指数関数的増加を一定速度で下っていく動きで表現できる．\\
強さが一定の対策で感染者数が減る場合も 128, 64, 32 という減り方．
この指数関数的減少は一定速度で上っていく動きで表現できる．\\
10から100の位置まで移動する時間と100から1000の位置まで移動する時間は等しい．
対数スケールではそれらの距離が等しい．\\
感染が拡大している時も，対策を強化して減らしていく時も，
その数字に到達するのにあとどのくらいの日数が必要かという目安を距離で表現できるのが対数スケール．\\
撲滅を目指すなら一番上までいく必要があるが，数字が小さくなるほど目盛の間隔が大きくなる．


- **なぜ傾斜角が一定か？**\\
感染は**1人の感染者が平均で何人他の人を感染させるか**で推移していく．現在の感染者数には依存しない．\\
東京の中でたった1人の感染者が2人に移しても**実効再生産数**は2．その状況がしばらく続くと感染者で溢れかえる．\\
一人の感染者が何人に感染させるかを制御する対策を比喩的に「力」と考えると，
その力は**感染者数に依存しない**．どの「位置」でも力は一定だから坂の角度は一定．

- [ワクチンの期待と現実](/assets/pdf/role_of_vaccine.pdf)



### 可視化

- 東京の感染者数 Tokyo's new cases ([tokyo_COVID19.nb (Mathematica)](/assets/misc/tokyo_COVID19.nb))

<center>
<video muted autoplay controls>
    <source src="/assets/movie/Tokyo_new_cases.mp4" type="video/mp4">
</video>
</center>

- [100万人あたりの死者数（世界）](/assets/movie/world_death_per_M.mp4) \\
 ([covid19-slope_deaths.nb (Mathematica)](/assets/misc/covid19-slope_deaths.nb))

- [100万人あたりの死者数（アジア）](/assets/movie/asia_death_per_M.mp4)

- [note の解説 (explanation in Japanese)](https://note.com/ryseto/n/n432fcc37c992)


- [長期ビジョンと短期ビジョンの緊急事態宣言（イメージ）](/assets/img/zerocovid3.jpg) [2021-4-6]

- [３回の緊急事態宣言の比較(東京) Comparison between two states of emergency in Tokyo's positive case number.](/assets/movie/tokyo.gif)



