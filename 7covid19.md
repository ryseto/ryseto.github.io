---
layout: page
title: COVID-19
permalink: /COVID19/
---

### **感染者数の推移を動きで表現**

Visualization to feel the impact of measures on COVID-19.

このページの図や動画，Mathematicaのファイルは自由に使ってください．問題を考えるとっかかりになると信じてこれを書いていますが，間違いや誤解を生む可能性がある等の指摘があれば連絡ください．

**東京の新規感染者数** ([tokyo_COVID19.nb (Mathematica)](/assets/misc/tokyo_COVID19.nb))

<center>
<video muted autoplay controls>
    <source src="/assets/movie/Tokyo_new_cases.mp4" type="video/mp4">
</video>
</center>


傾斜角一定の坂に感染者数（または死者数）を表す数字が対数スケールで刻まれている．

- **ワクチン効果の追記(2021-10-08)**\\
感染の広がりやすさを表す基本再生産数を感染症の性質で変わらないとして時間変動しない傾斜角にしていた。しかしワクチン接種が進みその感染防止効果が現れてきたので、それを表現するために傾斜角を変動させている。上のアニメーションでは日本全体のワクチン接種（２回完了）率を使っていて、基本再生算数を8、ワクチンを接種した人は感染しないと仮定しているので実際とは違う。ワクチンの効果をイメージするためのもの。集団免疫が成立するというのは、０に向かう坂道が上り坂から下り坂に切り替わる事。それができるかどうかは基本再生算数とワクチンの感染防止率に依存する。


- **なぜ対数スケールか？** \\
・活動度や接触頻度が変わらない状況では感染力の強い感染症の感染者数は**指数関数**的に増加する．つまり，ある時間間隔で2, 4, 8, 16 と倍々で増えていく．目盛が対数スケールなら，指数関数的増加は一定速度で坂を下っていく動き．\\
・強さが一定の対策で感染者数が減る場合も，ある時間間隔で 128, 64, 32 と減っていく．この指数関数的減少も一定速度で坂を上っていく動きで表現できる．\\
・10から100まで，また100から1000の位置まで移動する時間は等しい．対数スケールでは1, 10, 100, 1000 や 2, 4, 8, 16 が等間隔．だから，感染が拡大している時も，対策を強化して減らしていく時も，ある数字に到達するのにかかる時間を距離から認識できる．\\
・撲滅を目指して感染者数を減らす時，100から10まで減るのにかかる時間は1000から100までと同じ．減れば減るほど効率が悪くなっていくように感じるが，対数スケールでみれば順当は減り方と分かる．\\
・つまり，**何人増えたとか減った**でなく，**何割増えたとか減った**が目安．対数スケールなら数字がなんであれその点とその半分の数に対応する点の距離が同じ．\\
・対策の強さで動く速度が変わる．対策の強度が変われば動き方が変化する．対策と感染者数の変化を感覚的に捉えることができる．

- **なぜ傾斜角が一定か？**\\
・感染は**1人の感染者が平均何人感染させるか**で推移していく．\\
・東京の中でたった1人しか感染者がいなくても，その人が2人に感染させれば**実効再生産数**は2．2から4へ，4から8へと指数関数的に増加する．\\
・どこのだれが感染者か分からない．感染を防ぐには**感染者がいるかもしれない範囲の全員**の接触削減が必要になる．\\
・だから，一人の感染者が何人に感染させるかを制御する対策を比喩的に「力」と考えると，
その力は**感染者数に依存しない**．どこでも力は一定だから坂の角度は一定．\\
・感染者が本当に1人もいない場合だけ例外．接触削減をしなくても感染は広がらない．

- **注意点**\\
**「坂を重い岩が勢いを増しながら転がり落ちる」というアナロジーはここでは成り立たない**．支える力が弱くて落ちる時も，その力が一定なら落ちる速さも一定．それが指数関数的増加．指数関数的増加は数が大きくなるほど圧倒的な増え方になるけど，感染力を上回る十分な対策をすればすぐに止められる．国の対策や個人の心掛けで接触頻度を減らせば，その瞬間から多くの新たな感染を未然に阻止できる．その結果が数字として見えるようになるまでの遅れはあるけど，**現象そのものは力を変えた瞬間から変わる**．

- **コメント**\\
**「予想が外れた」**とか**「感染急拡大(“オーバーシュート”)が起こらなかった」**といった観点から，研究者の予想を疑うきらいがある．これまでの感染状況の推移は，ここの動画が示すように警戒感の高まりや緊急事態宣言で感染者数を抑えたと思ったら，その後力を緩めて感染拡大を許すということを繰り返している．感染は個々の行動や全体の対策に依存するので，台風の進路のような予測はできない．でも，**この坂の上にいることだけは確か**．力を抜けば下に落ちていく．警戒感が高まれば踏みとどまり感染の拡大は遅くなるけど，時間とともに疲弊するので支えるのがどんどん難しくなっていく．

- **３つの考え方**\\
(1) 上まで登り切ることでこの坂から抜け出すこと．これがゼロコロナ．国内で根絶し，水際対策で外から入ってこないようにする．入ってきた場合も短期的・局所的な強い対策でゼロに戻す．\\
(2) ワクチンの集団免疫が成立するというのは，再生産数が３の場合，本来感染させる３人のうち，ワクチンによる感染防止の効果で2人以上が感染しない状況．ワクチン接種が進むほど坂の角度が緩やかになり，最終的には下り坂で感染者０のところまでいける．多くの人がワクチンにこれを期待していたと思うけど，残念ながらワクチンの感染防止効果は十分でないらしい．\\
(3) 大半の人が感染してしまえば，感染させる相手がいなくなるので感染の拡大は止まる．これも集団免疫なので1人が感染させるはずだった人数のうち，そのほとんどが既に感染済みなら感染は止まる．**ワクチンで重症化を防げるなら**，このシナリオが現実的な選択肢という考え方もある．しかし，感染する絶対数が多いので犠牲は少なくない．


### その他

- [note の解説 (explanation in Japanese)](https://note.com/ryseto/n/n432fcc37c992)

- [ワクチンによる集団免疫の考え方](/assets/pdf/role_of_vaccine.pdf)

- [死者数と感染者数の相関](/_posts/2021-08-30-covid19-world.md)

- [日本の新規感染者数(2022-1-4)](/assets/movie/Japan_new_cases.mp4)

- [東京の新規感染者数(2022-1-4)](/assets/movie/Tokyo_new_cases_simple.mp4)

- [100万人あたりの死者数（世界）](/assets/movie/world_death_per_M.mp4) \\
 ([covid19-slope_deaths.nb (Mathematica)](/assets/misc/covid19-slope_deaths.nb))

- [100万人あたりの死者数（アジア）](/assets/movie/asia_death_per_M.mp4)

- [長期ビジョンと短期ビジョンの緊急事態宣言（イメージ）](/assets/img/zerocovid3.jpg) [2021-4-6]

- [３回の緊急事態宣言の比較(東京) Comparison between two states of emergency in Tokyo's positive case number.](/assets/movie/tokyo.gif)

- [感染者数と死者数 newcases_and_newdeaths.nb](/assets/misc/newcases_and_newdeaths.nb)
