# Improving Dependencies for Everyone

Speaker: Aaron Schlesinger [@arschles](https://twitter.com/arschles)

## Intro

This was a talk about the Athens project, which is a proxy for Go modules. We could run an instance of Athens at our organisation that would allow us to download Go modules when sites such as GitHub go offline. You could even run a local instance to allow you to download Go modules when working offline.
https://docs.gomods.io/
Link to the demo Aaron showed - https://github.com/aarons-talks/2019-08-23-GopherCon-UK


https://www.youtube.com/watch?v=WDbbIS7m9bU&list=PL2ntRZ1ySWBdDyspRTNBIKES1Y-P__59_&index=18&t=0s

Notes: Go 1.11 was a big release for all of us because we got a new package management system called modules built right into the go CLI. If you tried out vgo before 1.11, you'll be familiar with modules. There’s some really cool stuff in there, but there's one piece that a lot of us missed that we need to pay special attention to: the download API.

We used to download dependency code directly from GitHub, and that led to major problems for the community. Over time, heavily used packages would change owners or disappear completely, leaving everyone who used it out in the cold. But now we can build federated module proxies. These are servers that download code from GitHub / GitLab / etc..., save code in their own storage, and Gophers fetch their dependencies from them. This new development lets us, as a community, treat our dependencies as immutable artifacts, free up the package owner to focus on development, and separate the code from the released module artifact.

Even better, our proxies can serve these module artifacts to Gophers from CDNs to speed up their builds everywhere. The Athens project is leading the way toward this new world, and it’s a huge step forward for our community!

In this talk, I’ll start with a brief history of broken dependencies both inside and outside our community. Then, I'll summarize why proxies matter, how they help solve broken dependencies today, and where they're still lacking. Finally, I’ll focus specifically on how Athens solves many of those problems, and I'll show a live demo of Athens in action!

You’ll walk away understanding why module proxies and Athens matter, where they're already being used, what this new technology actually fixes, how it makes your life easier (without changing your current workflow much!), and how you can start using Athens right away with very little work.

You’ll also learn why you might want to set up your own Athens server and how to do it. And as an added bonus, you’ll be able to delete your vendor directories and break out of the GOPATH if that’s your thing!
