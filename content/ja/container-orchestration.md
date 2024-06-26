---
title: コンテナオーケストレーション
status: Completed
category: コンセプト
---

[コンテナ](/ja/container/)オーケストレーションとは、流動的な環境において、[コンテナ化](/ja/containerization)されたアプリケーションのライフサイクルを管理し自動化することを指します。
これはコンテナオーケストレータ(ほとんどの場合は[Kubernetes](/ja/kubernetes))を通じて実行され、デプロイメント、(自動)スケーリング、自動ヒーリング、モニタリングが可能になります。
オーケストレーションという言葉は比喩です。
オーケストレーションツールは、音楽指揮者のようにコンテナを指揮し、すべてのコンテナ(または音楽家)が適切に機能するようにします。

## 解決すべき問題は何ですか

スケールに応じて[マイクロサービス](/ja/microservices-architecture)、セキュリティ、ネットワーク通信や一般的な[分散システム](/ja/distributed-systems)を管理することは、手動で行うには難しく、場合によっては不可能です。
コンテナオーケストレーションにより、これらすべての管理タスクを自動化することができます。

## どのように役に立つのでしょうか

コンテナオーケストレーションツールは、ユーザーがシステムの状態を決定することを可能にします。
まず、システムがどのようにあるべきかを宣言します(例えばx個のコンテナ、y個のPodなど)。
その後、オーケストレーションツールは自動的にインフラを監視し、現状が宣言した状態から逸脱した場合には修正します(例えばコンテナがクラッシュした場合に新しいコンテナを立ち上げるなど)。
この自動化により、プロビジョニング、デプロイメント、スケーリング（増減）、ネットワーキング、ロードバランシングといった、エンジニアリングチームが手作業で行う複雑な運用タスクが大幅に簡素化されます。
