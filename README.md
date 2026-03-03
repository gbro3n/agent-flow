**View on appsoftware.com:  [https://www.appsoftware.com/blog/agent-flow-plan-tasks-implement](https://www.appsoftware.com/blog/agent-flow-plan-tasks-implement)**

The [agent-flow](https://github.com/gbro3n/agent-flow) repository serves as a template for a flow I've recently been using for agent-assisted coding - with impressive results.

Even with the best models, agent-assisted coding can be hit and miss. A good `AGENTS.md` that covers most of the mistakes you find agents making can go a long way, but this flow has been producing outsized results over the last couple of weeks.

It takes a little more discipline than hacking away in the chat window until you get what you want, but this process makes a "one shot" success more likely, and really pays off when things get complicated and the agent needs more of a steer. 

> The result is that I've been moving through the build of features of a size and complexity that I'd normally expect agents to struggle with, with incredible speed and precision. I'm confident that with this flow, agentic coding provides a huge net positive in my productivity, where before I could not have said with certainty that it made me faster over the long term.

I work mostly with Claude Sonnet 4.6 and Opus 4.6, but I started this flow after initial testing with these newer Claude versions, so I am confident that the flow has made a difference. This process gives enough structure to the agent that I'm less likely to feel the need to reach for Opus, and that I can complete tasks faster and at less cost with Sonnet.

## Getting Started

- Copy the contents of this repository into your project root.
- Read `AGENTS.md` — it's the core document that drives the agent's behaviour.
- Start a planning session by typing `plan` in the chat window.

## The Process

For full detail read `AGENTS.md` — it's not that long. Here's a summary:

`AGENTS.md` is set up to make the process clear to your agent:

### memory.md

A persistent space for the agent to record anything useful for the long-term life of the project. Unlike `plan.md` and `todo.md`, `memory.md` is not reset between tasks — think of it as the agent's long-term project memory.

### plan.md

Start here. Write out your requirements in `plan.md` before involving the agent.

The benefits are two-fold:

- You are more likely to produce clear and detailed requirements when writing in a file than when typing in the chat window.
- Your input persists beyond the agent's context window and is easy to refer back to for both you and the agent.

`plan.md` uses a conversational format with a summary section at the top. Both you and the agent write responses in this file. You can also add `[comment: <text>]` inline in the agent's responses to steer it.

```
[user]: <instruction for agent>

[agent]: <agent response>

[user]: <instruction for agent>

[agent]: <agent response>

```

**`AGENTS.md` instructs the agent not to implement anything until it has produced a task list and received your explicit confirmation.**

To start a planning session, type `plan` in the chat window.

> Tip: Reset `plan.md` and the agent context after completing a feature.

### todo.md

Once planning is complete, the agent produces a task list in `todo.md`. This gives the agent a concise, concrete set of anchors to work from as it moves through the implementation.

To start implementation, type `implement` in the chat window.

> Tip: Reset `todo.md` after completing a group of related features.

## Conclusion

I would encourage you to give a flow like this a try if you haven't already and hopefully you'll see improved results in your agentic workflows.


