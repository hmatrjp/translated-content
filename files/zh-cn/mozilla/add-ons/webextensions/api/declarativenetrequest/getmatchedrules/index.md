---
title: declarativeNetRequest.getMatchedRules
slug: Mozilla/Add-ons/WebExtensions/API/declarativeNetRequest/getMatchedRules
l10n:
  sourceCommit: 43e3ff826b7b755b05986c99ada75635c01c187c
---

{{AddonSidebar}}

返回扩展匹配的所有规则。调用者可以通过指定 `filter` 来过滤匹配的规则列表。此方法仅对具有 `"declarativeNetRequestFeedback"` 权限的扩展或为 `filter` 中指定的 `tabId` 授予 `"activeTab"` 权限的扩展可用。与活动文档无关且匹配超过五分钟的规则将不会返回。

## 语法

```js-nolint
let gettingMatchedRules = browser.declarativeNetRequest.getMatchedRules(
    filter                // 对象
);
```

### 参数

- `filter` {{optional_inline}}
  - : 一个用于过滤匹配的规则列表的对象。
    - `minTimeStamp` {{optional_inline}}
      - : `number`。如果指定，则仅匹配在指定时间戳之后的规则。
    - tabId {{optional_inline}}
      - : `number`。如果指定，则仅匹配指定标签页的规则。如果设置为 `-1`，则匹配与任何活动标签页无关的规则。

### 返回值

一个 [`Promise`](/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Promise)，其会兑现一个对象，具有以下属性：

- `rule`
  - : {{WebExtAPIRef("declarativeNetRequest.MatchedRule")}}。匹配规则的详细信息。
- `tabId`
  - : `number`。请求来源的标签页的 `tabId`，如果标签页仍然活跃。否则为 `-1`。
- `timeStamp`
  - : `number`。匹配规则的时间。时间戳对应于 JavaScript 的时间约定，即自纪元以来的毫秒数。

如果没有匹配的规则，则对象为空。如果请求失败，promise 将被拒绝并带有错误消息。

## 示例

{{WebExtExamples}}

## 浏览器兼容性

{{Compat}}

<!--
// Copyright 2015 The Chromium Authors. All rights reserved.
//
// Redistribution and use in source and binary forms, with or without
// modification, are permitted provided that the following conditions are
// met:
//
//    * Redistributions of source code must retain the above copyright
// notice, this list of conditions and the following disclaimer.
//    * Redistributions in binary form must reproduce the above
// copyright notice, this list of conditions and the following disclaimer
// in the documentation and/or other materials provided with the
// distribution.
//    * Neither the name of Google Inc. nor the names of its
// contributors may be used to endorse or promote products derived from
// this software without specific prior written permission.
//
// THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
// "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
// LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
// A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
// OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
// SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
// LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
// DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
// THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
// (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
// OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-->
