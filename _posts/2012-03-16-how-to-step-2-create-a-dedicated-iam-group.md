---
layout: post
title:  "How-to : Step 2 - Create a dedicated IAM group"
date:   2012-03-16 04:20:00 -0400
---
<p>This post describes the second step needed to <a href="http://blog.teevity.com/post/19339445622/amazon-cloud-costs-monitoring-with-teevity-cloudcost" target="_blank">configure an Amazon IAM account for use with Teevity AWS Cloud costs monitoring</a> solution.</p>
<ul><li><a href="http://blog.teevity.com/post/19400114920/aws-cloud-costs-monitoring-enabling-iam-billing-access" title="Teevity - Enable access to the AWS Billing page" target="_self">Step 1 - Enable access to the Billing page</a> </li>
<li><strong>Step 2 -</strong> <strong>Create the IAM group with the appropriate rights</strong></li>
<li><a href="http://blog.teevity.com/post/19399945507/aws-cloud-costs-monitoring-iam-user" title="Teevity - Create the AWS IAM user" target="_self">Step 3 - Create a new IAM user and add it to the group</a></li>
</ul><p><br/><strong>A/ Create the IAM group</strong></p>
<p>You can do that using the <a href="https://console.aws.amazon.com/iam/home" title="IAM tab of the Amazon AWS Console" target="_blank">IAM tab in the Amazon AWS Console</a>.  </p>
<p><figure class="tmblr-full" data-orig-height="351" data-orig-width="500"><img alt="image" src="https://64.media.tumblr.com/586df8fb3b302adb4c0ae6f6e1a3d4ec/8c96ca4b34894b6d-3a/s540x810/00b56b1d8cce28e8c98d5e6dfa66df083153aed7.png" data-orig-height="351" data-orig-width="500"/></figure></p>
<p><br/><strong>B/ Give the group a name like &ldquo;CloudCostMonitoringTools&rdquo;.</strong></p>
<p><figure class="tmblr-full" data-orig-height="218" data-orig-width="500"><img alt="image" src="https://64.media.tumblr.com/01eb0b948a187a2fd4f43caab8292086/8c96ca4b34894b6d-f8/s540x810/c99c1d1911858ba3cead9347b55bf8743cb7757f.png" data-orig-height="218" data-orig-width="500"/></figure></p>
<p><br/><strong>C/ Give the group the &ldquo;read-only rights&rdquo; needed by Teevity</strong></p>
<p>The easiest way to add the required authorizations is to use the Custom Policy wizard and to copy and paste the following policy.</p>
<p><figure class="tmblr-full" data-orig-height="335" data-orig-width="500"><img alt="image" src="https://64.media.tumblr.com/9dbdf6811c9356f5cf451aff18d62676/8c96ca4b34894b6d-cc/s540x810/57bb6b17e74eacbb919a2b4de195c59e62d26a20.png" data-orig-height="335" data-orig-width="500"/></figure></p>
<p><br/>Call the policy something like &ldquo;CloudCostMonitoringToolsPolicy&rdquo;</p>
<p><figure class="tmblr-full" data-orig-height="362" data-orig-width="500"><img alt="image" src="https://64.media.tumblr.com/0cbd149e186addd2473a6cbb247c0d7a/8c96ca4b34894b6d-ee/s540x810/4ed11c3be88743652acb00e55c72362bd2793e58.png" data-orig-height="362" data-orig-width="500"/></figure></p>
<p>And copy and paste into the &ldquo;Policy Document field&rdquo; the content of this read-only Access Policy you can find in this gist :</p>
<p>       <a href="https://gist.github.com/nfonrose/6038928" title="Teevity IAM Policy" target="_blank"><strong><a href="https://gist.github.com/nfonrose/6038928" target="_blank">https://gist.github.com/nfonrose/6038928</a></strong></a></p>
<p>Take your time and feel free to review it. It is a subset of the &ldquo;Read-only&rdquo; Access Policy provided by AWS to which we have added the ViewBilling and UsageReports rights.</p>
<p>You can see <a href="https://gist.github.com/nfonrose/6038928#comment-1187986" title="All the IAM rights Teevity is *not requiring*" target="_blank">here</a>, all the elements that we have removed from the default Read-only access policy provided by AWS (because they are not needed to provide the Teevity service to you) to create our describe-only policy.</p>

<p><strong>D/ And you&rsquo;re done with the creation of the IAM Group</strong></p>
<p><figure class="tmblr-full" data-orig-height="313" data-orig-width="500"><img alt="image" src="https://64.media.tumblr.com/7c83bbcafea3c0765c7b1fbf4e9d4557/8c96ca4b34894b6d-81/s540x810/907a8698696c6cb23fdcc8265058557bb594845f.png" data-orig-height="313" data-orig-width="500"/></figure></p>
<div></div>
<p><strong>E/ Now the last step : creating the IAM User and place it in the group you&rsquo;ve just created</strong></p>
<div>You can see here <a href="http://blog.teevity.com/post/19399945507/aws-cloud-costs-monitoring-iam-user" title="how to do that last step" target="_self">how to do that last step</a>.</div>