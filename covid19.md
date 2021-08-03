---
layout: page
title: COVID-19
permalink: /COVID19/
---

# **対数坂の上で玉を支え続けるのか？**

感染者数の推移を可視化 

Visualization to feel the impact of measures on COVID-19.

このページの図や動画，Mathematicaのファイルは自由に使ってください．何か内容に間違いがあればメールや[Twitter](https://twitter.com/ryseto)で教えてください．



傾斜角一定の坂に感染者数（または死者数）を表す数字が対数スケールで刻まれている．


- **なぜ対数スケールか？** \\
・活動度や接触頻度が変わらない状況では感染力の強い感染症の感染者数は**指数関数**的に増加する．つまり，ある時間間隔で2, 4, 8, 16 と倍々で増えていく．目盛が対数スケールなら，指数関数的増加は一定速度で坂を下っていく動き．\\
・強さが一定の対策で感染者数が減る場合も，ある時間間隔で 128, 64, 32 と減っていく．この指数関数的減少も一定速度で坂を上っていく動きで表現できる．\\
・10から100まで，また100から1000の位置まで移動する時間は等しい．
対数スケールでは1, 10, 100, 1000 や 2, 4, 8, 16 が等間隔．\\
・感染が拡大している時も，対策を強化して減らしていく時も，
ある数字に到達するのにかかる時間を距離で表現できる．\\
・撲滅を目指して感染者数を減らす時，1000から100までは900人も感染者が減るけど，
100から10までは90人．10から1までは9人．**減れば減るほど効率が悪くなっていくように感じる**．


- **なぜ傾斜角が一定か？**\\
・感染は**1人の感染者が平均で何人他の人を感染させるか**で推移していく．現在の感染者数には依存しない．\\
・東京の中でたった1人しか感染者がいなくても，その人が2人に感染させれば**実効再生産数**は2．2から4へ，4から8へと指数関数的に増加する．\\
・どこのだれが感染者か分からない．感染を防ぐには**感染者がいるかもしれない範囲の全員**の接触削減が必要になる．\\
・だから，一人の感染者が何人に感染させるかを制御する対策を比喩的に「力」と考えると，
その力は**感染者数に依存しない**．どこでも力は一定だから坂の角度は一定．\\
・感染者が本当に1人もいない場合だけ例外．接触削減をしなくても感染は広がらない．

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

- [感染者数と死者数 newcases_and_newdeaths.nb](/assets/misc/newcases_and_newdeaths.nb)

