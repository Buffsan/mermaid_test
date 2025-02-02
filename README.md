# 課題
Mermaidを触ってみよう

マークダウンファイルを編集して、Mermaidで図を描いてみよう

# 取り組み方
* 本プロジェクトをforkしてください。
* README.mdを編集して、Mermaidを使いこなしてください
* できたらプルリクエストを出します

# 課題項目
## 流れ図
### 条件
- 開始と終了ノードをつける
- 条件分岐を組み込む
- 5ノード以上
- カッコいいほど高得点

## 解答
```mermaid
flowchart LR;
A([開始])　-->  B[/入力/]; B--> C{判断};　C--真--> F[四角];　F--> E([終了])
C　--偽-->D[[サブルーチン]];
D　--> B
```

## シーケンス図
### 条件
- 3人以上
- メッセージをやり取りしない人がいないように
- 自己呼び出しを含むこと
- カッコいいほど高得点

## 解答
```mermaid
sequenceDiagram
    actor 太郎
    actor 花子
    actor 連続殺人犯田中マイケルジョンソン
    太郎->>連続殺人犯田中マイケルジョンソン: おはよう！
    
    activate 連続殺人犯田中マイケルジョンソン
    連続殺人犯田中マイケルジョンソン-->>太郎: おはようございます!
    
    連続殺人犯田中マイケルジョンソン-->>太郎:うるせぇ殺すぞ
    連続殺人犯田中マイケルジョンソン-->>花子:うるせぇ殺すぞ
    
    deactivate 連続殺人犯田中マイケルジョンソン
```

## クラス図

### 条件
- 3つ以上
- 汎化と集約を含むこと
- カッコいいほど高得点

## 解答
```mermaid
classDiagram
    キャラクター o-- アイテム
```
