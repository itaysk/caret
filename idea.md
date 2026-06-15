# Caret

TL;DR: I'm tired of copy-pasting between chat and other apps. We need an IDE for writing and thinking: Obsidian + Google Docs + LLM-Wiki + Agents.

This is an idea for a product, something that I desperately need for myself and still haven't found a good solution for. It's about how AI assists writing, researching and thinking. You might say it's a solved problem, isn't it? Don't we already use AI for writing, researching and thinking all the time? Well yes but in a very awkward way because AI currently lives in Chat. I can do some research in chat, I can produce a draft in chat, I can proof-read something or investigate something and it can be quite useful for ad-hoc tasks but it's the wrong paradigm for long-term, meaningful work. As a matter of fact, I have access to all the state-of-the-art AI tools and I'm still writing this text in a text editor. I need my agent here with me.

In fact, we've been here before - software development was one of the first to be disrupted by AI. 
I remember typing coding issues into ChatGPT. It would spit out code, which you then carefully copy into your project, modify it to fit the use case, test it, pass the feedback back to chat, and so on and so forth... That was objectively bad experience, so we changed it - we took the AI and integrated it into the Development Environment (IDE). Now the AI is right there in the IDE collaborating with you. It can see what you're working on, it can make changes directly to your code, it can test and engage with your tools - It's a seamless experience that keeps you in the flow.

Cursor was one of the first to put the AI directly in the user's environment, and pioneered the Agentic IDE. **What cursor is to coding, Caret is to writing, researching and thinking**. This text should have been written in something Caret.

## New paradigm

### User Interface

1. With chat, **You need to start by asking a question**: You always need to initiate the agent, and the agent has to respond to your specific input. This dramatically limits the creative process.
	1. What if: The app features a document editor as the center piece. You aren't forced to Q&A, you can simply start writing. This document is a canvas for interacting with agents, just like collaborating on a document with your co-workers.
2. With chat, **You are locked out of the artifact**: The agent is the only one with write access to the artifact you're creating. Want to make a small change? you have to ask the agent to do it, and we all know how frustrating that can be.
	1. What if: Agent's output isn't confined to a chat message, it's added straight to the document. And you can always edit it however you want and make it your own. You are in control, the agents are there to help.
3. With chat, **It's hard to follow along**: The more meaningful the chat, the faster it grows into unwieldy mess. Trying to understand what is the current state (of the artifact), looking up or referring to a previous message is too hard.
	1. What if: The main document, which clearly reflects the current state of work. You can comment on text selection and AI changes are tracked and previewed. You always have an clear view of what you've achieved and can iterate on it confidently without loosing track.

This isn't ground braking UI, it's basically an IDE for writing and thinking. Let's continue to explore other aspects of the new paradigm.

### Agent Performance

4. With chat, **Context management is a chore**: A chat session is a natural context boundary. If you keep all every conversation in the same chat session, you'll end up with bloated context window which degrade the LLM's performance, and costs you too much. On the other hand, if you start new chats sessions too often, you will end up with context fragments scattered across many chats which also degrades the LLM's performance.
	1. What if: Your work is organized in a workspace which extends the context boundary across chats and artifacts. Context is intelligently managed for each task.
5. With chat, **Grounding is broken**: Agents perform best when they have access to relevant and data source for the particular mission. Curating sources in the same chat where you're trying to get work done complicates the workflow and adds to your cognitive load.
	1. What if: Your workspace has a dedicated knowledge base. You collect relevant sources over time which makes your agents smarter and more productive. The knowledge base is maintained by both you and your agents.
6.  With chat, **You always get one point of view**: Diversifying agents is the best way to optimize results. This refers to both mixing models (e.g Opus for planning, Sonnet for coding, Codex for reviewing) and mixing specialized agents (e.g Planner, Coder, and Reviewer with different instructions). Chat doesn't allow you to do this.
	1. What if: You can easily define agents that represent different views, skills and models, and have them all collaborate with you like virtual co-workers.


## Building blocks
1. Markdown document editor (Similar to HackMD or Obsidian)
2. Wiki knowledge base management and curation (Similar to NotebookLM or LLM-Wiki)
3. Agent definition framework
4. Live collaboration and sharing framework (Similar to Google Docs or HackMD)

All of the building blocks exist but there isn't a single product that package them into a simple experience with a clear vision about how the workflow looks like end to end.

