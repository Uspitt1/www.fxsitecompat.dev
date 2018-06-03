---
title: "ほとんどの非標準 CSS `display` 値が廃止されました"
date: "2018-06-02T20:25:00-04:00"
categories: ["css"]
tags: []
versions: ["62"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=879275"
      title: "Bug 879275 - Consider turning off -moz-box display types in untrusted stylesheets"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1288572"
      title: "Bug 1288572 - Hide -moz-prefixed display values from web content"
aliases:
    - "/ja/docs/2015/non-standard-css-display-types-will-be-removed/"
---
元々 Mozilla アプリケーション UI 向けに作られた、非標準の `-moz` 接頭辞付き CSS [`display`](https://developer.mozilla.org/docs/Web/CSS/display) プロパティ値がウェブコンテンツから使用できなくなりました。標準の [可変ボックスレイアウト](https://developer.mozilla.org/docs/Web/CSS/CSS_Flexible_Box_Layout) か [グリッドレイアウト](https://developer.mozilla.org/docs/Web/CSS/CSS_Grid_Layout) を代わりに使ってください。

* `-moz-deck`
* `-moz-grid`
* `-moz-grid-group`
* `-moz-grid-line`
* `-moz-groupbox`
* `-moz-inline-grid`
* `-moz-inline-stack`
* `-moz-popup`
* `-moz-stack`

当面、互換性問題への懸念から、以下の値は残されます。Firefox 開発者は [Telemetry](https://telemetry.mozilla.org/) を使って、これらの例外を廃止する前にウェブ上での使用状況を確認する予定です。

* `-moz-box`
* `-moz-inline-box`