■ サービス概要
このWEBアプリは、大相撲の試合の盛り上がり度合いがどれ程のものになるかをシミュレーションするツール系アプリです

■ このサービスへの思い・作りたい理由
私は１０数年来の大相撲ファンですが、自分がどういった経緯で大相撲ファンになっのかを振り返った時に
「大相撲の試合には何年経っても語り継がれる名試合があるのはなぜだろう？」
「どうして大して盛り上がらない試合と大いに盛り上がる試合があるのだろう？」
「盛り上がる試合がなぜ盛り上がっているのかを相撲観戦の初心者にわかってもらうにはどうすればいいか？」
と考えを巡らせ気軽に初心者やファンが試合を楽しむ手助けをするプログラムを作ってみようと思いました

■ ユーザー層について
このアプリは大相撲に興味を持つ全ての人を対象としています
また、相撲の魅力を理解しようとしている初心者や、楽しみながら試合を観戦したい人にも利用されることを期待しています

■ サービスの利用イメージ
ユーザーは、取組の何日目か、東方力士と西方力士の番付、両者の前日までの対戦成績、試合結果を選択・入力し
ボタンをクリックすることで入力された条件に応じてその試合がどの程度の盛り上がりを見せるかをシミュレーションし
盛り上がり度合いを数値で得ることができます
その数値を「取組の熱量スコア」として表示し、数値が低ければ盛り上がりが小さくて高ければ盛り上がりが大きくなる仕様とし
試合の結果によって得られる感情的な価値を表現する指標としてユーザーに提供します

■ サービスの差別化ポイント・推しポイント
このアプリは、過去に実在した力士や現役の力士個人の情報には依存せずにユーザーが自由に選択した情報に基づいて熱量スコアを算出します
これにより、大相撲に関する知識や情報に差がある全てのユーザーが直感的に楽しめると思います
取組に対する新しい視点を提供し、現実には起こり得ない条件でのシミュレーションもできるため
ファン同士の会話のきっかけにもなればと考えています

■ 機能候補
取組の日程を選択（初日・2日目・3日目・4日目・5日目・6日目・7日目・中日・9日目・10日目・11日目・12日目・13日目・14日目・千秋楽）をプルダウンで選択
東方力士と西方力士の番付をそれぞれ選択（横綱・大関・関脇・小結・前頭１枚目〜１５枚目までをプルダウンで選択）
前日までの対戦成績を選択（2日目なら１勝０敗か０勝１敗のどちらかを選択する・※白星＋黒星＝取組日程−１となるように選択できるようにする）
試合結果の入力（東方力士勝利・西方力士勝利のどちらかをプルダウンで選択）
最後に「盛り上がり度合いを見る」ボタンを押すことで熱量スコアを算出し表示する

本リリース時
ユーザーごとのシミュレーション結果の保存と閲覧
熱量スコアに応じて自動でコメントを表示

■ 機能の実装方針予定
Railsを用いてバックエンドを構築し、フロントエンドはシンプルなHTML/CSSで実装する予定です
「取組の熱量スコア」の算出するプログラムのコーディング箇所はRailsのモデル層を想定しています
また算出方法については開発者である私個人の感覚で定義していく方針です

■技術スタック
バックエンド: Ruby on Rails
フロントエンド: HTML, CSS
データベース: PostgreSQL
開発環境: Docker
