---
nav_title: バッジ数の活用
article_title: バッジ数の活用
page_order: 8

page_type: reference
description: "この記事では、iOS バッジ数を使用して、プッシュに気付かなかったユーザーや、フォアグラウンドプッシュ通知を無効にしたユーザーに再エンゲージする方法について説明します。"
platform: iOS
channel: 
- push
- in-app messages

---

# バッジ数の活用

> iOS バッジ数には、アプリケーション内の未読通知の数が、アプリ アイコンの右上隅に赤い円の形で表示されます。近年、バッジはアプリユーザーを再エンゲージするための効果的な手段となっています。

バッジ数は、プッシュに気付かなかったユーザーや、フォアグラウンドプッシュ通知を無効にしたユーザーに再度エンゲージするために使用できます。同様に、アプリ内アップデートなどの未表示のメッセージについてユーザーに通知するためにも使用できます。

## Brazeによるバッジカウント

Brazeダッシュボードでプッシュ通知を作成する際に、必要なバッジ数を指定できます。これは、パーソナライズされたメッセージングを使用してユーザー属性に設定できるため、無限にカスタマイズ可能なロジックが可能になります。ユーザーの邪魔をせずにバッジ数を更新するサイレントプッシュを送信する場合は、プッシュに「Content-Available」フラグを追加し、そのメッセージの内容を空のままにします。

{% alert note %}
Androidのバッジ数を設定する方法を知りたいですか?Androidはプッシュ用のアプリのバッジを自動的に処理するため、Brazeにはバッジのカスタマイズ設定はありません。
{% endalert %}

### バッジ数の削除

バッジ数を 0 または "" に設定して、アプリのアイコンからバッジ数を削除します。また、Brazeは、アプリがフォアグラウンドにあるときにプッシュ通知を受信すると、自動的にバッジをクリアします。

## おすすめの方法

バッジの再エンゲージメント率を最適化するには、ユーザーエクスペリエンスを最もシンプルにする方法でバッジ設定を行うことが重要です。

### バッジの数を少なくする
調査によると、バッジの数が2桁を超えると、ユーザーは一般的にアップデートに興味を失い、アプリの使用を完全に停止することがよくあります。

> このルールには、アプリの性質に応じて例外があります (メール アプリやグループ メッセージング アプリなど)。

### バッジ数で表現できるものを制限する
バッジを付けるときは、通知をできるだけ明確かつ直接的にする必要があります。バッジ通知が表現できるものの数を制限することで、アプリの機能や更新についてユーザーに親しみを持たせることができます。
