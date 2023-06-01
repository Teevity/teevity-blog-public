---
layout: post
title:  "How-to : Step 3 - Create the Amazon IAM user dedicated to Teevity"
date:   2012-03-16 04:23:00 -0400
redirect_from:
  - /post/19399945507/aws-cloud-costs-monitoring-iam-user
---
<p>This post describes the third and last step need to <a href="{% post_url 2012-03-16-how-to-use-teevity-for-amazon-cloud-costs-monitoring-with-a-read-only-iam-user %}" target="_blank">configure an Amazon IAM account for use with Teevity Cloud costs analytics</a> solutions.</p>
<ul><li><a href="{% post_url 2012-03-16-how-to-step-1-enabling-access-to-the-billing-page %}" title="Enable IAM access to the Billing Page" target="_self">Step 1</a> - Enable access to the Billing page </li>
<li><a href="{% post_url 2012-03-16-how-to-step-2-create-a-dedicated-iam-group %}" title="Creating an Amazon IAM account for Cloud costs monitoring with Teevity" target="_self">Step 2</a> - Create an IAM group dedicated to Cloud cost monitoring</li>
<li>Step 3 - Create a new IAM user and add it to the group</li>
</ul>
<div>
<ul><li><strong>A - Create the IAM user</strong></li>
</ul></div>
<div>This can be done using the <a href="https://console.aws.amazon.com/iam/home" title="IAM tab of the Amazon AWS Console" target="_blank">IAM tab in the Amazon AWS Console</a>.<br/> </div>
<p><figure class="tmblr-full" data-orig-height="330" data-orig-width="500"><img alt="image" src="/assets/images/import/19399945507_0.png" data-orig-height="330" data-orig-width="500"/></figure></p>
<div></div>
<div>
<ul><li><strong>B - Let&rsquo;s call the IAM user &ldquo;teevity.cloudcostanalytics&rdquo;</strong></li>
</ul></div>
<div>Keep the &ldquo;Generate an access key for each User&rdquo; option selected. These credentials will also be needed by Teevity to analyze the way you use resources in order to provide you with cost optimizations.<br/> </div>
<div>
<ul><li><strong>C - Save the user&rsquo;s AccessKey and SecretKey</strong></li>
</ul></div>
<div>They are only provided once by Amazon. So you need to store them somewhere secure. If you don&rsquo;t know where, may be you can have a look at solutions like <a href="http://www.keepassx.org/" title='A possible "secure store" for your AWS credentials' target="_blank">KeePassX</a>.<br/> </div>
<div><figure class="tmblr-full" data-orig-height="241" data-orig-width="500"><img alt="image" src="/assets/images/import/19399945507_1.png" data-orig-height="241" data-orig-width="500"/></figure><br/><br/></div>
<div>
<ul><li><strong>D - Assign a password to this new user</strong></li>
</ul></div>
<div>The user you just created doesn&rsquo;t have a password.<br/> </div>
<div></div>
<div><figure class="tmblr-full" data-orig-height="358" data-orig-width="500"><img alt="image" src="/assets/images/import/19399945507_2.png" data-orig-height="358" data-orig-width="500"/></figure><br/><br/></div>
<div></div>
<div>You can assign one using the &ldquo;Manage Password&rdquo;.<br/><br/></div>
<div></div>
<div><figure class="tmblr-full" data-orig-height="157" data-orig-width="500"><img alt="image" src="/assets/images/import/19399945507_3.png" data-orig-height="157" data-orig-width="500"/></figure><br/><br/></div>
<div>
<ul><li><strong>E - Assign the user to the CloudCostMonitoringTools group<br/> </strong></li>
</ul></div>
<div></div>
<div><figure class="tmblr-full" data-orig-height="179" data-orig-width="500"><img alt="image" src="/assets/images/import/19399945507_4.png" data-orig-height="179" data-orig-width="500"/></figure><br/><br/></div>
<div></div>
<div>Choose the CloudCostMonitoringTools group <br/> </div>
<div></div>
<div><figure class="tmblr-full" data-orig-height="207" data-orig-width="500"><img alt="image" src="/assets/images/import/19399945507_5.png" data-orig-height="207" data-orig-width="500"/></figure></div>
<div><br/><br/></div>
<div></div>
<div>That&rsquo;s it. Your IAM user has been created. Just one last step and your are done !</div>