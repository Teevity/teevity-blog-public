---
layout: post
title:  "How-to : Use Teevity for Amazon cloud costs monitoring with a read-only IAM user"
date:   2012-03-16 4:27:00 -0400
---
<p>As <a href="http://blog.teevity.com/post/19003674956/no-more-confidentiality-issue-with-aws-cost-tracking-too" title="No more confidentiality issues with Amazon AWS cloud cost tracking solutions" target="_blank">we explained a few days ago</a>, Amazon has <a href="http://aws.typepad.com/aws/2012/03/new-iam-feature-control-activity-to-account-and-usage-pages.html" title="you can now create users with restricted rights that only have access to the Account Activity and Usage Report pages of the AWS portal" target="_blank">just announced</a> a new feature of their Amazon Identity and Access management system (aka Amazon IAM).</p>
<p>You can now create IAM users with restricted rights that <strong>only have access to the Account Activity and Usage Report pages of the AWS portal</strong>, the one that give you information about your current costs.</p>
<p>      <figure class="tmblr-full" data-orig-height="390" data-orig-width="500"><img alt="image" src="https://64.media.tumblr.com/32107b6e5ae75fc6da4d68e33e233d68/80361f3c838a1423-b4/s540x810/efba993516e1b3d1e458ff7fee8fb0029b6d0bbc.png" data-orig-height="390" data-orig-width="500"/></figure></p>
<p>These pages are the ones parsed by some AWS cloud costs monitoring solutions (the ones that do comprehensive and precise AWS cost reporting vs estimations), along-side other sources of information.<br/> </p>
<p><strong>Here is the 3 steps configuration process. It&rsquo;s only 2 minutes !</strong></p>
<ul><li><a href="http://blog.teevity.com/post/19400114920/aws-cloud-costs-monitoring-enabling-iam-billing-access" title="Enable IAM access to the Billing Page" target="_self">Step 1</a> - Enable access to the Billing page </li>
<li><a href="http://blog.teevity.com/post/19399771650/aws-cloud-costs-monitoring-iam-security-group" title="Creating an Amazon IAM account for Cloud costs monitoring with Teevity" target="_self">Step 2</a> - Create an IAM group dedicated to Cloud cost monitoring</li>
<li><a href="http://blog.teevity.com/post/19399945507/aws-cloud-costs-monitoring-iam-user" title="Creating an Amazon IAM account for Cloud costs monitoring with Teevity" target="_self">Step 3</a> - Create a new IAM user and add it to the group</li>
</ul><div><br/>You now have a &ldquo;user/password&rdquo; you can safely share with a third party AWS Cloud costs monitoring tool like <a href="http://cloudcost.teevity.com" title="Cloud cost monitoring and analytics for AWS and other Cloud services" target="_blank">Teevity Cloud costs analytics</a>.</div>
<div></div>
<div>And you&rsquo;re also pretty close to seeing these kind of charts on your Teevity dashboard.</div>
<div></div>
<div>        <figure class="tmblr-full" data-orig-height="361" data-orig-width="500"><img alt="image" src="https://64.media.tumblr.com/046ba71de58d3a5ebb1babb3a79de350/80361f3c838a1423-e7/s540x810/81749909df31d5d5aca8da1552c6512c757d5756.png" data-orig-height="361" data-orig-width="500"/></figure></div>
<div></div>
<div></div>
<div>And you can also use our graphical Widget on your desktop. </div>
<div>        <figure class="tmblr-full" data-orig-height="361" data-orig-width="500"><img alt="image" src="https://64.media.tumblr.com/0c2124eb41dec1d3d89ad27921af1b85/80361f3c838a1423-9f/s540x810/4dc41e46a9e5d639b968a0565aa65b48e9b733ce.png" data-orig-height="361" data-orig-width="500"/></figure></div>