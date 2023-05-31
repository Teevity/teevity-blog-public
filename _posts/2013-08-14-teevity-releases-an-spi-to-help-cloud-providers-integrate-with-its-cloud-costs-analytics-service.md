---
layout: post
title:  "Teevity releases an SPI to help Cloud providers integrate with its cloud costs analytics service"
date:   2013-08-14 00:22:00 -0400
---
 <p>We are very excited to announce the release of our SPI (service provider interface) used to integrate cost and usage data from Cloud and SaaS with our service.</p>
<p>We have been using it internally to integrate various IaaS, PaaS and SaaS services already. Considering how different the services and cost structure of the various Cloud providers are, it took us some time to get things right. Especilally when you want to go deeper than just &ldquo;how much has been spent since the beginning of the month&rdquo;.</p>
<p>But here we are ! And it&rsquo;s now time to release it more formally to help onboard more cloud providers and enable their customers to get a deep understanding of how they spend on the cloud. </p>
<p><strong>What&rsquo;s inside ?</strong></p>
<p>The Teevity SPI is an SDK for Cloud providers. It comes in the form of :</p>
<ul><li>REST services,</li>
<li>and File formats,</li>
</ul><p>which formalize the way cost and usage data have to be pushed to us in order to be used by our analytics engine.</p>
<p><strong>Want to know more and integrate with us ?</strong></p>
<p>Keep reading if you want to know more ! And contact us at founders@teevity.com if you want to integrate with us.</p>
<p>[[MORE]]</p>
<p><strong>How do we model cost and usage data for all the cloud providers ?</strong></p>
<p>It accomodates cost and usage data of various nature:</p>
<ul><li>historical and current cost and usage data</li>
<li>different time-steps (monthly, daily, hourly, by-the-min and custom)</li>
<li>different sorts of billing items (to support all the Cloud/SaaS providers with their various offering - classical services, reserved instances, support, &hellip;)</li>
<li>different data qualities (accurate, estimate, interpolated, &hellip;)</li>
<li>cost-tagging for cost allocation</li>
</ul><p>The SPI also offers a way for providers to push non directly cost related information:</p>
<ul><li>Declare the list of Cloud accounts a user has</li>
<li>Declare the list of resources a user has allocated</li>
<li>Declare events that have happened on the user&rsquo;s account (resources started/stopped, special services bought)</li>
<li>Declare events that are happening on the cloud providers side (public prices change, &hellip;)</li>
</ul><p><strong>How can Cloud and SaaS providers leverage the Teevity SPI ?</strong></p>
<p>There are two ways to use this SPI.</p>
<ul><li>Either remotely, through the REST services we expose. Cloud providers can remotely push cost and usage data to us.<br/><br/>You can either make many small calls distributed in time (continuous push of data) or generate large data blocks and push them to us (generaly a few times per day or at a lower rate).  </li>
</ul><ul><li>Or by creating code that will run on our premise, connect remotely to your systems, and use the local version of our SPI&rsquo;s interfaces.</li>
</ul><p><strong>Get in touch with us !</strong></p>
<p>In either case, get in touch with us to know more. You can email us at founders@teevity.com.</p>