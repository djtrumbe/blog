---
title: 'Drobo: Thin Provisioning'
author: David Trumbell
type: post
date: 2010-03-04T10:14:37+00:00
url: /2010/03/04/drobo-thin-provisioning/
dsq_thread_id:
  - 131590286
categories:
  - News
  - Tech
  - Uncategorized
tags:
  - Drobo
  - format
  - issues
  - News
  - Support
  - Thin Provisioning

---
If you know me, you know that I&#8217;m a huge proponent of Drobo.  As of late, the frustration level with Drobo is increasing and it may have edged away at this enthusiasm.

My most recent frustration came when I upgraded a drive in my Drobo to increase the usable space to more then 2TB.  After the Drobo finished updating all of its partitions, I was left with a partition that was labeled &#8216;unallocated&#8217; in the Drobo dashboard.  After searching the interwebs (which yielded **absolutely nothin****g** on Drobo&#8217;s site for &#8216;unallocated&#8217;) and posting on a couple of forums, I was led to this:

<a title="http://support.datarobotics.com/app/answers/detail/a_id/23/session/L3NpZC9LZFU0M3JWag%3D%3D/sno/0" href="http://support.datarobotics.com/app/answers/detail/a_id/23/session/L3NpZC9LZFU0M3JWag%3D%3D/sno/0" target="_blank">http://support.datarobotics.com/app/answers/detail/a_id/23/session/L3NpZC9LZFU0M3JWag%3D%3D/sno/0</a>

This is telling me that I&#8217;m stuck with adding partitions to my Drobo of maximum size 2TB because of a decision I made when I originally set it up, at which time I was not told how this setting would affect me as I add disk space.  Further, I think that Drobo&#8217;s claims of being both &#8220;simple&#8221; and &#8220;scalable&#8221; are misleading as this limitation is not spelled out up-front and if you don&#8217;t understand this, the affects of scaling can be considerably different then what is expected.

Now that I have have realized this, the only way to have 1 single partition again is to (in Drobo&#8217;s own words) &#8220;migrate the data onto another Drobo or storage device, reformat the original Drobo device to the volume size of your choice, and then move the data back.&#8221;  With 2TBs of data, not only is this a huge pain in the ass, I need to buy another drive in order to fit the entirety of my Drobo on a disk before reformatting.

I think this a huge failure on Drobo&#8217;s part that could be fixed one of 2 ways:

  1. Be explicit about how setting this soft limit is actually a hard limit on the amount of space that can be allocated to a volume.
  2. Drobo creates a tool to resize partitions to change storage space on a partition.

A tool in this situation would prove extremely handy and would prevent any confusion or problems when going over this thinly provisioned partition cap.

Any help here, Drobo?
