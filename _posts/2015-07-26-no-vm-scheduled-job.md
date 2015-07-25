---
layout: pattern
title:  "No VM Scheduled Job"
categories: batch
ate:   2015-07-26 01:18:48
author: marcy_terui
---

![No VM Scheduled Job](/images/no-vm-scheduled-job.png "No VM Scheduled Job")

# 概要
AzureのマネジメントサービスであるJob SchedulerのHTTP Request機能を使い、AWSのAPI Gatewayにリクエストを飛ばすことでLambda Functionを起動することで、EC2やAzure VMを一切使わずに定時処理を行う。
