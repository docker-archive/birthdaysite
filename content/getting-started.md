+++
date = "2015-03-10T21:23:17-04:00"
title = "Getting Started Contributing"
linktitle = "Getting Started"
aliases = [ "overview" ]
weight = "5"

+++


# ![Docker Party](/images/docker-friends.png)

Contributing to the Docker project or to any open source project can be a
rewarding experience. You help yourself and you help the projects you work on.
You also help the countless number of other project participants.

Open source projects depend on a lot more than just code to be successful.
Proper documentation, testing, training, publicity, support and organization are
all critical.

# New to Docker? Before you arrive at an event...

If you have time, here are some things you can do get a head start before an event:

* Learn a little about what Docker is.
	* [Video review of Docker
	fundamentals](https://www.youtube.com/watch?v=zRLyovWi1gs) (9 minutes)
	* [Other good Docker resources](http://www.nkode.io/2014/08/24/valuable-docker-links.html)
* Test your knowledge.
	* [Basic Dockerfile test](https://docs.docker.com/userguide/level1/)
	* [Advanced Dockerfile test](https://docs.docker.com/userguide/level2/)
*  [Install Docker](http://docs.docker.com/introduction/#installation) on your machine.
* Get a free [GitHub account](https://github.com).
* Sure you want to contribute code or docs? Work through the [project
contributors guide](http://docs.docker.com/project/who-written-for/).


# Contributing Guides

When you are ready to start contributing, choose from the list below or the menu
in the upper right corner.

{{% contributingguide %}}


# Filters for experienced contributors

If you are an experienced Docker contributor, we have pre-filtered for open
issues in the `docker/docker` repository.  

* [Graphics](https://github.com/docker/docker/issues?q=is%3Aopen+is%3Aissue+label%3Akind%2Fgraphics+-label%3Astatus%2Fclaimed+-label%3Astatus%2Fassigned+no%3Aassignee)
* [Test](https://github.com/docker/docker/issues?q=is%3Aopen+is%3Aissue+label%3Akind%2Ftest+-label%3Astatus%2Fclaimed+-label%3Astatus%2Fassigned+no%3Aassignee)
* [Documentation](https://github.com/docker/docker/issues?q=is%3Aopen+is%3Aissue+label%3Akind%2Fwriting+-label%3Astatus%2Fclaimed+-label%3Astatus%2Fassigned+no%3Aassignee)
* [Questions](https://github.com/docker/docker/issues?q=is%3Aopen+is%3Aissue+label%3Akind%2Fquestion+-label%3Astatus%2Fclaimed+-label%3Astatus%2Fassigned+no%3Aassignee)
* [Bugs](https://github.com/docker/docker/issues?q=is%3Aopen+is%3Aissue+label%3Akind%2Fbug+-label%3Astatus%2Fclaimed+-label%3Astatus%2Fassigned+no%3Aassignee)
* [Features](https://github.com/docker/docker/issues?q=is%3Aopen+is%3Aissue+label%3Akind%2Ffeature+-label%3Astatus%2Fclaimed+-label%3Astatus%2Fassigned+no%3Aassignee)
* [Enhancements](https://github.com/docker/docker/issues?q=is%3Aopen+is%3Aissue+label%3Akind%2Fenhancement+-label%3Astatus%2Fclaimed+-label%3Astatus%2Fassigned+no%3Aassignee)

You might also want to check for open issues in our other Docker repositories:
<table class="tg">
		<col width="20%">
		<col width="80%">
		<tr>
			<td class="tg-031e"><a href="https://github.com/docker/machine/issues" >docker/machine</a></td>
			<td class="tg-031e">Software for the easy and quick creation of Docker hosts on your computer, on cloud providers, and inside your own data center.</td>
		</tr>
				<tr>
			<td class="tg-031e"><a href="https://github.com/docker/distribution/issues">docker/distribution</a></td>
			<td class="tg-031e">Registry implementation for storing and distributing
			docker images. Provides a secure tool chain for distributing content.</td>
		</tr>
	<tr>
			<td class="tg-031e"><a href="https://github.com/kitematic/kitematic/issues" >kitematic/kitematic</a></td>
			<td class="tg-031e">Kitematic is a simple application for managing Docker containers on Mac OS X.</td>
   </tr>
		<tr>
			<td class="tg-031e"><a href="https://github.com/docker/swarm/issues">docker/swarm</a></td>
			<td class="tg-031e">Native clustering for Docker; manage several Docker hosts as a single, virtual host.</td>
		</tr>
		<tr>
			<td class="tg-031e"><a href="https://github.com/docker/compose/issues" >docker/compose</a></td>
			<td class="tg-031e">Define and run complex applications using one or many interlinked containers.</td>
		</tr>
	</table>


# General resources and acknowledgements

In addition to this guide, we’ve found [GitHub's guide on contributing
to open source](https://guides.github.com/overviews/os-contributing/) to
be a helpful guide to contributing in general.

This document was inspired by the [jQuery contributor
guide](http://contribute.jquery.org/open-source/).
