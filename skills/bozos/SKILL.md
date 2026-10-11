---
name: bozos
description: Make the agent address/process BOZO comments in the codebase
disable-model-invocation: true
user-invocable: true
metadata:
  author: paperbenni
  version: "0.1.0"
  opencode/slash: "true"
  opencode/autoinvoke: "false"
---

# Weekly Review

I have left BOZO comments throughout the codebase. A BOZO is not necessarily the same as a TODO. I occasionally peruse the codebase and flag anything that catches my eye with a BOZO. That might be because I don't understand a piece of code or because I have an idea what to change or because I suspect there is a problem. They are rough thoughts, not tasks or opinions set in stone. They're things I want your input on and which you should investigate. 

There are different possibilities on what I want you to do. If a BOZO turns out as me just lacking knowledge about the domain or codebase then I want you to explain that knowledge to me in a way that doesn't assume I know the codebase by heart (I wouldn't have left the BOZO otherwise)

If a BOZO requires explanation, then also ask yourself if the codebase is confusing or bad in some way which makes it difficult to understand or if I just haven't read enough of it yet. Both are possible. You are here to save me time, so it's perfectly possible that I have been lazy and want you to explain stuff to me. At the same time, it is also possible that the codebase shouldn't be in a way which requires BOZOs to understand (misnomers, unnecessary complexity, or maybe I dont understand it because it straight up does not make sense and is a bug) it and should be changed. If it should be changed in your opinion, come up with suggestions. 

If a BOZO turns out to have an obvious code change which can address it then do it directly. 

If a BOZO turns out to be a real problem, then investigate how to solve it, what the consequences of the solutions are and then give me recommendations. I prefer breaking changes over workarounds or tech debt, keep that in mind for suggestions (but no unnecessary breaking changes, I want them only if they improve things)


