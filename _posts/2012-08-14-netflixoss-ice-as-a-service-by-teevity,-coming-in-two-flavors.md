---
layout: post
title:  "NetflixOSS Ice as-a-Service by Teevity, coming in two flavors"
date:   2012-08-14 02:41:00 -0400
redirect_from:
  - /post/58240593080/netflixoss-ice-as-a-service-by-teevity-in-two-flavors
---
<p>We are pleased to announce that we will soon start offering two flavors of Netflix Ice in an &ldquo;as a service&rdquo; way:</p>
<ul><li>As an integrated part of our Teevity cloud costs analytics services for both the free and the premium SaaS Teevity offerings.</li>
<li>As a standalone service, through the AWS Marketplace. As simple as a SaaS solution, but without the cost-privacy concerns (since it runs on your own AWS account without any connection to us).</li>
</ul><p>It&rsquo;s the easiest way to run Ice and to get an always up-to-date version. If you are interested: <a href="http://ice.teevity.com/register/" title="Register for NetflixOSS Ice as a Service by Teevity" target="_blank">http://ice.teevity.com/register/</a>.</p>
<p>The code behind these two services is based off Teevity&rsquo;s fork of the Ice project, which can be found on Github.</p>
<p><figure class="tmblr-full" data-orig-height="467" data-orig-width="500"><img alt="image" src="/assets/images/import/58240593080_0.png" data-orig-height="467" data-orig-width="500"/></figure></p>
<p><figure class="tmblr-full" data-orig-height="360" data-orig-width="500"><img alt="image" src="/assets/images/import/58240593080_1.png" data-orig-height="360" data-orig-width="500"/></figure></p>
<p><strong>What is NetflixOSS Ice ?</strong></p>
<p>Last June, NetflixOSS released &ldquo;Ice&rdquo;, their <a href="https://github.com/Netflix/ice" title="NetflixOSS Ice" target="_blank">cloud spend and usage analytics </a><a href="https://github.com/Netflix/ice" title="NetflixOSS Ice" target="_blank">on GitHub</a> which they've been using internally for a while.</p>
<p><figure class="tmblr-full" data-orig-height="291" data-orig-width="500"><img alt="image" src="/assets/images/import/58240593080_2.png" data-orig-height="291" data-orig-width="500"/></figure></p>

<p>It&rsquo;s a tool that&rsquo;s mainly targetting DevOps and Dev folks, with a focus on:</p>
<ul><li>Getting a detailed understanding of how much is spent, and on which services, on your AWS account(s), all through charts and filters</li>
<li>Giving feedback to teams on how much they have, or their project have, spent over a giving period of time</li>
</ul><p>The way Netflix has been using this tool was presented at AWS re:Invent 2012 back in November by Watson Coburn and his colleagues. But the exact feature set of the version of Ice was unknown at that time.</p>
<p><strong>How does Ice fit in the Cloud cost analytics landscape ?</strong></p>
<p>Ice is somewhat different from the existing cloud cost monitoring solutions in that:</p>
<ul><li>It&rsquo;s focusing on a purely graphical analysis of cost and usage data</li>
<li>It doesn&rsquo;t provide any cost optimizations recommendations</li>
<li>it&rsquo;s purely based off the output of AWS billing engine and is not doing any cost simulation based on usage analysis.</li>
</ul><p>And it goes further than the existing players in one interesting area: </p>
<ul><li>it offers the basis of what is needed to compute a &ldquo;cost per unit of business&rdquo; through a notion called &ldquo;throughput&rdquo;</li>
</ul><p>It also has many extension points that Netflix is probably taking advantage off on its internal version and which can be used to extend the product.</p>
<p>After a careful analysis of the product, we think it has the potential to become a standard in detailed cloud costs analytics targeted at technical teams. So we have decided to invest and build on it. </p>
<p><strong>Very complementary to Teevity existing service</strong></p>
<p>Ice is very complementary to Teevity&rsquo;s existing service, which is mainly targeted at managers.</p>
<p>It makes a very natural extension to our existing feature set. And our goal has always been to target both the technical and the financial world and to create a cost related communication channel between them.</p>
<p>So expect to see more and more integration of Ice features inside the Teevity cloud cost analytics service in the months to come.</p>
<p><strong>The easiest way to run Ice</strong></p>
<p>Since 2012 when we&rsquo;ve started building Teevity, we&rsquo;ve heard customers who were concerned about privacy issue related to their cloud spending. And they were not keen on using a SaaS service to track and optimize their cloud costs.</p>
<p>In response to that, we have decided to start offering a &ldquo;run in on your own AWS account&rdquo; version of Ice that is a easy to use as a SaaS version.</p>
<p>If you want to start using Ice today (for just a few hours or in an always-on mode), without having to go through many technical steps, the easiest way to run it is here : <a href="http://ice.teevity.com/register/" target="_blank">http://ice.teevity.com/register/</a></p>
 