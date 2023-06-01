---
layout: post
title:  "How-to : Use Teevity for Amazon cloud costs monitoring with a read-only IAM user"
date:   2012-03-16 4:27:00 -0400
redirect_from:
  - /post/19339445622/amazon-cloud-costs-monitoring-with-teevity-cloudcost
---
<p>As <a href="{% post_url 2012-03-09-no-more-confidentiality-issues-with-amazon-aws-cloud-cost-tracking-solutions %}" title="No more confidentiality issues with Amazon AWS cloud cost tracking solutions" target="_blank">we explained a few days ago</a>, Amazon has <a href="http://aws.typepad.com/aws/2012/03/new-iam-feature-control-activity-to-account-and-usage-pages.html" title="you can now create users with restricted rights that only have access to the Account Activity and Usage Report pages of the AWS portal" target="_blank">just announced</a> a new feature of their Amazon Identity and Access management system (aka Amazon IAM).</p>
<p>You can now create IAM users with restricted rights that <strong>only have access to the Account Activity and Usage Report pages of the AWS portal</strong>, the one that give you information about your current costs.</p>
<p>      <figure class="tmblr-full" data-orig-height="390" data-orig-width="500"><img alt="image" src="/assets/images/import/19339445622_0.png" data-orig-height="390" data-orig-width="500"/></figure></p>
<p>These pages are the ones parsed by some AWS cloud costs monitoring solutions (the ones that do comprehensive and precise AWS cost reporting vs estimations), along-side other sources of information.<br/> </p>
<p><strong>Here is the 3 steps configuration process. It&rsquo;s only 2 minutes !</strong></p>
<ul><li><a href="{% post_url 2012-03-16-how-to-step-1-enabling-access-to-the-billing-page %}" title="Enable IAM access to the Billing Page" target="_self">Step 1</a> - Enable access to the Billing page </li>
<li><a href="{% post_url 2012-03-16-how-to-step-2-create-a-dedicated-iam-group %}" title="Creating an Amazon IAM account for Cloud costs monitoring with Teevity" target="_self">Step 2</a> - Create an IAM group dedicated to Cloud cost monitoring</li>
<li><a href="{% post_url 2012-03-16-how-to-step-3-create-the-amazon-iam-user-dedicated-to-teevity %}" title="Creating an Amazon IAM account for Cloud costs monitoring with Teevity" target="_self">Step 3</a> - Create a new IAM user and add it to the group</li>
</ul><div><br/>You now have a &ldquo;user/password&rdquo; you can safely share with a third party AWS Cloud costs monitoring tool like <a href="http://cloudcost.teevity.com" title="Cloud cost monitoring and analytics for AWS and other Cloud services" target="_blank">Teevity Cloud costs analytics</a>.</div>
<div></div>
<div>And you&rsquo;re also pretty close to seeing these kind of charts on your Teevity dashboard.</div>
<div></div>
<div>        <figure class="tmblr-full" data-orig-height="361" data-orig-width="500"><img alt="image" src="/assets/images/import/19339445622_1.png" data-orig-height="361" data-orig-width="500"/></figure></div>
<div></div>
<div></div>
<div>And you can also use our graphical Widget on your desktop. </div>
<div>        <figure class="tmblr-full" data-orig-height="361" data-orig-width="500"><img alt="image" src="/assets/images/import/19339445622_2.png" data-orig-height="361" data-orig-width="500"/></figure></div>