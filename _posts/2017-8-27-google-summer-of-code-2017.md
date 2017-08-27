---
title: Google Summer of Code 2017
date: 2017-08-27 11:00 +5:30
categories:
- event
- gsoc
layout: article
coverPhoto: /blog/images/gsoc-cover.png
---

I spend this summer doing [Google Summer of Code](https://summerofcode.withgoogle.com) with [Zulip](https://zulip.org). This blog post summarizes the work that I did. All my work was to improve or add new features to the [Zulip server](https://github.com/zulip/zulip/). As a result I was able to work on a multitude of areas covering frontend, backened, management commands etc.

![GSOC Image]({{site.baseurl}}/images/gsoc2017.png)

## Merged Pull Requests

* Except for the first table all other tables list pull requests that are aimed at solving one problem. The first tables lists pull requestss that are independent of each other.
* Note that all the pull requests listed in this section are merged. But most of them have closed label on it as Zulip merges pull requestss manually.

|**No**|**Pull Request**|
|1|Show detailed message why password is weak to user. [#5500](https://github.com/zulip/zulip/pull/5500)|
|2|Refactor email confirmation pathways to use common error handling [#5891](https://github.com/zulip/zulip/pull/5891)|
|3|Create helper to pass and parse coma separated emails to management commands [#6194](https://github.com/zulip/zulip/pull/6194)|
|4|List realms and show only users in the selected realm. [#6087](https://github.com/zulip/zulip/pull/6087)|
|5|Use get_realm in management commands [#6026](https://github.com/zulip/zulip/pull/6026)|
|6|/apps/: Detect the user OS and show the appropriate app by default. [#6192](https://github.com/zulip/zulip/pull/6192)|
|7|Add an PM from welcome bot on user creation. [#5342](https://github.com/zulip/zulip/pull/5342)|
|8|Move all_users option to ZulipBaseCommand [#6269](https://github.com/zulip/zulip/pull/6269)|
|10|Analytics: Add translation bundle and tags to stats page [#5755](https://github.com/zulip/zulip/pull/5755)|
|11|Implemented a feature to show user presence and last seen time in user popover. [#4487](https://github.com/zulip/zulip/pull/4487)|
|12|portico: Make backend validation errors similar to frontend. [#5609](https://github.com/zulip/zulip/pull/5609)|
|13|Use POST instead of PUT in endpoints which are not idempotent [#5721](https://github.com/zulip/zulip/pull/5721)|
|14|User .on('load') instead of .load() [#5930](https://github.com/zulip/zulip/pull/5930)|
|15|Send message only if notifications_stream is not deactived [#6249](https://github.com/zulip/zulip/pull/6249)|
|16|Create list_realms command [#6026](https://github.com/zulip/zulip/pull/6026)|
|17|Move add new default stream box to top. [#4745](https://github.com/zulip/zulip/pull/4745])|
|18|docs: Update the path of Supervisor config file. [#4700](https://github.com/zulip/zulip/pull/4700)|
|19|requirements: Add service_identity to scrapy.txt. [#5465](https://github.com/zulip/zulip/pull/5465)|
|20|management: Use Realm.objects.get instead of get_realm. [#5729](https://github.com/zulip/zulip/pull/5729)|
|21|create_user: Separate password help into multiple lines. [#5736](https://github.com/zulip/zulip/pull/5736)|


* One major project I was working on was to enable users to register to more than one organization in a Zulip instance. 
The following pull requests were made for accomplishing this. 



|**No**  |**Pull Request** | 
|----|-----------------------------------------------------------------|
|1   |Add get_user function [#4868](https://github.com/zulip/zulip/pull/4868)
|2 |Add get_user_for_mgmt function [#5022](https://github.com/zulip/zulip/pull/5022)
|3|Replace get_user_profile_by_email with get_user in management commands [#5737](https://github.com/zulip/zulip/pull/5735)
|4|Eliminate get_user_profile in remaining management commands [#5761](https://github.com/zulip/zulip/pull/5761)
|5|Replace get_user_profile_by_email with get_user [#5783](https://github.com/zulip/zulip/pull/5783)
|6|Replace get_user_profile_by_email in analytics, webhooks and avatar [#5808](https://github.com/zulip/zulip/pull/5808)
|7|Use get_user in zilencer, messages, and users [#5852](https://github.com/zulip/zulip/pull/5852)
|8|Replace get_user_profile_by_email [#5867](https://github.com/zulip/zulip/pull/5867)



* Upgraded all the python dependencies(35+) twice over the summer.

|**No**  |**Pull Request** | 
|----|-----------------------------------------------------------------|
|1|Python dependency upgrade [#6169](https://github.com/zulip/zulip/pull/6169)|
|2|Python dependency upgrade [#5450](https://github.com/zulip/zulip/pull/5450)|

* I also worked on many pull requestss that replaced hardcoded emails with helper functions.

|**No**|**Pull Request**|
|------|----------------|
|1|Add ZulipTestCase.mit_user() function [#4915](https://github.com/zulip/zulip/pull/4915)|
|2|Add example_email, mit_email + refactorings [#4948](https://github.com/zulip/zulip/pull/4948)|
|3|Use mit_email and example_email in test_bots.py [#4977](https://github.com/zulip/zulip/pull/4977)|
|4|Replace mit_user().email with mit_email(). [#5014](https://github.com/zulip/zulip/pull/5014)|
|5|Use example_email function in zerver/tests [#5041](https://github.com/zulip/zulip/pull/5041)|

## Unmerged Pull Requests

|**No**|**Pull Request**|**Reason for not getting merged**|
|------|----------------|-----------------|
|1|Make internal send private message take recipient user profile [#5904](https://github.com/zulip/zulip/pull/6137)| We decided to go with an alternative approach as in [#6175](https://github.com/zulip/zulip/pull/6137)|
|2|Refactor to get_user in zerver/mgmt/commands/ [#5324](https://github.com/zulip/zulip/pull/5324)|We decided to go with an alternative approach as in [#5735](https://github.com/zulip/zulip/pull/5735)|
|3|Use regex validation for full_name and realm_subdomain [#5441](https://github.com/zulip/zulip/pull/5441)|Decided to not replicate the form checking logic in front end|

## Work Remaining

* [#5656](https://github.com/zulip/zulip/pull/5441) needs some work before getting merged.





