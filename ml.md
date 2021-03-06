# はじめに 

## 参考図書
仕事ではじめる機械学習、  
https://www.oreilly.co.jp/books/9784873118215/  
ゼロから作るDeep Learning  
https://www.oreilly.co.jp/books/9784873117584/  

## 用語集
https://qiita.com/Ted-HM/items/298116d03cbb9b3477e6#_reference-3681771679c368269ebb


# 機械学習の使用場面  

通常、何らかの問題を解決しようとする場合 ***――特に何らかのパターンを見つける必要がある場合――*** 、  
人があれやこれやと考えて答えを出すことが一般的。  
「この問題はどうやらこういう規則性があるのではないか」、  
「いやいや、別の場所に原因があるかもしれない」  
といったように、人の経験や直感を手がかりに試行錯誤を重ねて仕事を進めます。  
一方、機械学習による手法では、人の介入を極力避け、集められたデータから答え（パターン）を見つけようと試みます。


***機械学習で解ける範囲と解けない範囲を線引きする***

人間は、例えば徹夜で連続して単純作業をしていると、その判断基準がぶれてくることが往々にしてあります。  
それに対し、機械学習の予測基準は学習フェーズからブレることはないので、大量のデータに対しても人より安定した予測を行えるのです。

そもそも解こうと思っている課題が人間にも解けない問題の場合は機械学習で解くのも難しいでしょう。  
機械学習、特に「教師あり学習」では、何が「正解」なのかを人間が機械に教えなければなりません。  
つまり、人が「正解」を決められない問題は機械にも解くことができないのです。  

* 大量のデータに対して、高速に安定して判断を求める必要がある
* 予測結果には、一定数の間違いが含まれることが許容できる

業務課題からビジネスの意思決定までのセットのプロジェクトを考えることが重要。  
業務課題の発見と意思決定、アクションは人だけができる重要な仕事。  






## シバタアキラさんの記事
https://blog.datarobot.jp/2017/08/31/how-to-make-machine-learning-pj-successful/
https://ashibata.com/2017/10/30/aifail/


## マネジメント層の理解不足
https://www.m2ri.jp/news/detail.html?id=238


経営層としては、機械学習で何ができるかを理解して  
モデルを作るまでは簡単にできる。   
それをどのように使うかが大事。モデルを作ってどう使うかが大事。  
機械学習をプロジェクトに当てはめることが大事。 　

トップがAIを使いたいけど、現場が出さないみたいなケースもある。 　　
現場がやりたいときにモデルを探すんだけど、AIは魔法の箱だからなんでもやってみたいなケースでは難しい。   
基本的な最低限の知識が必要かも。（トレーニング用とモデリング用で分けるとか）  

経営で回す時に理解するための難所   
わかるとできるが違う、何ができるかがわかるということが大事。そのためには、どのような処方箋が必要？  
どうやって使うとどうできているは違う。PCを使うと半導体がわかっているとの違い。   
モデルのインサイトを理解する。モデルが問題解決に使えるかどうかを理解することが大事。  
どういうデータを持ってきたらいいかとか、技術的なことは別にして、インサイトに繋げること。  
実際にモデルを作って、予測を実行してみることが大事。アルゴリズムがフワッとわかっていれば良い。ハンズオンセミナーとかで実際にいじってみるのも大事。   



「日本企業は新しいITが登場したとき、それが必ず効果をもたらすと確認できて初めて、自社に取り入れるという傾向が強い印象です。他社の成功事例を収集し、その事例を自社に当てはめた場合の効果を測定してから、ようやく着手するのです。つまり事例がトリガーになっており、私のところにも『できれば同業他社の成功事例が知りたい』という問い合わせが多数寄せられています」

## IA
https://japan.zdnet.com/article/35106670/3/
「最近、AIブームだが、コンサルティング業界では、“知能増幅（IA：Intelligence Amplification）”が注目されている。これまでは、顧客に価値ある提言をするために、時間と工数をかけて分析を行い、結果を出していた。DataRobotは、とりあえずの分析を繰り返すことで知識を増幅できる。機械が完全に意思決定してくれる時代がくるかもしれないが、それまではAIよりもIAが重要になる」


# 機械学習のマイナス面

* 「正解の判断が難しい。」
* 機械学習に100％正解を出力するアルゴリズムは存在しない機械学習、特にDeepLearningは、モデルを元に大量のデータを使ってパラメータを自動調整する。
* 「入力データの傾向が変化する」

昔の文章ではネガティブな意味合いしかなかったのに対し、比較的新しい文章ではポジティブな意味もありうる《JK語とかありそう》

* セキュリティ（一定の誤検知が許される）
トレーニングセット・ポイズニング
アドバーサリアルエグザンプル
誤検知の誘導、

### ニューラルネットワークやディープラーニングの特性

ニューラルネットワークやディープラーニングは、従来の機械学習で使われた手法以上に、人の介入を遠ざけることができるという重要な性質を持ちます。

ディープラーニングは、「end-to-end machine learning」と呼ばれることがあります。  
ここで言うend-to-end とは、「端から端まで」という意味であり、これは生データ（入力）から目的の結果（出力）を得ることを意味します。

人  
↓  
機械学習  
↓  
ディープラーニング  

### 今の流れ。　数年で精度は更にあがると思う
（大きな学習工数をかけず）に、既存のモデルで70-80%の精度でデータ予測することができる。  　　
　数年で、この予測精度が90%近くになれば、大事なプロセスはアルゴリズムの選択部分は簡素化し、問題の定式化、データ収集、MVPによる結果の検証になる。
 
# 問題を定式化する

どのように問題を解くのか定式化する。何を目的にするのか、そして解きたい課題について仮説を立て、何をすればよいのかを明確にすることです。

システムを作る（施策）時には、ビジネス上の目的があるはず。

***プロジェクトの目的と解き方をセットで考える***

***AIで何をするかが明確でないと失敗する***

資生堂
　顧客の顔の特徴点を取る。メークアップのパーソナライズ化
　http://itpro.nikkeibp.co.jp/atcl/column/14/346926/111701210/?rt=nocnt



ここまで私が学びながらも勉強してきた、AI(人工知能)ですが、やはりビジネスに導入するためには「基本確認」が大事！！
どのような課題があるのか、その課題をAI(人工知能)が解消すれば、売り上げが伸びるのか、それともコストが削減できるのか…などなど
「AI(人工知能)を導入する必要性」を明確にする必要があります。

### IBMの導入フロー
https://www.ibm.com/developerworks/jp/linux/library/l-machine-learning-deep-learning-trs/index.html



### 目的
「生産コストを減らす」 

### 目的をブレークダウンする。
「歩留まり改善」→　
「どこで不良が起こっているかを特定する、そのために機械学習の力を使う」

## 仮説検証とは 
「仮説を立て、それを証明するためのデータを集め、真偽を確かめること」

1. 仮説を立てる
知りたいことを言い切る形にすれば仮説になります

「クックパッドの利用者が有料会員になるきっかけは文字ではなく美味しそうな料理の写真である」

2. 施策/KPIを考える
仮説は根拠の程度はあれど真偽は不明です。その真偽を確かめるために何のデータを集める必要があるか考えます。***ここが一番の難所です。***  


KPIの設計時にはできるだけ少ない指標にする方が良いのですが、機械学習に使える情報は出来る
限り多い方が望ましいのです。後から必要に応じて特徴選択のロジックを加えたり次元圧縮をしたりす
ることは可能ですが、保存していない情報を増やすのは困難です。例えばあるユーザーが広告をクリッ
クするかを予測する際に、性別や午前中／夕方に訪問した、掲出する広告のカテゴリなど、予測に関
する情報の多様性を確保する必要があります。



3. 仮説検証後のアクションを決める
実際にデータを集める「前」に、データを集めた後のアクションを決めます。このステップにより先の「施策/KPI」が必要十分か判断できます。

サービスの改善のように、指標となるKPIの意味に主観が含まれる場合はとくに意識します。事後の解釈ではサンクコストによるバイアスがかかり、冷静な判断が難しくなります。

4. 対象を決める

「2. 施策/KPIを考える」と、この「4.対象を決める」では、相関関係と因果関係の問題に十分注意

最終的なサービスへの全体影響を知りたい場合は細かいことを考えず全体を分割してABテストなどでデータを集めます。

一方で、何かしらの価値の有無を確認したい場合、まずは「このユーザの行動が変わらないのであれば、価値自体が無いのだろう」と考える理想的なユーザを施策の対象とすることをおすすめします。

5. サンプルサイズを決める

データには　***「明示的データ」***　と　***「暗黙的データ」***　がある。

* 「明示的データ」
ユーザーに直接好き嫌いや関心のあるなしを質問して回答してもらう

* 「暗黙的データ」
利用者が商品を購入したり閲覧したりといったアイテムは関心があるとみなすデータ

データ量は明示的データよりも暗黙的データの方が圧倒的に多くなる。


実際にシステムとして使う場合は、評価値がないため苦労することが多いでしょう。評価値を取得するためのインタラクションはシステムとしてユーザーメリットがある形で組み込まなければデータとして集まりません。また、予測対象とするデータはユーザーの嗜好が現れるデータを適切に利用するよ
うに心がけましょう。特に、その対象が最終的に予測したい値なのか、それとも特徴量として使える途中のデータなのかを切り分けることが重要です。



6. A/Bテスト、仮説検定を実行


## 機械学習とディープラーニング
通常の機械学習は、特徴量が肝となる。
そのばあい、特徴量を決めるのはビジネスドメインの知識がある人の経験など、人が介入する。
一方、ディープラーニングは大量のデータを処理することで機会が特徴量を発見する。

ニューラルネットワークの特徴は、データから学習できる点にあります。データから学習するとは、重みパラメータの値をデータから自動で決定できるということです。


***ビジネスの多くでは、教師あり学習を使い何かしらを分類することが多い***

***教師あり学習では、質の良い正解ラベルをどのように取得するかが重要***

機械学習はデータが命です。データから答えを探し、データからパターンを見つけ、データからストーリーを語る――これが機械学習で行うことであり、データがなければ何も始まりません。そのため、機械学習の中心には「データ」が存在します。このデータ駆動によるアプローチは、「人」を中心とするアプローチからの脱却とも言えます。（by　0からはじめるDeepLearning）


***試行錯誤を効率よく行うことが重要***

分類のモデルを作ったけれどランダム出力のほうが良い性能となることも頻繁に起こります。機械学習を含めたシステムの開発は、通常のWebシステムの開発で期待されるような1,2週間という短いサイクルでイテレーションを回すのは難しく、数ヶ月かかることも珍しくありません。

http://www.sascom.jp/blog/2017/10/27/artificial-intelligence-separating-reality-hype/


## アルゴリズムを選択する
http://www.sascom.jp/blog/2017/11/21/machine-learning-algorithm-use/




## Deep Learningでは、
プラットフォームの選択が大事?  Azure/AWS  


## 開発環境例
https://employment.en-japan.com/engineerhub/entry/2017/04/28/110000

## Deep Learningの種類

http://gagbot.net/machine-learning/ml4

### CNN
https://deepage.net/deep_learning/2016/11/07/convolutional_neural_network.html


### RNN

* LSTMネットワーク  
https://qiita.com/KojiOhki/items/89cd7b69a8a6239d67ca  
データの正規化など  
http://techlife.cookpad.com/entry/2017/10/30/080102



### GNN



#  学習のためのデータを収集(難所)

ビジネスにおける知見を得るためには教師なし学習を用いますが、分類や回帰などの教師あり学習や推薦システムなどの性能を上げるためには、ラベル付きのデータやコーパス、辞書などより多くの良質なリソースが必要

* サービスの中にログ取得の仕組みを用意してそこから抽出する（完全に自動）  
* コンテンツなどを人が見て付与する（人力で行う）  
* 機械的に情報を付与して、人手で確認する（自動＋人力）

本章では、教師データを作るのは誰かという観点から説明を進めていきます。
1. 公開されたデータセットやモデルを活用する
2. 開発者自身が教師データを作る
3. 同僚や友人などにデータ入力してもらう
4. クラウドソーシングを活用する
5. サービスに組み込み、ユーザに入力してもらう

はじめに、解きたい問題から分類をするべきなのか、回帰をするべきなのかを考える。



## ディープラーニングでは
学習率のようなパラメータはハイパーパラメータと言います。これは、ニューラルネットワークのパラメータ――重みやバイアス――とは性質の異なるパラ
メータです。なぜなら、ニューラルネットワークの重みパラメータは訓練データと学習アルゴリズムによって“自動”で獲得されるパラメータであるのに対して、学習率のようなハイパーパラメータは人の手によって設定されるパラメータだからです。一般的には、このハイパーパラメータをいろいろな値で試しながら、うまく学習できるケースを探すという作業が必要になります。

* 多段モデル(binary classification)
　識別機を多段階に入れる。　正確性を出せる。
　人の手がかかる。
* 


# 事例

https://employment.en-japan.com/engineerhub/entry/2017/11/30/110000  
  
https://www.nri.com/~/media/PDF/jp/opinion/teiki/chitekishisan/cs201611/cs20161103.pdf
  
## Cookpad

機械学習
* 着実な方法で実装する（実績のあるモデルを使う、地道にデータを用意する）  
* 手軽な方法で改善する（素性でなく、訓練データを修正する）  
* 最後は機械学習に拘らない（ルールで直す、手で直す）

2015年の記事はもう古い？

http://techlife.cookpad.com/entry/2015/09/30/170015
http://techlife.cookpad.com/entry/2017/09/14/161756
http://techlife.cookpad.com/entry/2017/11/28/151855

## Gree
http://labs.gree.jp/blog/2017/10/16600/

http://labs.gree.jp/blog/2017/03/16347/


## スーパーソフトウエア
http://tokyo.supersoftware.co.jp/press/7927

### 介護×AI
http://blog.idcf.jp/entry/iot-operation-analysis


### ビデオからの人間の行動認識
https://www.twentybn.com/

### AIの見える化プラットフォーム
http://useaible.com/useaible-machine-learning-with-no-blackbox/

### 車のモデルベース開発におけるモデル生成
https://www.ipa.go.jp/files/000057837.pdf  

機械学習を活用してプラントモデルを作成する手法は利点も多く、しっかり特徴を理解して活用することでプラントモデルの精度を上げることができる。  
しかし、機械学習を活用して作成したプラントモデルの信頼性については現在のところ証明することが難しいという課題もある。  
関係する教師データの品質と網羅性が、できあがったプラントモデルの精度に影響することがわかった。  

