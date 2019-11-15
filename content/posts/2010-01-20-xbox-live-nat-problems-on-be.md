---
title: XBox Live NAT problems on BE
author: David Trumbell
type: post
date: 2010-01-20T22:19:59+00:00
url: /2010/01/20/xbox-live-nat-problems-on-be/
dsq_thread_id:
  - 144869943
categories:
  - Tech
tags:
  - BE
  - Speedtouch
  - XBox
  - XBox Live

---
For quite a while I've struggled with a 'strict' NAT when connecting to XBox Live.  I've finally fixed this problem.  Apparently, <a title="https://www.bethere.co.uk/" href="https://www.bethere.co.uk/" target="_blank">BE</a> locks down their Speedtouch routers which creates this problem.  The fix is simple:

<a title="http://www.beusergroup.co.uk/technotes/index.php/Xbox_Live" href="http://www.beusergroup.co.uk/technotes/index.php/Xbox_Live" target="_blank">http://www.beusergroup.co.uk/technotes/index.php/Xbox_Live</a>

On top of this, you may need to forward some ports on your router:

<a title="http://portforward.com/english/routers/port_forwarding/Thomson-Alcatel/SpeedTouch585/Xbox_Live_360.htm" href="http://portforward.com/english/routers/port_forwarding/Thomson-Alcatel/SpeedTouch585/Xbox_Live_360.htm" target="_blank">http://portforward.com/english/routers/port_forwarding/Thomson-Alcatel/SpeedTouch585/Xbox_Live_360.htm</a>

When I get some time, I will try to confirm the need for mapping ports.
