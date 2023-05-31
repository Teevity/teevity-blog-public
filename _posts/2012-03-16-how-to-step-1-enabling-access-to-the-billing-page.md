---
layout: post
title:  "How-to : Step 1 - Enabling access to the Billing page"
date:   2012-03-16 04:03:00 -0400
---
<p>This post describes the first step needed to <a href="http://blog.teevity.com/post/19339445622/amazon-cloud-costs-monitoring-with-teevity-cloudcost" title="Teevity - Configure an Amazon IAM account" target="_blank">configure an Amazon IAM account for use with Teevity cloud costs analytics</a> solutions.</p>
<ul><li><b>Step 1 - Enable access to the Billing page</b></li>
<li><a href="http://blog.teevity.com/post/19399771650/aws-cloud-costs-monitoring-iam-security-group" title="Teevity - Create the IAM group" target="_blank">Step 2 - Create the IAM group</a></li>
<li><a href="http://blog.teevity.com/post/19399945507/aws-cloud-costs-monitoring-iam-user" title="Teevity - Create a new IAM user" target="_blank">Step 3 - Create a new IAM user and add it to the group</a></li>
</ul><p><br/><b>A/ Go to the Manage Account page on the AWS console</b> </p><p>Here is the link to this page on the AWS Portal<br/><a href="https://console.aws.amazon.com/billing/home#/account" target="_blank">https://console.aws.amazon.com/billing/home#/account</a></p><figure data-orig-width="1140" data-orig-height="568" class="tmblr-full"><img src="/assets/images/import/19400114920_0.png" alt="image" data-orig-width="1140" data-orig-height="568"/></figure><p><b>B/ Scroll down to the “IAM User Access to Billing Information” section</b></p><p>When you reach this section you simply have to</p><ul><li>check &ldquo;Activate IAM Access&rdquo;<br/></li><li>click the “Update” button<br/></li></ul><p>You’re done for this part.</p><figure data-orig-width="1656" data-orig-height="498" class="tmblr-full"><img src="/assets/images/import/19400114920_1.png" alt="image" data-orig-width="1656" data-orig-height="498"/></figure><p><b>C/ Next step : Create an IAM group with read-only rights</b></p>
<p>Here is <a href="http://blog.teevity.com/post/19399771650/aws-cloud-costs-monitoring-iam-security-group" title="Teevity cloud costs analytics - Creating an IAM group with the appropriate right only rights" target="_blank">how you can do it</a> in two easy steps.</p>
 