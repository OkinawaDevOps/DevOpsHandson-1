情報共有
------------------

## はじめに

DevOpsOkinawa#1 において共有しておくべき情報について以下に列挙することとします。

- すること、について
- 用意しておいて欲しい環境
- セッションで使う環境について
- 資料の URL など

## すること、について

[Doorkeeper](http://devops-okinawa.doorkeeper.jp/events/6568) にて以下な案内をしています。

> 当初はハンズオンセミナー形式を予定しておりましたが、Coderetreat で採用されている方式に沿った形を取ってみようと考えております。基本的には
> 
> - Vagrant などを使い、仮想リソースの構築
> - Puppet または Chef (あるいは Chef-Solo) などを使い、サービスなどの導入
> - serverspec などを使い、動作の検証
> 
> をペアを組んで行なう形を取ります。45 分を一つの単位として、ペアをその度に作りかえる方向で考えています。また、サービスの導入についてはペア毎で決めて頂いてかまいません。

[ここ](http://yamanetoshi.github.io/blog/2013/11/18/devops-okinawa-11-23/) で羅列しているのは以下ですね。

- Chef あるいは Puppet で作って serverspec で試験する流れを学ぶ
- 実際のユースケイスを想定して色々ヤッてみる
- 必要な cookbook を作る (Chef)
- 流通している cookbook を適用してみる (Chef)
- Debian 系と RHL 系のパケジ管理の抽象化について確認してみる

ただ、初心者な方も、という話は聞いているのでまず流れてきな部分を、という事もありだとは思っています。

## 用意しておいて欲しい環境

以下は必須になると思っていますが、vagrant などを使う場合はその限りではないかもしれません。ただ、Ruby は必須になるはずです。

- Chef-Solo、knife-solo、serverspec が実行できる
- ssh でリモート接続できる

## セッションで使う環境について

IDCF さまから仮想リソースを提供頂いています。が、使用はマストではありませんので、お好きな環境をお使い頂いて構いません。

以下に提供を予定している環境について簡単に列挙しておきます。

- 用意している Linux の配布系は Ubuntu のみです
- ssh 接続可能
  - ポートはデフォルトから変更しています (詳細は当日案内します)
  - 鍵については事前に案内させて頂きます
- 接続ユーザはパスワード入力無しで sudo できます

## 資料の URL など

- [Serverspec のはじめかた](http://yamanetoshi.github.io/blog/2013/11/05/how-to-begin-serverspec/)
- [ChefSoloの正しい始め方](http://tsuchikazu.net/chef_solo_start/)
- [Vagrant + Chef Handson 材料](https://github.com/yamanetoshi/vagrant-chef-handson)
- [Vagrant 導入など](https://github.com/yamanetoshi/vagrant-chef-handson/blob/master/vagrant.md)

