# stalkr
Gather data on an individual's public web-presence.

## the problem
Every time I sign up for a new service, I add the same pieces of data to my profile:
 - email address
 - website
 - full name
 - location
 - bio
 - gender
 - birthday
 - profile pic

Yet, all this information is already publically avaliable on my twitter, facebook, g+, last.fm, dribbble, VK, github, personal domain, deviantart, keybase, carrot profile, tumblr, instagram, vine, snapchat, gravatar, rap genius, oAuth, persona, and npm account. I'm a pretty "public" person, and I put this info out there because I want people to have access to it. It saves me a lot of boring introductions and makes it very easy for people to find me.

But if people can find me, then why can't web-services? Why must I "introduce" myself every time I sign up for a new site? 

## existing solutions
The way developers seem to approach this problem right now is integrate oAuth or some social network site and sign-in through that. A few sites that take this approach really get it right, but most sites either have a separate system for adding profile information (which doesn't pull data from the network that you signed in with), or have no integration with an existing identity provider at all.

And I don't _really_ blame them for not wanting to build around a centralized identity provider: doing so requires a lot of trust in that provider. I _can_ blame them for not working with distributed solutions like [Tent](https://tent.io/), but I suppose that will take some time to become stable and popular.

## the stalkr solution
Stalkr takes a different approach, because it's not an identity provider - it's an information provider. It's also not a centralized service that requires users to enter data (like gravatar). Instead, stalkr stalks the information that people have made public on various social accounts, and compares multiple possible online profiles. Data is then scraped from these profiles, compared, and information that is consistent accross a person's online identity is returned.

## ethics?
Well, first of all, it's called "stalkr" - that should kinda set the tone. Anyway, it might bother some people, but it only takes information that people have decided to make public so I'd consider it ethical.