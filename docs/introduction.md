# プログラミングを始めよう

本セクションでは、

- そもそもプログラミングとは
- 何が必要なのか
- どんなメリットがあるのか

などを説明したうえで、まずは参加者の皆さんにとってのプログラミングへのハードルをできるだけ下げていきます。

よく「テスターはコードが書けない、読めない」と言われたりしますが、講師が過去社内教育をやってきた経験上**テストエンジニアはプログラミングが出来るようになる**と断言できます。

## プログラミングとは

”プログラミング”をWikipediaで調べると、以下の説明がされています。

> コンピュータープログラミング（英語: Computer Programming）とは、ある特定のコンピューティングの結果を得ることを目的として、実行可能なコンピュータープログラムを設計・構築するプロセスのことである。プログラミングが関係するタスクの例としては、アルゴリズムの生成、アルゴリズムの正確さとリソースの消費量のプロファイリング、選択したプログラミング言語でのアルゴリズムの実装（これは一般にコーディングと呼ばれる）などがある[1][2]。プログラムのソースコードは、コンピューターのCPUで直接実行される機械語ではなく、プログラマーが理解できる1つ以上のプログラミング言語で書かれる。プログラミングの目的は、あるタスク（オペレーティングシステムのように複雑な場合もある）をコンピューター上で自動化する1連の命令を見つけることで、与えられた問題を解決することである。そのため、プログラミングのプロセスには、アプリケーションドメインに関する知識、特定のアルゴリズム、形式論理など、さまざまな主題に関する専門性が要求されることが多い。 - [プログラミング - Wikipedia](https://ja.wikipedia.org/wiki/%E3%83%97%E3%83%AD%E3%82%B0%E3%83%A9%E3%83%9F%E3%83%B3%E3%82%B0)

**読み飛ばしましたね？**

はい、この説明はとても難しいので、読み飛ばしても仕方がありません。

おおざっぱには、プログラミングとは「コンピューターに命令すること」と言えます。皆さんがご存知の通り、人間と違ってコンピューターは以下の特徴があります。

- 自分で考えて動くことはできない
- 決められたことを速く・たくさんやるのが得意

そのため、人間がコンピューターになにか（よく「処理」と表現されます）をさせたいと思ったら、コンピューターが理解できる形と粒度で命令をする必要があります。

コンピュータが理解できる形で命令をすることが、すなわち「プログラミング」です。

それでもまだ難しい、と感じる方も多いかもしれません。しかし、テストエンジニアをしている人はプログラミングに近いことを普段から行っています。

### テストエンジニアの業務に置き換えて考えてみると・・・

テスト設計（テスト詳細設計、テストケース作成・・・用語はおまかせします）をするシチュエーションを想像してみてください。

あなたはテスト設計者です。チームにはあなたが作成したテスト手順書を見ながらテスト実行を行うメンバーがいます。しかし、そのメンバーはチームに入ったばかりで、テスト対象の操作方法や仕組みなどを全く知りません。

こんなとき、たとえばテスト手順書に

> 手順：Adminユーザーでログインしてユーザー退会処理を行う。<br>
> 期待結果：対象ユーザーがDB上で論理削除されていること。

のような記載をするでしょうか。おそらくしないと思います。（ですよね？）

きっと後輩思いのみなさんであれば、

> 手順：<br>
> １．トップ画面のメニューバー右上にある「ログイン」を押下<br>
> ２．ログイン画面で、Adminユーザー（ユーザ一覧シート参照）のアカウントでログインする<br>
> ３．左のメニューから「退会処理」を選択<br>
> （略）<br>
> 期待結果：<br>
> 以下のクエリを実行して、deletedカラムがTrueになっていること<br>
> SELECT * FROM 略

くらいの書き方をするのではないでしょうか。

テスト対象に馴染みがない人に向けて、操作手順や期待結果の確認手順を詳細に指示するはずです。

これはプログラミングにおいて、コンピューターに対して詳細な手順を書き下して指示することと、実はほとんど一緒です。人間の言葉で書くか、プログラミング言語で書くか、の違いだけ、です。

プログラミングは一見難しそうですが、

1. やりたいことを実現するための手順を考える
2. それを（プログラミング言語で）書く

というシンプルなこと（かつ、テストエンジニアが実は業務のなかでやっているようなこと）をしているに過ぎません。


## 必要なもの

- 環境構築
- 言語

## プログラミングが出来るメリット

- 開発者とのコミュニケーションを活性化し、テストエンジニアとしての仕事に活かす
- 自分の業務を効率化し、テストエンジニアとしての仕事に活かす


## 学習を難しくしている要素

### 実務とのつながりを感じづらい

プログラミングを学ぼう！と思ったとき最初に行うのは、なにか学習のための教材を入手することです。

!> プログラミングを習いにいく、という選択肢もありますが、費用や時間の点で今回は対象外とします。

昨今は学習のための教材も多くなっており、例えば以下が挙げられます。

- 書籍
- YouTubeの動画や、Udemyなど有料講座の動画
- ProgateやPaizaラーニングなどオンライン学習サイト

これらの教材は、プログラミングを学ぶ上で確かに有用です。

しかし、よくある学習の流れはというと・・・

1. 言語の特徴
2. 変数・定数などの言葉と書き方の説明
3. if, for, whileなどの書き方の説明
4. 関数、クラスとオブジェクト、などなど・・・
5. （以下略）

このような順番が多いです。

これらの合間に

``` python
# 1+2の計算をするプログラム
>>>1 + 2
3
```

や

``` python
# コマンドプロンプトに「Hello!World」と表示するプログラム
>>> print("Hello!World.")
Hello!World.
```

などのプログラムを書いて動かすことになります。

これ自体は確かに基本的な練習ですし、これで「おお、動いた！プログラミングの第一歩が踏み出せた！」と思える方は素晴らしい素質の持ち主です。が、当てはまる方はかなり少ないのではないでしょうか。

画面に「Hello!World」という文字を出力するだけではプログラミングの面白さを感じづらく、かつ日々の仕事でプログラミングを活用することとのギャップが大きすぎる点が、プログラミング学習を難しくしている要因のひとつです。

今回のワークショップでは（時間が限られていることもあり）一般的な書籍などのように一歩一歩積み重ねる形での説明はせず、まず動作するプログラムをお配りして、その動作を理解しながら少しずつ手を加えることで、「理屈よりも仕事に使えそう感を得る」ことを優先していきます。

!> モチベーションを保ちながら学習を進めていただくためのやり方なので、決して基礎知識が不要であるというわけではありません。本ワークでプログラミングに触れたのち、書籍などで基礎部分も理解していただくことを推奨します。


### プログラミングや、プログラミングができる人への誤解

プログラミングの経験がない方が、よく誤解している、ハードルを上げてしまっている点があります。

#### 「プログラミングはたくさんのことを暗記しなければならない」という誤解

プログラミングが出来る人はキーボードをすごいスピードで打っていて、Googleでいちいち調べたりしない。というイメージを持っている方がいますが、そんなことはありません。プログラミングが出来る人はなんでもかんでも暗記をしているわけではなく、都度Googleで検索しながら書いている部分も多くあります。

!>たまに「＊＊＊というプログラミング言語を**覚えたい**」という方がいますが、講師の主観では、プログラミング全般や言語毎の「考え方を理解する」必要はありますが、「書き方を覚える」ことは本質ではありません。特に「プログラミングもできるテストエンジニアになりたい」であれば、Googleなどの検索を頼ってでも、やりたいことが実現できればいいのです。実務にカンニングはありません。

大切なのは、書き方を覚えることよりも、プログラミングでは一般的にどんなことができるのか、の感覚を身につけることです。

「何ができるか」の発想を得ることができれば、「やり方」は調べることができます。

プログラミングが出来る人というのは、コンピューターにやってほしい（けれども大きくてそのままではコンピューターが理解できない）仕事を、小さなタスク＝手順に分解する能力を身に着けています。「このくらい小さければ、こんな言い方をすれば、コンピューターが理解できるはずだ」というのを思いつける力です。

そして、分解した小さなタスクをそれぞれ、プログラミング言語を使ってコンピューターに命令しています。

仕事で毎日同じプログラミング言語を使っていると、同じような命令を書く機会が増えます。同じような命令を何度も書いていると、だんだん検索しなくとも書けるようになります。この状態になると、一見たくさんのことを暗記しながら書いているように見えます。が、実際には短期的に記憶しているだけなので、時間が経ったり、他のプログラミング言語を使ったりすると、忘れてしまうこともしばしばです。書き方を忘れたとしても、考え方が見についているので、調べられるというわけです。

#### 「プログラミングができる人はエラーで悩まない」という誤解

エラーが出て動かない、は普通です。プログラミングに慣れた人でもそうなります。

プログラミングに慣れた人は、エラーをちゃんと読みます。ここが、初心者との一番の違いかもしれません。

確かに、プログラミング学習を始めてすぐに、見慣れない＆長いエラーが出ると、つい読み飛ばしたくなってしまいます。しかし、エラーの文面には問題がある箇所や解消方法の候補などが書かれている場合もあり、エラーをよく読むことがエラー解消への第一歩です。

「エラーは友達、怖くないよ」の精神で、まずはエラーの文面を読むようにしましょう。
