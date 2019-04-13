---
title: Libraries, Patterns, and Puppies
tags: elixir pattern
---
I've published an Elixir github repository called [Quest](https://github.com/gvaughn/quest) that I'm not certain what to do with. Primarily
I think of it as a pattern, not a library, though it could probably be developed into a library. My thoughts
lately have made me more wary of libraries than I used to be.

Once upon a time the Free Software movement and Open Source movement had a slogan to distinguish one from
the other: "free as in *freedom* vs. free as in *beer*." I don't wish to discuss those ideological differences,
but mention that for some historical grounding. I've since heard, but forgotten the original source of
the simile: "free as in *puppy*." This suggests that adding some library to your project means that you are
taking on some long term maintenance responsibilities. Younger me and the teams I was on have dealt with the
pain of deep, convoluted dependency trees that became a source of inertia holding the project back because
it was too much work relative to the gain to upgrade to a new version of a primary library/framework we were
using. If we had been a bit more wary of each dependency as we added it and asked ourselves if perhaps we should
instead write and own that functionality ourselves, then we might have overall improved the long term velocity of
our project precisely because we did not have to wait for (or fork) the library in order for its depedencies
to be compatible with the rest of our set.

I love puppies! Puppies are great! I am not suggesting that we never use third party libraries in our projects,
but instead that we be more thoughtful of which ones and how many we choose to adopt. We should be aware of
those short term vs. long term considerations. We should think about the knowlege and skill gained if we
ourselves write that portion of functionality we need out of the whole set a library might provide. That brings
me to thoughts of my [Quest](https://github.com/gvaughn/quest) repository.

Forgive me for throwing out yet another old saying: "Give someone a fish, feed them for a day. Teach them how to
fish, feed them for a lifetime." Giving someone a pattern is more like teaching them how to fish, while giving
them a library is like giving them a fish. In the culture of some programming languages it is common to see
API client libraries that are for one specific service, like a Twitter client library, or Github, etc. but with
[Quest](https://github.com/gvaughn/quest) I'm not providing any concrete implementation for any specific service. Instead it provides a struct that
can describe any HTTP API call along with examples of how to interact with it. The value it offers is packaging
what is conceptually an *action* into a *thing*, a data structure. Doing this allows for reusable infrastructure for
dealing with HTTP calls, and even allows for concurrent tests without any mocking library.

## Conclusion?

Help me decide. Does this mesh with your view of third party libraries? Should I develop [Quest](https://github.com/gvaughn/quest) into a library and
publish on hex? Can I do that and still provide the didactic goal of the pattern? Is it better to treat it
as a tutorial repo?

I have no comments on this blog, but you can find me as *gregvaughn* on Twitter, Elixir Slack, ElixirForum.
