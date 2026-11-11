---
name: opencode-trial-manager
description: Help me try out new free model or stealth model promotions
disable-model-invocation: true
user-invocable: true
metadata:
  author: paperbenni
  version: "0.1.0"
  opencode/slash: "true"
  opencode/autoinvoke: "false"
---

Go into ~/.config/opencode (use the opencode skill if available) and do the
following:

Go through the manually configured custom providers with free models and check
if the providers have any new free models, and if the currently configured free
models still work. Formerly free models might have gone paid, or new free models
might have appeared. Providers might provide an API to list models, or you might
have to read through their docs or new pages on the web. 

Some providers might put free somewhere in the model ids or names, some might not. 
Before doing any checks or experiments which might be expensive, ask me first. 
Sending a ping prompt to a model you suspect to be free or at least cheap is
allowed, but anything big by google, openAI or Anthropic is off limits. 

The user might tell you about a promotion they heard of, in that case you're
definitely allowed to mess with the model they tasked you to. 

If you are unsure about any model, then just skip it, and present the user with
all the models/providers you were unsure about and ask the user what to do (with
suggestions as well)



