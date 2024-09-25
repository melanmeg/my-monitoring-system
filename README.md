# my-monitoring-system-2
my-monitoring-system 2版
### ※未工事

- いつかやりたい用
- メモ）検証用なので、mimir, loki, minio, pyroscope辺りはリソースの関係から分散は辞めたい

```bash
# 構想
ダッシュボード
  ・grafana
  ・kiali
ネットワーク
　・cilium: ネットワーク制御
  　- hubble: メトリクス
　・istio: トレース、サービスメッシュ、ネットワーク制御
収集
　・otelcol: ログ、メトリクス、トレース
集積
　・minio: オブジェクトストレージ
　・mimir: メトリクスストレージ
　・loki: ログストレージ
バックエンド
　・tempo: トレース管理
　・prometheus: メトリクス管理、メトリクス
ポータル
　・backstage
クラスタートレース?プロファイリング
　・pixie: トレース?プロファイリング
プロファイリング
　・pyroscope: プロファイル、ebpf
セキュリティ
　・Falco ※暫定
```
