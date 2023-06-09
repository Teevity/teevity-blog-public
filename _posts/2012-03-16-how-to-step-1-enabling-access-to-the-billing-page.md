---
layout: post
title:  "How-to : Step 1 - Enabling access to the Billing page"
date:   2012-03-16 04:03:00 -0400
redirect_from:
  - /post/19400114920/aws-cloud-costs-monitoring-enabling-iam-billing-access
---
<p>This post describes the first step needed to <a href="{% post_url 2012-03-16-how-to-use-teevity-for-amazon-cloud-costs-monitoring-with-a-read-only-iam-user %}" title="Teevity - Configure an Amazon IAM account" target="_blank">configure an Amazon IAM account for use with Teevity cloud costs analytics</a> solutions.</p>
<ul><li>Step 1 - Enable access to the Billing page </li>
<li><a href="{% post_url 2012-03-16-how-to-step-2-create-a-dedicated-iam-group %}" title="Creating an Amazon IAM account for Cloud costs monitoring with Teevity" target="_self">Step 2</a> - Create an IAM group dedicated to Cloud cost monitoring</li>
<li><a href="{% post_url 2012-03-16-how-to-step-3-create-the-amazon-iam-user-dedicated-to-teevity %}" title="Creating an Amazon IAM account for Cloud costs monitoring with Teevity" target="_self">Step 3</a> - Create a new IAM user and add it to the group</li>
</ul><p><br/><b>A/ Go to the Manage Account page on the AWS console</b> </p><p>Here is the link to this page on the AWS Portal<br/><a href="https://console.aws.amazon.com/billing/home#/account" target="_blank">https://console.aws.amazon.com/billing/home#/account</a></p><figure data-orig-width="1140" data-orig-height="568" class="tmblr-full"><img src="/assets/images/import/19400114920_0.png" alt="image" data-orig-width="1140" data-orig-height="568"/></figure><p><b>B/ Scroll down to the “IAM User Access to Billing Information” section</b></p><p>When you reach this section you simply have to</p><ul><li>check &ldquo;Activate IAM Access&rdquo;<br/></li><li>click the “Update” button<br/></li></ul><p>You’re done for this part.</p><figure data-orig-width="1656" data-orig-height="498" class="tmblr-full"><img src="/assets/images/import/19400114920_1.png" alt="image" data-orig-width="1656" data-orig-height="498"/></figure><p><b>C/ Next step : Create an IAM group with read-only rights</b></p>
<p>Here is <a href="{% post_url 2012-03-16-how-to-step-2-create-a-dedicated-iam-group %}" title="Teevity cloud costs analytics - Creating an IAM group with the appropriate right only rights" target="_blank">how you can do it</a> in two easy steps.</p>
 