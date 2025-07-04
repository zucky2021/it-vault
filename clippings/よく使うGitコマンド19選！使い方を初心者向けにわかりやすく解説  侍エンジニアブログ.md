---
title: "よく使うGitコマンド19選！使い方を初心者向けにわかりやすく解説 | 侍エンジニアブログ"
source: "https://www.sejuku.net/blog/5816"
author:
  - "[[侍エンジニア編集部]]"
published: 2025-04-25
created: 2025-06-26
description: "この記事では「 よく使うGitコマンド19選！使い方を初心者向けにわかりやすく解説 」について、誰でも理解できるように解説します。この記事を読めば、あなたの悩みが解決するだけじゃなく、新たな気付きも発見できることでしょう。お悩みの方はぜひご一読ください。"
tags:
  - "clippings"
---
[![](https://www.sejuku.net/blog/wp-content/uploads/2024/09/627d7a6dc2c550d270a3ed63c7b492bb-1.png)](https://lp.sejuku.net/lp1_blog_02/?cid=freelance_fv_howto&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816)

この記事では、よく使うGitコマンドを一覧にまとめて紹介します。

**Gitコマンドってどうやって使うの？  
Gitコマンドの中でも良く使うものが知りたい**

Gitは今やエンジニアだけでなく、WebデザイナーやWebライターの方にも使われるツールとなりました。しかしGitを使いこなすためのコマンドについて、良く知らない方もまだまだ多いですよね。

そのような方のために、今回は **良く使うGitコマンドを19個ピックアップしてご紹介** します。この記事を読めば、仕事で急にGitを使うことになっても困らなくなりますよ。エンジニア未経験の方でも分かりやすい内容となっていますので、ぜひご一読ください。

この記事の要約

- **インストール後はユーザー名とメールアドレスの設定が必要**
- **Gitのコマンドはリポジトリ作成やコミット・ブランチ操作などに使える**

「独学と並行しながら、副業で稼げるようになれるかな…」

そんな不安を抱えている人は、ぜひ「 **[侍エンジニア](https://lp.sejuku.net/lp1_blog_02/?cid=lp_text_cta&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816)** 」をお試しください。

侍エンジニアでは現役エンジニアと学習コーチの **2名体制で** 学習をサポート。フリーランスエンジニアの支援を受けながら、実際の副業案件にも挑戦できます。

これまで **4万5,000名以上** の 受講生を指導してきた侍エンジニアなら、未経験からでも挫折なく副業での収入獲得に直結するスキルが身につけられますよ。

＼ 給付金で受講料が最大80%OFF ／

なお、休日やふと空いたすきま時間に収入が増やせるスキルを身につけたい人は、ぜひ **「 [侍エンジニア](https://lp.sejuku.net/lp1_blog_02/?cid=btn_article_lp) 」** をお試しください。

侍エンジニアでは現役エンジニアと学習コーチの2名体制で学習をサポート。月5~10万円の収入獲得を見据え、スキルの習得から仕事の取り方・進め方まで一貫して学べます。

受講料が **最大80%OFFになる「給付金コース」** も提供中。未経験から副業で収入を増やしたい人は、ぜひ一度お試しください。

＼ オンラインで相談可能 ／

目次
1. [Gitのインストールと初期設定](https://www.sejuku.net/blog/#index_id0)
2. [よく使うGitコマンド一覧](https://www.sejuku.net/blog/#index_id1)
3. [リポジトリ作成などに使うコマンド](https://www.sejuku.net/blog/#index_id2)
4. [コミットを操作するコマンド](https://www.sejuku.net/blog/#index_id3)
5. [作業ツリーを操作するコマンド](https://www.sejuku.net/blog/#index_id4)
6. [ブランチを操作するコマンド](https://www.sejuku.net/blog/#index_id5)
7. [まとめ](https://www.sejuku.net/blog/#index_id6)

## Gitのインストールと初期設定

画像：Gitの操作

そもそも [「Git」](https://git-scm.com/) とは、ソースコードなどのファイルに対する変更内容を管理するためのツールです。変更内容をチーム内で共有できたり、簡単に変更前のバージョンに戻せたりといったメリットがあり、多くの企業で使われています。

Gitのインストール方法は、使用しているOS（Windows／Linux／Mac）によって異なります。またインストール後の初期設定として、 **ユーザー名とメールアドレスの設定が必要** です。

各OSへのインストールや初期設定の方法については以下の記事で丁寧に解説しているので、参考にしてくださいね。

なお、プログラミングを学びたい気持ちはあるものの、どの言語が自分にあうのか、どう学習を進めればいいのかなどがあいまいな人は「 [プログラミング学習プラン診断](https://www.sejuku.net/blog/diagnose/?cid=btn_article_jobdiagnose&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816) 」をお試しください。

かかる時間は1分ほど。4つの質問に答えるだけで、あなたにあう言語や学習プランを診断してもらえます。

効率よくプログラミングを学習したい人は、ぜひ一度お試しください。

＼ 4つの質問に答えるだけ ／

## よく使うGitコマンド一覧

![よく使うGitコマンド](https://www.sejuku.net/blog/wp-content/uploads/2021/01/shutterstock_648958390-2.jpg)

よく使うGitコマンド

画像：よく使用するGitコマンドを覚えることで多くのメリットが得られる

Git使用経験の豊富なエンジニア目線で、よく使うGitコマンドを19個ピックアップしました。まずはコマンド名と用途を一覧表にしましたので、参考にしてください。

| コマンド名 | **用途** |
| --- | --- |
| [git init](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#a) | リポジトリを新規作成 |
| [git clone](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#b) | リポジトリをコピー |
| [git gc](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#c) | リポジトリを最適化 |
| [git pull](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#d) | リモートリポジトリの変更点をローカルリポジトリにマージ |
| [git push](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#e) | ローカルリポジトリの変更点をリモートリポジトリにマージ |
| [git add](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#f) | コミット対象のファイルを登録 |
| [git commit](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#g) | 変更されたファイルをコミット（ローカルリポジトリに変更内容を入れ込む） |
| [git reset](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#h) | 直前のコミットを取消 |
| [git revert](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#i) | 特定のコミットを取消 |
| [git tag](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#j) | コミットにタグを付ける |
| [git log](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#k) | コミット履歴を表示 |
| [git status](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#l) | 作業ツリー内の差分ファイルを表示 |
| [git diff](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#m) | ファイル内の差分箇所を表示 |
| [git mv](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#n) | ファイルを移動／ファイル名を変更 |
| [git stash](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#o) | 作業ツリーの状態を一時的に保存 |
| [git branch](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#p) | ブランチの作成／一覧表示 |
| [git checkout](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#q) | 処理対象ブランチの切り替え |
| [git merge](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#r) | 別のブランチから変更点をマージ |
| [git rebase](https://www.sejuku.net/blog/wp-admin/post.php?post=5816&action=edit&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816#s) | 派生元ブランチに変更点をマージ |

それぞれの詳細については、次章以降で解説していきますね。

なお、ITの仕事に興味はあるものの、どの職種が自分にあうのかわからない人もいますよね。そんな人は「 [ITキャリア診断](https://www.sejuku.net/blog/job-diagnose/?cid=btn_article_jobdiagnose&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816) 」をお試しください。

かかる時間はたったの1分。5つの質問に答えるだけで、自分にあうIT職種を診断してもらえます。

自身に適した職種が知りたい人は、手軽に試してみると良いですよ。

＼ 5つの質問に答えるだけ ／

## リポジトリ作成などに使うコマンド

![リポジトリ作成などに使うコマンド](https://www.sejuku.net/blog/wp-content/uploads/2021/01/image17.jpg)

リポジトリ作成などに使うコマンド

画像：リポジトリのイメージ

「リポジトリ」というのは、 **Gitにより管理するファイルの格納場所** です。サーバー上にありチームで共有するリモートリポジトリ（マスターリポジトリ）と、自分のパソコン上で管理するローカルリポジトリの2種類があります。

この章では、リポジトリの取り扱いに関するGitコマンドを5つご紹介します。

### git init　「リポジトリを新規作成」

Gitを利用するためには、リポジトリがないと始まりません。「git init」コマンドを使用すると、カレントディレクトリ(Gitが処理する対象フォルダ)にリポジトリを新規作成します。

作成したリポジトリには「.git」という名前のディレクトリが作成されます。Gitのプログラムはこのディレクトリを使用することで、リポジトリの変更履歴を管理するのです。

```
$ cd [リポジトリを作成するディレクトリ]
$ git init
```

git initコマンドについてもっと詳しく知りたい方には、以下の記事もおすすめです。

### git clone　「リポジトリをコピー」

「git clone」コマンドを実行すると、既存リポジトリを指定したディレクトリへコピーします。コピーするリポジトリは、リモートリポジトリ・ローカルリポジトリのどちらでも構いません。

```
$ git clone [コピーするリポジトリ] [コピー先ディレクトリ(省略可)]
```

なお、コピー先ディレクトリは省略可能です。省略した場合、カレントディレクトリに同名のリポジトリを作成します。

git cloneコマンドの情報がもっと欲しい方は、以下の記事も読んでみると良いでしょう。

### git gc　「リポジトリを最適化」

「git gc」コマンドを使用すると、すべてのリポジトリを最適化してくれます。具体的には **管理上不要なファイルを削除したり、ファイルサイズを圧縮したりといった処理内容** です。

```
$ git gc
```

実はリポジトリの最適化は、Gitのシステムが定期的に自動実行してくれます。そのため頻繁に実行する必要はありませんが、大量の変更内容を入れ込んだ場合などに手動で実行すると良いでしょう。

### git pull　「リモートリポジトリの変更点をローカルリポジトリにマージ」

「git pull」は、リモートリポジトリの変更内容を指定したローカルリポジトリにマージ（統合）するコマンドです。 **チーム開発で他の人がリモートリポジトリに入れた変更内容を、ローカルリポジトリに取り込むため** に使われます。

```
$ git pull [マージ元のリモートリポジトリ名] [マージ先のローカルリポジトリ名]
```

厳密には、マージ元もマージ先も省略可能。ただし省略するためにはリポジトリの関連付けなどの事前設定が必要なので、今回は割愛します。

git pullコマンドについてより理解を深めたい方には、以下の記事もおすすめです。

なお、IT企業への転職や副業での収入獲得を見据え、独学でプログラミングスキルを習得できるか不安な人は「 [侍エンジニア](https://lp.sejuku.net/lp1_blog_02/?cid=btn_article_lp&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816) 」をお試しください。

侍エンジニアでは、現役エンジニアと学習コーチの2名体制で学習をサポートしてもらえます。

「受講生の学習完了率98%」「累計受講者数4万5,000名以上」という実績からも、侍エンジニアなら未経験からでも挫折なく転職や副業収入の獲得が実現できますよ。

＼ 給付金で受講料が最大80%OFF ／

### git push　「ローカルリポジトリの変更点をリモートリポジトリにマージ」

「git push」はgit pullの反対で、指定したローカルリポジトリの変更内容をリモートリポジトリにマージするコマンドです。 **自分の変更内容をチーム開発用のリモートリポジトリにアップロードするため** に使われます。

ただし自分の想定していない変更をリモートリポジトリに入れると、チームに迷惑をかけてしまいます。git pushコマンドを実行する前には、後述の「git diff」コマンドにより差分のある箇所を確認しましょう。

```
$ git push [マージ先のリモートリポジトリ名] [マージ元のローカルリポジトリ名]
```

git pullコマンドと同様に、厳密にはマージ元・マージ先を省略できます。しかし正しく事前設定しないと想定外のリポジトリにマージされる恐れがあるので、おすすめしません。

以下の記事では実際にgit pushコマンドを使う方法をご紹介していますので、参考にしてくださいね。

## コミットを操作するコマンド

![コミットを操作するコマンド](https://www.sejuku.net/blog/wp-content/uploads/2021/01/image23.jpg)

コミットを操作するコマンド

画像：コミットのイメージ

「コミット」は、 **ローカルリポジトリに自分が変更した内容を入れ込むこと** です。コミットされたローカルリポジトリの変更内容が、前述のpushコマンド実行時にリモートリポジトリへマージされます。

コミット時には、変更者・変更日時・変更内容といった情報が変更履歴として記録されます。コミットを繰り返して、1つのリポジトリをバージョンアップさせていくのが開発の基本的な流れです。

この章では、コミットに関するGitコマンドを6つご紹介します。

### git add　「コミット対象のファイルを登録」

「git add」は、新たに追加/変更/削除したファイルをインデックスに追加するコマンドです。前述のとおり、コミット時にはインデックスに追加されたファイルがすべてローカルリポジトリに加えられます。

**元々Gitの管理対象となっていたファイルを削除（管理対象外に）する場合も、インデックスに追加＆コミットが必要** なので注意が必要です。

```
$ git add [追加/変更/削除したファイルパス1] [追加/変更/削除したファイルパス2] ・・・
```

上記のように半角スペース区切りでファイルパスを複数指定すると、ファイルを一括でインデックスに追加できます。また以下のようにすると、カレントディレクトリ配下で追加/変更/削除されたファイルを一括で追加できて便利です。

```
$ git add .
```

git addコマンドについてより詳しく知りたい方は、以下の記事もご覧くださいね。

### git commit　「変更されたファイルをコミット」

「git commit」は、 **インデックスに存在するすべてのファイルをコミット（ローカルリポジトリにマージ）するコマンド** です。新たに追加したファイルは、コミットすることで初めてGitの管理対象に加えられます。

```
$ git commit
```

git commitコマンドを実行すると、エディタが起動して変更履歴に記録するコミットメッセージの入力が求められます。エディタを起動したくない場合は以下のように、「-m」オプションとメッセージを指定すればOKです。

```
$ git commit -m "[コミットメッセージ]"
```

git commitコマンドについて更に知識を得たい方は、以下の記事もチェックしてはいかがでしょうか。

### git reset　「直前のコミットを取消」

コミットした後に、ミスに気づく場合もありますよね。このような場合は「git reset」コマンドを使うことで、直前のコミットを取り消せます。

```
$ git reset
```

git resetコマンドは主に、 **ローカルリポジトリへの変更を取り消すため** に使います。リモートリポジトリへの変更を取り消す際にも使えなくはありませんが、不整合が発生しやすいのでおすすめしません。

git resetコマンドをもっと使いこなしたい方は、以下の記事を読むとより高度な使い方が分かりますよ。

### git revert　「特定のコミットを取消」

「git revert」コマンドを使うと特定バージョンのコミットだけを取り消して、ローカルリポジトリにコミットできます。たとえば、変更A→変更B→変更Cの順にコミットした場合、 **変更Aと変更Cはそのままにして変更Bだけを取り消し可能** です。

ただし変更Bを取り消したとしても、当時の変更履歴は削除されないので注意しましょう。この場合、変更Bを取り消した旨の新たな変更履歴が追加されます。

```
$ git revert [取り消すコミットID]
```

なお、コミットIDは次章の「git log」コマンドを使用することで確認できます。git revertコマンドの情報がもっと欲しい方には、以下の記事もおすすめです。

### git log　「コミット履歴を表示」

「git log」は、ローカルリポジトリに自分がコミットした履歴を表示するコマンドです。さまざまな変更をコミットした後でも、このコマンドを使えば **後から開発状況を把握できます** 。

```
$ git log
```

表示される情報は、以下の通りです。

- **コミットID**
- **変更者の氏名・メールアドレス(基本的に自分の情報)**
- **変更日時**
- **コミット時に入力したコミットメッセージ**

### git tag　「コミットにタグを付ける」

「git tag」コマンドを使うと、直前のコミットに対して分かりやすい別名（タグ）を付けられます。たとえば重要な変更を入れた際にタグを付けておくと、 **変更履歴の確認時に目印となるので便利** です。

```
$ git tag [タグ名]
```

ローカルリポジトリのコミットに対して付けたタグを、リモートリポジトリに反映したい場合もありますよね。その場合は、git pushコマンドで以下のようにタグ名を指定して実行すればOKです。

```
$ git push origin [タグ名]
```

以下の記事ではgit tagコマンドを実際に使う方法をご紹介しているので、ぜひご覧ください。

## 作業ツリーを操作するコマンド

![作業ツリーを操作するコマンド](https://www.sejuku.net/blog/wp-content/uploads/2021/01/image43.jpg)

作業ツリーを操作するコマンド

画像：作業ツリーのイメージ

作業ツリー（ワーキングツリー）とは、 **プログラマーが実際に変更するファイルの格納されたディレクトリ** です。前述のgit initコマンドでリポジトリを作成したディレクトリとも言い換えられます。

作業ツリーのファイルをコミットする際には、あらかじめ「インデックス」に追加する必要があります。インデックスとはコミット対象ファイルを格納しておく場所で、「控え室」のようなものです。

この章では、作業ツリーに関するGitコマンドを4つご紹介します。

### git status　「作業ツリー内の差分ファイルを表示」

「git status」は、指定したディレクトリ内に下記いずれかの条件を満たすファイルがあれば、 **一覧で表示するコマンド** です。

- **Gitの管理対象に含まれていない（新たに追加した）ファイル**
- **インデックスに追加されたが、まだコミットされていないファイル**
- **インデックスに追加されていないが、変更されているファイル**

```
$ git status [表示するディレクトリ(省略可)]
```

ディレクトリを省略すると、作業ツリー全体のファイル状態を表示します。

git statusコマンドについてもっと詳しく知りたい方には、以下の記事もおすすめです。

### git diff　「ファイル内の差分箇所を表示」

「git diff」は、作業ツリー内の指定ファイルをリモートリポジトリのものと比較して、差分のある箇所を表示するコマンドです。前述のgit pushコマンドにより自分の変更をマージする前に、 **必ずこのコマンドで差分確認することをおすすめ** します。

```
$ git diff [変更を確認するファイル名またはディレクトリ(省略可)]
```

ディレクトリを指定した場合は、ディレクトリ内にある全ファイルの差分を一括で表示可能です。ファイルやディレクトリを省略した場合は、作業ツリー内にある全ファイルの差分を表示します。

git diffコマンドのさらに高度な使い方を知りたい方は、以下の記事も読むと良いでしょう。

### git mv　「ファイルを移動／ファイル名を変更」

「git mv」コマンドには、 **2つの用途が存在** します。

1つ目は、ファイルを指定したディレクトリに移動させる使い方。ただし作業ツリー内で移動するだけなので、コミットしないとローカルリポジトリには反映されません。

```
$ git mv [移動するファイル名] [移動先のディレクトリ]
```

2つ目は、ファイル名を変更する使い方。こちらの場合も作業ツリー内のファイル名が変わるだけなので、ローカルリポジトリに反映させるにはコミットが必要です。

```
$ git mv [変更前のファイル名] [変更後のファイル名]
```

### git stash　「作業ツリーの状態を一時的に保存」

「git stash」は、作業ツリーの状態を一時的に保存するコマンドです。作業ツリー内の変更内容をすぐにコミットしたくない場合、 **一時退避のため** に使われます。

```
$ git stash [実行コマンド]
```

実行コマンドの代表的なものは以下の4種類で、用途に応じて使い分けられます。

| 実行コマンド名 | **用途** |
| --- | --- |
| save | 作業ツリーの状態を保存 |
| list | 保存されたバックアップデータを一覧表示 |
| apply | 保存されたバックアップデータを使用する環境に戻す |
| drop | 保存されたバックアップデータを削除 |

git stashについてより詳しく知りたい方は、以下の記事もあわせて参考にしてください。

## ブランチを操作するコマンド

![ブランチを操作するコマンド](https://www.sejuku.net/blog/wp-content/uploads/2021/01/image33.jpg)

ブランチを操作するコマンド

画像：ブランチのイメージ

「ブランチ」とは、 **リモートリポジトリやローカルリポジトリをコピーして、分岐リポジトリを作る機能** です。複数人で並行しての開発や、1人で複数機能を開発する場合などにブランチ機能が良く使われます。

ただし複数のブランチを同時には処理できないため、Gitのシステム上で次に処理する対象のブランチは決められています。処理対象ブランチの確認・切り替えに使うコマンドについては、後述しますね。

この章では、ブランチに関するGitコマンドを4つご紹介します。

### git branch　「ブランチの作成／一覧表示」

「git branch」コマンドを使うと、 **現在処理対象となっているブランチを基にして新たなブランチを作成可能** です。以下のように、作成するブランチ名を指定します。

```
$ git branch [作成するブランチ名]
```

また以下のようにブランチ名を省略すると、現在のローカルブランチ（自分のパソコン内にあるブランチ）を一覧表示できます。

```
$ git branch
```

リモートブランチ（共有サーバー上にあるブランチ）を一覧表示したい場合は、以下のように「-r」を付けます。

```
$ git branch -r
```

git branchコマンドについてさらに理解を深めたい方は、以下の記事も読むと良いでしょう。

### git checkout　「処理対象ブランチの切り替え」

先ほど解説したとおり、Gitでは処理対象のブランチが決められています。処理対象のブランチを切り替えるために使うのが「git checkout」コマンドです。

```
$ git checkout [切り替えるブランチ名]
```

ブランチを切り替えた後にコミットを行うと、切り替え後のブランチに対して変更履歴が追加されます。 **チーム開発で自分の変更をマージする際に良く使われる** コマンドです。

### git merge　「別のブランチから変更点をマージ」

「git merge」は現在処理しているブランチに、別のブランチから変更点を取り込むコマンドです。 **各チームメンバーがブランチで変更した内容を、マスターリポジトリに集約する際** に良く使われます。

```
$ git merge [変更点の取り込み元ブランチ名]
```

このコマンドを使用する際は必ず、前述のgit checkoutコマンドで取り込み先のブランチに処理対象を切り替えましょう。

以下の記事では、git mergeコマンドについてさらに詳しく解説しているのでおすすめです。

### git rebase　「派生元ブランチに変更点をマージ」

たとえば、ブランチAをコピーしてブランチBを作成したとします。この時、ブランチBの基になったブランチAが派生元ブランチ。「git rebase」コマンドを使うとブランチBで入れた変更内容をすべて、派生元であるブランチAに取り込めます。

```
$ git rebase [派生元ブランチ名]
```

前述のgit mergeコマンドでブランチAに変更をマージした場合は、コミット当時の時系列にしたがって変更履歴が記録されます。するとブランチAとブランチBの変更履歴が入り混じってしまい、分かりづらくなるのが難点です。

その点git rebaseコマンドでブランチAに変更を取り込む場合は、新たに追記する形でブランチBの変更履歴が記録されます。そのため、 **変更履歴の見やすさを保ったままマージしたい方におすすめ** のコマンドです。

git rebaseコマンドのさらに高度な使い方を知りたい方は、以下の記事もぜひチェックしてくださいね。

## まとめ

今回は、良く使うGitコマンドを以下4カテゴリーに分けてご紹介しました。

- **リポジトリに関する5つのGitコマンド**
- **コミットに関する6つのGitコマンド**
- **作業ツリーに関する4つのGitコマンド**
- **ブランチに関する4つのGitコマンド**

Gitコマンドはとても種類が多く、この記事で紹介しきれていない便利なコマンドもまだまだあります。しかし今回ご紹介したGitコマンドを使えるようになれば、 **開発で困ることはかなり少なくなる** でしょう。

分からなくなったら、いつでもこの記事を読み返してくださいね。

[![](https://www.sejuku.net/blog/wp-content/uploads/2025/04/20250401-2.png)](https://lp.sejuku.net/lp1_blog_02/?cid=pro_popup_howto_0402&utm_source=blog&utm_medium=blog&utm_campaign=blog_Low_5816)