---
layout: post
title:  "Feedback on using Netflix Ice by a select group of current Teevity users"
date:   2013-08-19 04:45:00 -0400
---
<p>We’ve put between the hands of a select group of our customers, a version of Netflix Ice running against their AWS account billing. The idea was to get functional feedback from “real users”.</p>
<p><strong>Context of the test</strong></p>
<p>These users had already been using Teevity cloud costs analytics for several month and we have a direct connection with them.</p>
<p>They did not auto-discover the product, we pushed it at them and gave access to it pre-configured for their AWS accounts, as a SaaS solution but isolated from our existing Teevity SaaS service. So they had in their hands a “very easy to get access to” version of Ice, with functional support provided by us.</p>
<p>This first test didn’t cover all aspects of Ice (AWS Reservations for instance where not covered by the test).</p>
<p><strong>Feedback 1 - Ice is very good for AWS cost debugging</strong></p>
<p>One thing which comes back from all the participants is that Ice is very good at “debugging” your cloud costs. The graphical view it provides enable a deep dive inside the cost and usage data that AWS dumps inside your Programmatic Billing bucket.</p>
<p>[[MORE]]</p>
<p><strong>Feedback 2 - Ice comes with a powerful “factor throughput” concept built-in</strong></p>
<p>Another point that some participants liked very much is that Ice has a “Factor throughput” feature that they would have liked to use. It’s not useable out of the box from the existing code base but it aims at:</p>
<ol><li>showing business metrics along side your cost timeline</li>
<li>factorizing these cloud costs y the business metric to show your ‘cloud cost per unit of [business metric]</li>
</ol>
<p><strong>Feedback 3 - Frustration for missing features, lack of data from Programmatic Billing or Cost Allocation Reports tagging</strong></p>
<p>The Ice code published on GitHub is quite incomplete (probably because before being published, the code had to be cleaned up from Netflix specifics) and so Ice, as it is on Github today, lacks several features that at least some companies need regarding cloud costs management</p>
<ul><li>easy cost sharing between people in the company,</li>
<li>historical analysis going before Programmatic Billing which is not retroactive,</li>
<li>cost classification beyond AWS tagging which are not retroactive either,</li>
<li>access protection,</li>
<li>and an API (if you want to integrate your costs in Excel for instance)</li>
</ul><p><em>AWS Programmatic Billing and Cost Allocation Report are not retroactive</em></p>
<p>The other thing that caused frustration is not related to Ice but to the way AWS Programmatic Billing and Cost Allocation Report work: they are not retro-active.</p>
<p>You cannot go further in your cost exploration than the initial date of activation of Programmatic Billing (which is why you should activate Programmatic Billing now !)</p>
<p>When Tags are used inside the Cost Allocation Report, they only apply from the time you apply them. You need to quickly get them right, because until you stabilize them for a full month, your cost reports will be hard to read.</p>
<p><strong>Feedback 4 - Some customers don’t love SaaS that much</strong></p>
<p>One of these customers, a Europe-based US army supplier who has strong confidentiality requirements, was very interested in this test because Ice “could run all inside [his] AWS account” (since it was started on his account with a CloudFormation) but was “as easy as SaaS”.</p>
<p><em>AWS Marketplace vs SaaS</em></p>
<p>That’s an interesting feedback! And I guess what is true for cost analytics will be true for many other solutions: the &ldquo;AWS Marketplace&rdquo; option will probably be a serious challenger to the &ldquo;SaaS option&rdquo; in the years to come, especially as the AWS Marketplace matures (and is able to launch full CloudFormations instead of just single EC2 instances).</p>
<p><strong>Conclusion</strong></p>
<p>When used as a Cloud cost debugging tool, the feedback on Ice has been very good.</p>
<p>Ice was thus seen as very complementary to Teevity’s existing feature set and a very good addition for deep “AWS cloud costs analysis”.</p>
<p>This is why, <a href="http://blog.teevity.com/post/58240593080/netflixoss-ice-as-a-service-by-teevity-in-two-flavors" target="_blank">as announced in our previous post</a>, Ice features will make their way into Teevity cloud costs analytics and will complement the existing features which make it easy to share cost data inside the company and to fetch historical cost and usage data. </p>

        