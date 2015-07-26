---
layout: pattern
title:  "Low Cost High Availability CDN"
categories: contents-delivery
date:   2015-07-27 13:00:00
author: marcy_terui
---

![Low Cost High Availability CDN](/images/low-cost-ha-cdn.png "Low Cost High Availability CDN")

# 概要
平常時は転送量課金が安い（というか無料）国内クラウドからコンテンツ配信しつつ、Route53のDNSフェイルオーバーでお手軽冗長化。フェイルオーバー先及びコンテンツのマスターは、堅牢性に定評のあるS3とする。

# 利用シーン
- スモールスタートな画像・動画配信系サイトなど
- 大容量コンテンツへのアクセス集中時の一時的処置

# 注意事項
- 大きくなったらちゃんとお金を払ってCDN使うべき
- 普通のサイトは平常だと転送量課金 < VM代金となる可能性有り
