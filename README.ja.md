# English0.1（E01）

**単語は小さく。意味は大きく。頭は自由に。**

**間違いを恐れない。意味を送ろう。**

English0.1（E01）は、ゲームやオンラインチャットで使うための、英単語を土台にした最小限のコミュニケーションシステムです。

英語の代わりになる言語ではありません。

目的は、少数の親しみやすい単語と、ごく少ない文法で、すばやく意思を伝えることです。

英語を少し勉強したものの、話したり書いたりする自信がない人を主な対象にしています。

大切なのは完璧さではなく、自信を持って意味を伝えることです。正確でも難しい単語より、学校・ゲーム・日常生活で見覚えのある単語を優先します。

## すぐ分かる例

次の例は、正式な128語だけを使っています。

```text
enemy north
run
wait
team all attack

enemy dead
team win
game good
```

意味の例：

```text
北に敵
走れ
待て
チーム全員で攻撃

敵は死んだ
チームの勝ち
良いゲーム
```

## 3層の語彙システム

### 第1層：Core E01

正式な語彙と、基本的なコミュニケーションルールです。

Core E01は、小さく、安定し、親しみやすく、使いやすい状態を保つよう設計します。

### 第2層：Universal Game Terms

多くのゲームで広く理解されている用語や略語は、コア語彙の語数に数えず使用できます。

例：

```text
GG
AFK
BRB
HP
XP
NPC
PvP
PvE
```

すでに多くのゲームで広く認識されているものだけを、この層に入れます。

### 第3層：Open Vocabulary

ゲーム固有の単語、名前、物、場所など、必要な英単語を自由に追加できます。

例：

```text
Creeper
diamond
redstone
zombie
```

E01の仕組みは単純なまま保ち、不足する細かな情報をOpen Vocabularyで補います。

## 2つの使い方

### Strict E01

正式語彙、数字、承認されたUniversal Game Termsだけを使います。

```text
enemy north
team wait
attack later
```

### Open E01

E01の仕組みを使いながら、重要な単語が足りないときは普通の英単語を追加します。

```text
door locked
need key
boss second floor
```

Open E01は、開発中の検証や実際のゲームプレイに役立ちます。何度も必要になる単語は、将来の正式語彙候補になります。

## 基本ルール

- メッセージは短くする。
- 基本的に1行で1つの意味を送る。
- 必要なら最も重要な単語を先に置く。
- 質問には `?` を使う。
- 緊急、感情、強い命令には `!` を使う。
- 句読点や記号を繰り返すと、強さを増やせる。
- 否定には `no` を使う。
- 必要なら複数形の `s` を付ける。
- 数字はいつでも使える。
- 意味が分かるなら語順は自由。
- 知っている単語を先に出す。完璧な文法は後でよい。

例：

```text
enemy here?
3 enemies
danger north
no run
team all attack!
help!!!
```

## 語彙システム

English0.1は現在、128の正式語彙を使います。

- Core Vocabulary：64語
- Additional Vocabulary：64語
- 合計：128語

将来は256語版、さらに512語版への拡張を検証する予定です。候補語は、レビューとテストを通過するまで正式語彙ではありません。

## Core Vocabulary（64語）

### 動作

go, come, run, stop, attack, see, give, take, eat, know, help, have, follow, start, end

### 状態

big, small, good, bad, fast, slow, new, old

### 結果

win, lose, dead

### 方角と移動

north, south, east, west, left, right, here, there, move, up, down, clear

### 時間

now, later

### 接続・反応

no, ok

### 人と集団

man, woman, child, friend, enemy, team

### 基本概念

AI, game, world, map, house, food, water

### 命令

wait, open, close, all

### 戦術

danger, need, target

### 数量

many

## Additional Vocabulary（64語）

### 距離と位置

near, far, back, front, center

### 戦術支援

heal, cover, safe, hold, protect, low

### ゲーム進行

spawn, respawn, base, camp, loot, drop, build, break

### 装備とアイテム

weapon, ammo, shield, armor, tool, item, bag, money

### プレイ状態

ready, again, pause, continue, join, leave

### 感情と交流

nice, great, thanks, sorry, fun, cool

### 会話

like, want, think, tell, ask

### 数量

few

### 一般的なゲーム語

push, rush, mid, boss, quest, trade, party, level

### MMO・サンドボックス

farm, mine, craft, block, village, shop, sell, buy

## 数字

数字は世界共通のため、語彙数に数えません。

```text
1 enemy
3 team
10 food
```

## 繰り返しルール

単語を繰り返すと意味が強くなります。感情が伝わる限り、回数に固定の上限はありません。

```text
nice = 良いね
nice nice = とても良いね
nice nice nice = ものすごく良いね
help = 助けて
help help = 急いで助けて
HELP!!! = 最大級の緊急事態
```

句読点や記号の繰り返しでも、感情や緊急度を強められます。

## 単語結合ルール

単語を組み合わせて、より大きな意味を作ります。

```text
enemy house = 敵の拠点
team help = 支援
 danger north = 北が危険
target enemy = この敵を攻撃
```

## 文法のまとめ

English0.1には複雑な文法がありません。

親しみやすい単語、自由な語順、繰り返し、句読点、単語の組み合わせを使って意味を伝えます。

正しい英語で書いても構いませんが、正しい英語である必要はありません。

```text
enemy north
team follow
attack now
old man give food
game good good
```

## バージョン規則

English0.1は、バージョンが進むほど英語に近づきますが、英語そのものにはなりません。

```text
0.11
0.12
0.13
...
0.19
0.191
0.192
```

バージョン `0.2` は禁止です。

## 英語への敬意

English0.1は英単語と簡単な英文法を土台にしています。

英語は世界中で使われる、力強く美しい言語です。English0.1は、ゲームやオンラインチャットで速く簡単に意味を伝えるための、小さな道具にすぎません。

English0.1をきっかけに、誰かが英語を学びたいと思ってくれたら、とても嬉しいです。

## 利用・改造・派生版

English0.1は、利用、複製、翻訳、改造、拡張、再配布、派生版の作成が可能です。

個人、教育、コミュニティ、商用のいずれにも利用できます。

English0.1を元にした作品やシステムを公開するときは、元のEnglish0.1を基にしていることと、次のGitHub URLを分かりやすい場所に記載してください。

```text
Based on English0.1 by kotto & Yomi
https://github.com/kotto0430/E01-language
```

表記場所は `Credits`、`Special Thanks`、`Acknowledgements` など、利用者が確認できる項目で構いません。

この出典表記があれば、個別の許可を取る必要はありません。

改造版は、このリポジトリで正式採用されていない限り、公式English0.1仕様を名乗らないでください。

## 翻訳について

翻訳版では、E01の英単語、例文、コード部分を勝手に現地語へ置き換えず、説明文を現地語に翻訳します。

翻訳者は直訳よりも、英語に自信のない読者が理解しやすい自然な説明を優先してください。

## 制作者

**kotto（Japan）& Yomi（ChatGPT）**
