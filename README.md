# BoardGate
ボードゲームを題材としたマッチングアプリです。  
私自身が趣味としてボードゲームをやっていた際に、一緒に遊ぶ人を探すということが意外に難かしいなと感じていたので、興味のあるボードゲームを探して、それをやりたいと思ったときに一緒に遊ぶ人を探すことを手助けできるようなWebアプリがあればいいなと思って作成しました。  
ターゲットとしては、「**ボードゲームに少し興味があるけど、どれから遊んでみればいいか分からない**」ような初心者から、「**遊んでみたいボードゲームはたくさんあるけど周りに一緒にやってくれる人がいない**」といった中～上級者まで幅広い人達を対象としています。

# 使用した技術
OS Windows  
Django 3.2.13  
HTML/CSS  
Boostrap4  


# 機能一覧
- 会員登録機能・ログイン機能
- CRUD機能
- マッチング機能
- コメント機能
- 検索機能
- 興味あり機能

# 工夫した点・苦労した点
- **マッチング機能に関して**
  - ネットで調べてみてもDjangoでマッチングアプリを作成している情報や教材はなかったので、今まで学習してきた知識を組み合わせてマッチング機能を何とか実装しました。情報が少ない中で、自分でアプリケーションの仕組みを一から考えるのは大変で、考慮しなくてはならないことの多さを痛感しました。
  
- **モデル設計に関して**
  - アプリを設計する上で一番苦労したのはモデルの設計でした。
  - 特に苦労した点はモデルのリレーション関係で、リレーションに関する理解が足りていなかったため、自分の意図するフィールドの値を上手く取得できず、とても苦労しました。
  - また、重複制限に関しても、最初はDB制約のみで実装していましたが、その場合だと自分の期待する結果にならなかったため、Views側でコントロールするようにしました。

- **ウェルカムページに関して**
  - ウェルカムページはユーザーが最初に目にするページなので、見た時にそのサイトに興味が沸くように、サイトで公開されているボードゲームが目に入るようなデザインにしました。
