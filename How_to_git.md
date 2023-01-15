## このマークダウンについて
Gitについて学習したことのメモ書き

## Gitのリポジトリ関係について
- ワークツリー
    - 実際に作業をしているディレクトリであり、コードの編集をここで行う
- インデックス 
    - リポジトリとワークツリーの差分(変更箇所)を記録する場所
    - 「git add ファイル名」でワークツリーからインデックスにファイルを登録する
- ローカルリポジトリ
    - 自分のPC環境内でファイルやディレクトリの状態を記録する場所
- リモートリポジトリ
    - ネット上でファイルやディレクトリの状態を記録する場所

### Gitのファイル更新の流れ
- git checkout [オプション] ブランチ名
    - 作業を行うブランチを切り替えるコマンド
    - 指定したブランチがない場合、切り替えに失敗する
    - オプション「-b」で新たにブランチを作ることができる 
- git branch
    - 現在のブランチの場所と種類を確認できる
    - 「git checkout」実行後の確認に使用する
- git add ファイル名
    - ワークツリーからファイルをインデックスに登録するコマンド
    - リポジトリとワークツリーの差分（変更箇所）のみを登録する
    - ファイル名を「.」にするとワークツリー内のすべてのファイルが対象になる
- git status
    -  ディレクトリの情報（ブランチやファイルの変更、インデックスへの追加など）を確認できる
    - 「git add」実行後に、ファイルが登録されているかを確認する
- git comnmit [オプション] -m "コミットメッセージ"
    - インデックスに追加されたファイルをローカルリポジトリにコミットする
    - コミットメッセージには変更した内容や追加したファイルなどの具体的な情報を記述する
    - オプション[--amand]で直前のコミットメッセージを修正できる
- git push [オプション] origin ローカルブランチ名
    - ローカルブランチの情報をリモートリポジトリに送信するコマンド
    - 「origin ブランチ名」でリモートリポジトリにある同じ名前のブランチに内容を更新する
    - オプション[-u]で送信先と送信元を固定でき、次からの送信するときは「git push」のみでよくなる
 