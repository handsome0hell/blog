---
title: Find My Device 中消失的手机
date: 2023-10-14 07:22:00
excerpt:
  <p>出于安全性考虑，新手机里使用了<a target="_blank" rel="noopener" href="https://github.com/oasisfeng/island">「炼妖壶（Island）」</a>这个 App 来隔离私人和工作的 App。我终于发现它是我的手机没有出现在 Find My Device 的原因。</p>
---

> Keep Paranoid, Beyond Anxiety

## 新手机

我的手机总会藏在家里某个不起眼的角落里，也许被子下，也许沙发缝，也许冰箱上。我习惯了在第一时间问音箱我的手机去了哪里，能帮我省不少时间。

直到半年前，一部新手机没有出现在 Find My Device 的列表里。把选项关了又开，开了又关，把 Google 账号删了又加，加了又删，联系 Google One 的客服，联系三星的客服，都没能解决这个问题。

## The Island

我又想起了这个问题，习惯性地删掉 Google 账号，再添加回去。直觉让我注意到了添加账号时显示的「Sign in with your **work** account」字样。

出于安全性考虑，新手机里使用了[「炼妖壶（Island）」](https://github.com/oasisfeng/island)这个 App 来隔离私人和工作的 App。我终于发现它是我的手机没有出现在 Find My Device 的原因。

Island 提供了一个叫 [「Managed Mainland」](https://island.oasisfeng.com/#managed-mainland) 的功能，允许它对私人的 App 进行管理。Island 需要成为 Device Admin 才能启用这项功能，而这会让 Google 认为这是一台受管理的设备。出于预期或是 Bug，Google 不会为这台设备启用 Find My Device，但我依然能看到相关的选项（这绝对是 Google 的问题）。

## 解决方案

显而易见，只要关掉 「Managed Mainland」，添加账号时就会显示正常的「Sign in with your Google Account」字样了，随后这部迟到了半年的 Samsung Galaxy S23 Ultra 就出现在了 Find My Device 的列表里。这不影响 Island 的主要功能，需要冻结 App 的时候也可以直接用 adb 操作。

终于我不用再满房间找被坐在屁股底下的手机了，好耶！