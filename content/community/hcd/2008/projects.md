+++
type = "article"
title = "Finalists"
date = "2009-09-11T05:26:37.000Z"
tags = []
+++

<p>This page shows the projects selected by the community to participate in the Haiku Code Drive 2008. The projects are listed in the order that the community ranked them through the Haiku Code Drive 2008 poll</a>.</p>

<a name="bfs"></a>
<h3 class="icon-person-medium">Salvatore Benedetto</h3>
<ul>
<p><strong>Project:</strong> BFS stress-testing, UDF port to new FS Haiku API</p>
<p><strong>Mentor:</strong> Axel Dörfler</p>

<p>The aim of this project is quite different from the others. Instead of proposing to add a new feature, I'd like to work on something R1 related, like making sure that BFS is *STABLE*. Since I'm almost done with Dominic's book about BFS, what I have in mind is to run some tests to stress all the aspects of Haiku's BFS implementation and see where it fails in order to fix the problem and bring the file system a step closer to being stable. To achieve this, I propose to do the following:</p>

<ul>
<li>Porting <a href="http://www.coker.com.au/bonnie++/">Bonnie++</a> to Haiku, which is a benchmark suite that is aimed at performing a number of simple tests of hard drive and file system performance.</li>
<li>The porting would require to implement XSI semaphore and IPC API, that is <a href="https://dev.haiku-os.org/ticket/1980">ticket 1980</a></li>
<li>Once this is all done and working, bug hunting would be next along with fixes.</li>
</ul>

<p>Additionally, as a second milestone for my proposal, I also intend to port UDF support to the new FS Haiku API, and if I have some time left, I would like to look also into adding write support to UDF.</p>

</ul>

<a name="cups"></a>
<h3 class="icon-person-medium">Jovan Ivankovic</h3>
<ul>
<p><strong>Project:</strong> CUPS port</p>
<p><strong>Mentor:</strong> Michael Pfeiffer</p>
<p>I'm interested in helping bring wider printing support to Haiku. I know very little about Printing kit, but I'm reading through the BeBook and existing code in Haiku source tree. I do not know at which stage the current port is(I know there is <a href="http://www.zeta-os.com/cms/download.php?view.19">Zeta port of Cups here</a>), so I guess it would be even easier to port it to Haiku because of greater posix compliance. I'm also aware of Ithamar Adema's work and his approach on the matter (reusing foomatic database and create Haiku native frontends for existing GhostScript backends) and would like to continue his work.</p>
</ul>

<a name="icmp"></a>
<h3 class="icon-person-medium">Yin Qiu</h3>
<ul>
<p><strong>Project:</strong> ICMP error handling and propagation</p>
<p><strong>Mentor:</strong> Philippe Houdoin</p>
<p>ICMP is a necessary part of the IP protocol family. I will refer to other open source implementations to add ICMP error handling to the Haiku network stack. RFC 792 will be my reference for ICMP segment structure and other implementation details. ICMP messages are usually handled in the OS network stack as a special case. To do so I will study the ICMP message types and ICMP error codes in detail. The error handling mechanism will be implemented with a neat interface. After implementation, I will verify the stack with a Haiku virtual machine and a Linux or Windows host machine.</p>
</ul>

<a name="dv"></a>
<h3 class="icon-person-medium">JiSheng Zhang</h3>
<ul>
<p><strong>Project:</strong> Write a DV media node</p>
<p><strong>Mentor:</strong> Rene Gollent</p>

<p>As is known to all, a media "node" in Haiku's Media Kit system is a special object that processes buffers of media data. They can be loaded from Add-on modules by the Media Server.</p>

<p>This project will make it easy for Application Programmers to access DV hardware over firewire using the powerful Media Kit APIs without knowing details of firewire protocol and without accessing the somewhat complicated raw interface in /dev.</p>

<p>There are three parts will be implemented. First, a FireWireMediaAddOn class (derived from BMediaAddOn) is used to tell the Media Server the types of nodes it supports and create them when told to do so by the server. Second, A FireWireMediaNode class derived from BBufferProducer, BufferConsumer, BMediaEventLooper which is the major part of this project. Finally, one or more abstract classes which supply convenient methods accessing the raw interface exported by the Firewire stack.</p>
</ul>
