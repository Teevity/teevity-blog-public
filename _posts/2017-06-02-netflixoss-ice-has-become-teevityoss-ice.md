---
layout: post
title:  "NetflixOSS ICE has become TeevityOSS ICE"
date:   2017-06-02 01:50:00 -0400
---
<p>We are very thrilled to announce that <a href="https://twitter.com/NetflixOSS/status/870475268166606851" target="_blank">NetflixOSS has moved the ICE project under the control of the Teevity GitHub organization</a>. Thank you NetflixOSS for trusting us with the continuation of this project !</p><figure data-orig-width="1172" data-orig-height="498" class="tmblr-full"><img src="../../media/161348125187_0.png" alt="image" data-orig-width="1172" data-orig-height="498"/></figure><p>More details on the reason for this transfer and what it means for the ICE community below. <br/></p>[[MORE]]<p><b>Why has the project been transfered to Teevity?</b></p><p>We have been in regular contact over the years with people at Netflix regarding ICE and people out there know we have:</p><ul><li>a ton on expertise on the ICE code (since a significant part of Teevity SaaS is based on our own private fork of ICE) and on AWS costs management and optimization in general. <br/></li><li>and a strong interest in keeping the open-source ICE active, which is good for the project on the long term,<br/></li></ul><p>Netflix having built another internal cost analytics solution (more in line with the rest of their Data Analytics pipelines and the size of their <a href="https://twitter.com/adrianco/status/763201371810123776" target="_blank">700 millions line billing file</a>), they were not accepting PRs anymore and were looking for an organization that would give the most changes for a good future to ICE.</p><p><br/></p><p><b>What it means for the community?</b><br/></p><p>The ICE project is coming back to life!!!  </p><p>As I’m writing this blog post, <a href="https://github.com/Teevity/ice/commits/integration" target="_blank">we’re already merging PRs and making changes</a> to ensure ICE can be started and used as-is, right from the repo. That’s the basics of what needs to be done.</p><p>And our next step it to put ICE in a position where it can receive contributions from others a lot more safely and easily:</p><ul><li>Addition of a basic test suite that will let people ensure they don’t break anything in the core computation logic when they make contributions (this is also going to simplify our work of accepting PRs, which means more PRs can get accepted)<br/><br/></li><li>Addition of a CloudFormation to start ICE on an AWS account and also to handle all the IAM rights related stuff (a Docker image is already maintained by <a href="https://github.com/jonbrouse" target="_blank">@jonbrouse</a> in the <a href="https://github.com/jonbrouse/docker-ice" target="_blank">docker-ice</a> project so no need to do anything more here).</li></ul><p><br/></p><p><b>What it means for our customers and users</b></p><p>Our users and customers can rest assured that we are more committed than ever to making the SaaS service continue to evolve and provide more and more value over time. This is obviously true not only for the components of our service which use ICE, but also for the other parts (Multi-cloud and muti-user dashboard, RI optimization and Resource Usage Analytics).</p><p><br/></p><p><b>And finally, what it means for Teevity as a company</b></p><p>Back in 2013, <a href="http://blog.teevity.com/post/58240593080/netflixoss-ice-as-a-service-by-teevity-in-two-flavors" target="_blank">when we announced that we were integrating the ICE technology into our already existing SaaS service</a>, we had no idea how much involvement we were going to put into ICE and how much benefit we would get from betting a significant technical part of Teevity on it, not only for AWS costs monitoring, but also for Microsoft Azure and Google GCP.</p><p>Four full years later, there is no doubt that it was a very good choice. And it’s one of the reasons why our SaaS service is so popular and used by small, large and very large organizations around the world.</p>
 