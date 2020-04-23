---
title: Wide Open Games
subtitle: Let's roll some pure Javascript!
date: 2016-01-01
description: No frameworks, no SPAs, no nothing. Just a static-site generator and Javascript to create this subscription-based eZine I created and ran back in 2017.
featured_image: demo.jpg
accent_color: '#4C60E6'
gallery_images:
  - demo.jpg
#   - demo.jpg
#   - demo.jpg
---
## A membership site. A blog. And a games portal.

[Wide Open Games](https://wideopengames.com) was a lot of things, and it was all running on simple Javascript. Even most of the games themselves - complicated as some of them are - are built in JS so they can run smoothly in the browser.

Under the hood, the site was built using [Hugo](https://gohugo.io/) as a static site generator and used [aMember](https://www.amember.com/) to handle memberships. A little trickery to keep certain sections of the site free to the public and certain sections behind the paywall was all that was needed for the paywall to function successfully.

Production-wise, it was a lot to run solo, but I'm incredibly proud of the results. And very much glad to be doing other work as part of larger teams again :-)

{% include post-components/gallery.html
	columns = 2
	full_width = true
	images = "/images/demo.jpg,/images/demo.jpg,/images/demo.jpg,/images/demo.jpg,
	"
%}