---
layout: page
---

### Multi Cloud Design Pattern(Beta)とは？
クラウドの垣根を越えた、アーキテクチャ設計ノウハウをデザインパターンとしてまとめ、ユーザによるユーザのための集合知を実現を目指しています。

### ルール
- 新パターンの提案や修正はPull Requestにて行ってください。
- 公平性を期すため、一度パターンが採用された人にはコミット権を付与します。
- 古くなったパターンなどはIssueで議論の上削除・修正します。
- 最低限、実証済みのパターンのみを登録します。
- 特定の事業者を貶めるような内容はNGです。
- 本ルール自体もIssueで議論の上削除・修正します。


### パターンを考える際のポイント
- 基本は同一クラウド内で解決できるかどうかを考えましょう。
- むやみに色々使うと管理コストが上がります。
- 異なるクラウド間には必ずレイテンシがあることを考慮しましょう。
- 経路の暗号化はほぼ必須です。
- 転送量課金があることを念頭に置きましょう。
- ただ、データのみのやりとりだと意外と転送量課金は気にならない事が多いです。

### パターン
- [No VM Scheduled Job](/batch/no-vm-scheduled-job/)
- [Enhanced Scaling](/scaling/enhanced-scaling/)
- [Low Cost High Availability CDN](/contents-delivery/low-cost-ha-cdn/)
- [BigQuery for now](/analytics/bq-for-now/)

### Authors and Contributors
- Masashi Terui([@marcy_terui](https://github.com/marcy-terui))

### RSS
<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
