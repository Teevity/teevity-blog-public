---
layout: post
title:  "No more confidentiality issues with Amazon AWS cloud cost tracking solutions"
date:   2012-03-09 3:40:00 -0400
redirect_from:
  - /post/19003674956/no-more-confidentiality-issue-with-aws-cost-tracking-too
---
 <p>Great news ! Amazon <a href="http://aws.typepad.com/aws/2012/03/new-iam-feature-control-activity-to-account-and-usage-pages.html?utm_source=feedburner&amp;utm_medium=feed&amp;utm_campaign=Feed%3A+AmazonWebServicesBlog+%28Amazon+Web+Services+Blog%29" title="IAM users can now have access to AWS Account Billing pages" target="_blank">just announced</a> today that IAM users can now be given access to the Account Activity page which contains billing information.</p>
<p><figure class="tmblr-full" data-orig-height="445" data-orig-width="500"><img src="/assets/images/import/19003674956_0.png" data-orig-height="445" data-orig-width="500"/></figure></p>
<p>This is not only great news for all the people involved in Amazon AWS projects whom were bared access from the previous billing information and can now access it (this was much needed, for instance to <strong>enable software architects to measure the cost impact of their technical decisions</strong>).</p>
<div></div>
<p>But it&rsquo;s also a great news for the users of <a href="http://cloudcost.teevity.com" title="Teevity Cloud cost - Tracking and analytics for Cloud spendings" target="_blank">Cloud cost tracking and analytics</a> products like <a href="http://cloudcost.teevity.com" title="Cloud costs tracking for AWS, Google AppEngine, OVH " target="_blank">Teevity</a> or <a href="http://www.cloudabillity.com" target="_blank">Cloudabililty</a>. These products had to ask users for the user/password of the administrator account attached to the AWS account in order to be able to parse the billing page. <a href="http://docs.amazonwebservices.com/AWSConsolidatedBilling/1.0/AWSConsolidatedBillingGuide.html" target="_blank">AWS Consolidated Billing Accounts</a> could be used to mitigate that risk but here again, we had to request access to the user/password of these accounts and the solution was not completely safe.</p>
<p>With this new features from Amazon IAM, <strong>problem solved !</strong> Companies using Cloud costs tracking solutions for AWS just need to create a special IAM Group with just the rights needed to access the billing page and use that user when declaring on account on these product.</p>

<p>figure class="tmblr-full" data-orig-height="218" data-orig-width="500"><img src="/assets/images/import/19003674956_1.png" data-orig-height="218" data-orig-width="500"/></figure></p>
<p><strong>Teevity CloudCost has full support for this new IAM feature right now</strong>.</p>
<p>You can sign-up for free right now and <a href="http://cloudcost.teevity.com" title="Teevity Cloudcost" target="_blank">start monitoring your cloud costs and get insight on how to optimize them</a>.</p>
<p><a href="http://cloudcost.teevity.com" target="_blank">http://cloudcost.teevity.com</a></p>
<p><a href="http://cloudcost.teevity.com" title="Teevity Cloudcost - Cloud costs tracking, analytics and management" target="_blank"><figure class="tmblr-full" data-orig-height="305" data-orig-width="500"><img src="/assets/images/import/19003674956_2.png" data-orig-height="305" data-orig-width="500"/></figure></a></p>
<p>Happy Cloud use.</p>
<p>Nicolas Fonrose<br/>@nfonrose </p>
<p>PS : Some &ldquo;cloud costs&rdquo; solutions you can find on the Web were not facing this confidentiality issue because they are not tracking &ldquo;real costs&rdquo; by accessing your AWS Billing Page but are rather *estimating* costs via the analysis of running instances. This has the disadvantage of only tracking EC2 costs which, from the feedback we get from our customers, can be only a part of the AWS costs (S3, CloudFront, SimpleDB, &hellip; usage can be very significant).</p>
        