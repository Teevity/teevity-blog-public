---
layout: post
title:  "How-to : Step 3 - Create the Amazon IAM user dedicated to Teevity"
date:   2012-03-16 04:23:00 -0400
---
<p>This post describes the third and last step need to <a href="http://blog.teevity.com/post/19339445622/amazon-cloud-costs-monitoring-with-teevity-cloudcost" target="_blank">configure an Amazon IAM account for use with Teevity Cloud costs analytics</a> solutions.</p>
<ul><li><a href="http://blog.teevity.com/post/19400114920/aws-cloud-costs-monitoring-enabling-iam-billing-access" title="Teevity - Creating the IAM group" target="_self">Step 1 - Enable access to the Billing page </a></li>
<li><a href="http://blog.teevity.com/post/19399771650/aws-cloud-costs-monitoring-iam-security-group" title="Teevity - Creating a new IAM group" target="_self">Step 2 - Create the IAM group</a></li>
<li><strong>Step 3 - Create a new IAM user and add it to the group</strong></li>
</ul><p>[[MORE]]<br/><br/></p>
<div>
<ul><li><strong>A - Create the IAM user</strong></li>
</ul></div>
<div>This can be done using the <a href="https://console.aws.amazon.com/iam/home" title="IAM tab of the Amazon AWS Console" target="_blank">IAM tab in the Amazon AWS Console</a>.<br/> </div>
<p><figure class="tmblr-full" data-orig-height="330" data-orig-width="500"><img alt="image" src="https://64.media.tumblr.com/9338f8a8952764af1a8cdd465aa883d0/b316eb8ee4e4c386-97/s540x810/bcf4e49289d7ae083bdfadd5fd9fb9f138e2022a.png" data-orig-height="330" data-orig-width="500"/></figure></p>
<div></div>
<div>
<ul><li><strong>B - Let&rsquo;s call the IAM user &ldquo;teevity.cloudcostanalytics&rdquo;</strong></li>
</ul></div>
<div>Keep the &ldquo;Generate an access key for each User&rdquo; option selected. These credentials will also be needed by Teevity to analyze the way you use resources in order to provide you with cost optimizations.<br/> </div>
<div>
<ul><li><strong>C - Save the user&rsquo;s AccessKey and SecretKey</strong></li>
</ul></div>
<div>They are only provided once by Amazon. So you need to store them somewhere secure. If you don&rsquo;t know where, may be you can have a look at solutions like <a href="http://www.keepassx.org/" title='A possible "secure store" for your AWS credentials' target="_blank">KeePassX</a>.<br/> </div>
<div><figure class="tmblr-full" data-orig-height="241" data-orig-width="500"><img alt="image" src="https://64.media.tumblr.com/05802237b858ad581310e388fdd55da3/b316eb8ee4e4c386-a3/s540x810/41f42248c6b252b8afcbaa8616a028ad5b4035a9.png" data-orig-height="241" data-orig-width="500"/></figure><br/><br/></div>
<div>
<ul><li><strong>D - Assign a password to this new user</strong></li>
</ul></div>
<div>The user you just created doesn&rsquo;t have a password.<br/> </div>
<div></div>
<div><figure class="tmblr-full" data-orig-height="358" data-orig-width="500"><img alt="image" src="https://64.media.tumblr.com/7ac0ddfa854de62fbbe80e48ca9483de/b316eb8ee4e4c386-d9/s540x810/7289cdc67cd90f4a22b22c394c05b7e29121788a.png" data-orig-height="358" data-orig-width="500"/></figure><br/><br/></div>
<div></div>
<div>You can assign one using the &ldquo;Manage Password&rdquo;.<br/><br/></div>
<div></div>
<div><figure class="tmblr-full" data-orig-height="157" data-orig-width="500"><img alt="image" src="https://64.media.tumblr.com/cac5eb067659fbf925fb58e1ffd4e353/b316eb8ee4e4c386-87/s540x810/6336dd38022c4eb317c1d5233491cb083af886ad.png" data-orig-height="157" data-orig-width="500"/></figure><br/><br/></div>
<div>
<ul><li><strong>E - Assign the user to the CloudCostMonitoringTools group<br/> </strong></li>
</ul></div>
<div></div>
<div><figure class="tmblr-full" data-orig-height="179" data-orig-width="500"><img alt="image" src="https://64.media.tumblr.com/2b106a4ff6ad5b9e003fb6084a59a48d/b316eb8ee4e4c386-1e/s540x810/623715e4acda9b0321b1db675100e39049f26bde.png" data-orig-height="179" data-orig-width="500"/></figure><br/><br/></div>
<div></div>
<div>Choose the CloudCostMonitoringTools group <br/> </div>
<div></div>
<div><figure class="tmblr-full" data-orig-height="207" data-orig-width="500"><img alt="image" src="https://64.media.tumblr.com/946bc704398254f3e75e008468059578/b316eb8ee4e4c386-78/s540x810/479dd0d5e3d85e8c6c5663531aad1a7dcf50ecf9.png" data-orig-height="207" data-orig-width="500"/></figure></div>
<div><br/><br/></div>
<div></div>
<div>That&rsquo;s it. Your IAM user has been created. Just one last step and your are done !</div>