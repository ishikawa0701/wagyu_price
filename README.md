# Git Lesson

## リモートリポジトリとローカルリポジトリとはそれぞれ何でしょうか？
リモートリポジトリはネット上に配置して複数人で共有するためのリポジトリ
現在使用しているリモートリポジトリはgit hubというホスティングサービスでPublicリポジトリというネット上に公開して誰でも見ることができるもの
Privateリポジトリで作成すれば共同編集者として登録している人しか見ることができないというもできる
ローカルリポジトリは開発者一人ひとりが使用するために自分のPC上に配置するためのリポジトリ


## プッシュとマージの違いは何でしょうか？
マージはブランチの変更内容を別のブランチに変更内容を反映させる
プッシュはローカルリポジトリの変更内容をリモートリポジトリに反映させる


## コミットとプッシュの違い
コミットは変更した内容をローカルリポジトリに反映させる
プッシュはその変更したローカルリポジトリをリモートリポジトリに反映させる


## コミットのメッセージはどのように書いてあげるのが最適でしょうか？
何をどのようにしたのか誰が見てもわかりやすいように書く
プレフィックスという頭文字を使うことでどのような変更をしたか一目でわかりやすく書くことが多い
feat:○○という機能を追加 fix:○○で発生するバグを修正 refactor:○○の機能をリファクタ
などがある


## ローカルでマージするフローと、プルリクエストでマージするフローの違いは何でしょうか？
ローカルでの場合は、変更したブランチをコミットした後にローカルの幹ブランチにマージしてリモートリポジトリに反映させる
プルリクエストでの場合は、コミットした後リモートリポジトリにプッシュしてレビュー担当者にプルリクエストをし承認されたらマージする


## コンフリクトを起こしてしまった場合、どう対処すべきですか？
・先にマージされた変更内容を取り込む
・後にマージしようとしてる変更内容を取り込む
・どちらの変更内容も取り込む
のいずれかを行う