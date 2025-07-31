# 
![alt text](carmeet-1.png)

## 開発背景

私はもともと車が好きなのですが、リアルでのオフ会や集まりには少しハードルの高さを感じていました。
そのため、自分のペースで関われるSNSという形に魅力を感じ、「みんカラ」や「カーチューン」といった車系SNSを試してみました。

しかし、みんカラはブログ形式で投稿のハードルが高く、カーチューンはUIが複雑で慣れるまでに時間がかかると感じました。
そういった経験から、「車は好きだけど、既存のコミュニティには馴染みにくい」と感じている人が、もっと気軽に・もっとシンプルに車を通じてつながれる場所が必要だと思うようになりました。

そこで私は、気軽に投稿できて、使いやすく、同じ車好き同士が安心して交流できるSNSアプリを自分で作ってみようと決意しました。
このCarMeetは、そうした想いから生まれたプロジェクトです。



## デモ画像


  <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 32px;">
  <div style="text-align: center; font-size: 16px;">
    <h2>ログイン画面</h2>
    <img src="login-page.png" alt="ログインページ" style="width:100%; max-height:300px; object-fit: contain;">
    <p>
      - ユーザーがメールアドレスとパスワードを入力してログインできます。<br>
      - JWTを用いた認証トークンの発行処理を実装しています。
    </p>
  </div>
 <div style="text-align: center; font-size: 16px;">
    <h2>新規会員登録</h2>
    <img src="signup-page.png" alt="サインアップページ" style="width:100%; max-height:300px; object-fit: contain;">
    <p>
      - ユーザー登録が可能な画面です。<br>
    </p>
  </div>
  <div style="text-align: center; font-size: 16px;">
    <h2>ホーム画面</h2>
    <img src="index-page.png" alt="ホーム画面" style="width:100%; max-height:300px; object-fit: contain;">
    <p>
      - CarMeetのトップページです。<br>
      - カテゴリ別の絞り込み・並び替えに対応しています。
    </p>
  </div>
  <div style="text-align: center; font-size: 16px;">
    <h2>マイページ画面</h2>
    <img src="profile-page.png" alt="プロフィール画面" style="width:100%; max-height:300px; object-fit: contain;">
    <p>
      - 登録されたユーザー情報（名前・紹介・趣味など）を表示するマイページです。
    </p>
  </div>
  <div style="text-align: center; font-size: 16px;">
    <h2>プロフィール編集画面</h2>
    <img src="edit-profile-page.png" alt="プロフィール編集画面" style="width:100%; max-height:300px; object-fit: contain;">
    <p>
      - プロフィール情報を編集できます。<br>
      - 新規会員登録の項目から新たに、カーライフ歴やプロフィール画像などの追加設定ができます。
    </p>
  </div>
  <div style="text-align: center; font-size: 16px;">
    <h2>投稿一覧画面</h2>
    <img src="postlist-page.png" alt="投稿一覧" style="width:100%; max-height:300px; object-fit: contain;">
    <p>
      - 投稿を評価順・予約順・新着順で並び替えて表示できます。<br>
      - 投稿キャプションや画像も一目で確認できるようにしています。
    </p>
  </div>
  <div style="text-align: center; font-size: 16px;">
    <h2>トークルーム一覧（ワイヤーフレーム）</h2>
    <img src="Car Meet ワイヤーフレーム（トークルーム）.drawio-1.png" alt="トークルーム一覧 WF" style="width:100%; max-height:350px; object-fit: contain;">
    <p>
      - トークルームの一覧を表示する想定の画面です。<br>
      - クリックでトークルーム詳細に遷移する構成です（未実装）。
    </p>
  </div>
  <div style="text-align: center; font-size: 16px;">
    <h2>トークルーム詳細（ワイヤーフレーム）</h2>
    <img src="Car Meet ワイヤーフレーム（トークルーム詳細）.drawio-1.png" alt="トークルーム詳細 WF" style="width:100%; max-height:380px; object-fit: contain;">
    <p>
      - メッセージの吹き出し表示や送信フォームの配置を検討しています。<br>
      - ユーザーごとの発言表示を左右で分けた構成です。
    </p>
  </div>
  <div style="text-align: center; font-size: 16px;">
    <h2>投稿作成画面（ワイヤーフレーム上部）</h2>
    <img src="Car Meet ワイヤーフレーム（投稿作成ページ（写真・動画投稿を選択した場合））.drawio-1.png" alt="投稿作成 上部 WF" style="width:100%; max-height:500px; object-fit: contain;">
    <p>
      - 投稿作成時に、タイトル・キャプション・写真 or 動画の選択ができる構成です。<br>
      - 入力フォームやファイル選択UIの配置を確認できます。
    </p>
  </div>
  <div style="text-align: center; font-size: 16px;">
    <h2>投稿作成画面（ワイヤーフレーム下部）</h2>
    <img src="Car Meet ワイヤーフレーム（投稿作成ページ（写真・動画投稿を選択した場合））.drawio-2.png" alt="投稿作成 下部 WF" style="width:100%; max-height:500px; object-fit: contain;">
    <p>
      - 投稿内容の確認・カテゴリ選択・送信ボタンの配置構成です。<br>
      - ページ下部の構成まで見えるよう、縦に分割して表示しています。
    </p>
  </div>

</div>


## 🛠 技術スタック

| 種類         | 使用技術                         |
|--------------|----------------------------------|
| フロント     | HTML / CSS / JavaScript |
| バックエンド | Java                               |
| フレームワーク| SpringBoot                        |
| DB           | MariaDB                           |
| 認証         | JWT（JSON Web Token）              |
| その他       | Maven / Git / Postman / Figma     |

## ER図

<div style="text-align: left;">
  <img src="Car Meet ER図.drawio.png" alt="ER図" style="max-width: 100%; max-height: 600px; object-fit: contain;">
</div>

## 今後の展望

<hr />

<h3>■ 第1フェーズ：コア機能の完成</h3>
<ul>
  <li>トークルーム作成・一覧機能と投稿作成機能の実装</li>
  <li>ローカル画像管理からAmazon S3への移行</li>
  <li>投稿・プロフィールのバリデーション精度向上とUIの整理</li>
</ul>

<h3>■ 第2フェーズ：運営・管理基盤の整備</h3>
<ul>
  <li>管理者機能の実装（ユーザー・投稿の管理）</li>
  <li>投稿・通報・ブロックの管理パネル設置</li>
  <li>会員一覧・詳細、退会対応機能の構築</li>
</ul>

<h3>■ 第3フェーズ：SNSとしての拡張</h3>
<ul>
  <li>コメント機能・いいね機能の追加</li>
  <li>フォロー・ブロック・通報機能の実装</li>
  <li>タグ検索・投稿検索機能の整備</li>
</ul>

<h3>■ 第4フェーズ：コミュニケーション強化と最適化</h3>
<ul>
  <li>DM（ダイレクトメッセージ）機能</li>
  <li>通知機能（いいね・コメント・フォローなど）</li>
  <li>アクセス分析・ユーザー行動の統計機能（管理画面）</li>
</ul>
