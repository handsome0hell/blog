---
title: Missing Phone from Find My Device
date: 2023-10-14 07:22:00
excerpt:
  <p>Due to security reasons, the new phone was installed with the <a target="_blank" rel="noopener" href="https://github.com/oasisfeng/island">Island</a> app to separate personal and work apps. I finally discovered that it was the reason my phone didn't appear in the Find My Device.</p>
---

> Keep Paranoid, Beyond Anxiety

## A New Phone

My phone is always hidden in some inconspicuous corner at home, maybe under the sheets, maybe in the crevices of the sofa, maybe on top of the refrigerator. I've gotten used to asking my speaker where my phone is immediately, which saves me a lot of time.

Until half a year ago, a new phone didn't show up in the list of Find My Device. Turned the option off and on, on and off, deleted and added my Google account, added and deleted it, contacted Google One customer service, contacted Samsung customer service, none of these solved the problem.

## The Island

Once again the issue comes into my mind, habitually delete my Google account and add it back. Intuition made me notice the words "Sign in with your **work** account" displayed while adding account.

Due to security reasons, the new phone was installed with the [Island](https://github.com/oasisfeng/island) app to separate personal and work apps. I finally discovered that it was the reason my phone didn't appear in the Find My Device.

Island provides a feature called ["Managed Mainland"](https://island.oasisfeng.com/#managed-mainland), which allows it to control personal apps. Island needs to be a Device Admin to enable this feature, and it makes Google think this is a managed device. Either by expectation or a bug, Google doesn't enable Find My Device for this device, but I still see the option (definitely a Google's problem).

## The Solution

Obviously, turn off the "Managed Mainland“, the normal "Sign in with your Google Account" words will show up during adding account, then the Samsung Galaxy S23 Ultra, delayed by half a year, appeared in the list of Find My Device. This does not affect the primary functionality of Island, and adb can freeze apps directly if it's necessary.

Finally, I no longer have to search the entire room for my phone that was sitting right under some butt, YEAAAAAH!
