---
layout: post
title:  "How-to : Step 2 - Create a dedicated IAM group"
date:   2012-03-16 04:20:00 -0400
---
<p>This post describes the second step needed to <a href="{% post_url 2012-03-16-how-to-use-teevity-for-amazon-cloud-costs-monitoring-with-a-read-only-iam-user %}" target="_blank">configure an Amazon IAM account for use with Teevity AWS Cloud costs monitoring</a> solution.</p>
<ul><li><a href="{% post_url 2012-03-16-how-to-step-1-enabling-access-to-the-billing-page %}" title="Enable IAM access to the Billing Page" target="_self">Step 1</a> - Enable access to the Billing page </li>
<li>Step 2 - Create an IAM group dedicated to Cloud cost monitoring</li>
<li><a href="{% post_url 2012-03-16-how-to-step-3-create-the-amazon-iam-user-dedicated-to-teevity %}" title="Creating an Amazon IAM account for Cloud costs monitoring with Teevity" target="_self">Step 3</a> - Create a new IAM user and add it to the group</li>
</ul><p><br/><strong>A/ Create the IAM group</strong></p>
<p>You can do that using the <a href="https://console.aws.amazon.com/iam/home" title="IAM tab of the Amazon AWS Console" target="_blank">IAM tab in the Amazon AWS Console</a>.  </p>
<p><figure class="tmblr-full" data-orig-height="351" data-orig-width="500"><img alt="image" src="/assets/images/import/19399771650_0.png" data-orig-height="351" data-orig-width="500"/></figure></p>
<p><br/><strong>B/ Give the group a name like &ldquo;CloudCostMonitoringTools&rdquo;.</strong></p>
<p><figure class="tmblr-full" data-orig-height="218" data-orig-width="500"><img alt="image" src="/assets/images/import/19399771650_1.png" data-orig-height="218" data-orig-width="500"/></figure></p>
<p><br/><strong>C/ Give the group the &ldquo;read-only rights&rdquo; needed by Teevity</strong></p>
<p>The easiest way to add the required authorizations is to use the Custom Policy wizard and to copy and paste the following policy.</p>
<p><figure class="tmblr-full" data-orig-height="335" data-orig-width="500"><img alt="image" src="/assets/images/import/19399771650_2.png" data-orig-height="335" data-orig-width="500"/></figure></p>
<p><br/>Call the policy something like &ldquo;CloudCostMonitoringToolsPolicy&rdquo;</p>
<p><figure class="tmblr-full" data-orig-height="362" data-orig-width="500"><img alt="image" src="/assets/images/import/19399771650_3.png" data-orig-height="362" data-orig-width="500"/></figure></p>
<p>And copy and paste into the &ldquo;Policy Document field&rdquo; the content of this read-only Access Policy you can find in this gist :</p>
<p>       <a href="https://gist.github.com/nfonrose/6038928" title="Teevity IAM Policy" target="_blank"><strong><a href="https://gist.github.com/nfonrose/6038928" target="_blank">https://gist.github.com/nfonrose/6038928</a></strong></a></p>
<p>Take your time and feel free to review it. It is a subset of the &ldquo;Read-only&rdquo; Access Policy provided by AWS to which we have added the ViewBilling and UsageReports rights.</p>
<p>You can see <a href="https://gist.github.com/nfonrose/6038928#comment-1187986" title="All the IAM rights Teevity is *not requiring*" target="_blank">here</a>, all the elements that we have removed from the default Read-only access policy provided by AWS (because they are not needed to provide the Teevity service to you) to create our describe-only policy.</p>

<p><strong>D/ And you&rsquo;re done with the creation of the IAM Group</strong></p>
<p><figure class="tmblr-full" data-orig-height="313" data-orig-width="500"><img alt="image" src="/assets/images/import/19399771650_4.png" data-orig-height="313" data-orig-width="500"/></figure></p>
<div></div>
<p><strong>E/ Now the last step : creating the IAM User and place it in the group you&rsquo;ve just created</strong></p>
<div>You can see here <a href="{% post_url 2012-03-16-how-to-step-3-create-the-amazon-iam-user-dedicated-to-teevity %}" title="how to do that last step" target="_self">how to do that last step</a>.</div>