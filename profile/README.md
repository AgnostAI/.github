# Agnost AI

**Agnost AI monitors AI agents in production: chat agents, voice agents, copilots and MCP servers.**
It judges whole conversations to catch failures, frustrated users and broken tool calls, alerts in
Slack, and opens pull requests with fixes tested against past runs.

- **Judges conversations, not single traces.** Traffic is grouped by user and session, so Agnost sees
  loops, repeated questions, wrong answers that look like success, and users who give up.
- **Plain-language checks.** Write a rule like "never promise a refund"; an LLM judge checks every
  assistant message once the conversation goes idle and flags each one pass or fail.
- **Alerts in Slack or email** when a failure, intent or rule violation crosses a threshold.
- **Fixes as pull requests.** When an alert fires, Agnost opens a PR with a fix, replays the affected
  conversations against it, and shows the results in the PR for a human to review.
- **OpenTelemetry-native.** Python and TypeScript SDKs, plus guides for the OpenAI Agents SDK,
  Vercel AI SDK, LangChain/LangGraph, Mastra, Pydantic AI, Google ADK and Agno, and voice platforms
  such as LiveKit, Pipecat, Vapi and Retell.

[Website](https://agnost.ai) · [Docs](https://docs.agnost.ai) · [Start free](https://app.agnost.ai) · Backed by [Y Combinator](https://www.ycombinator.com/companies/agnost-ai) (S26)

### Open source from the team

- [create-evals](https://github.com/AgnostAI/create-evals): build ~10 evals from what your agent actually gets wrong.
- [improvemyagent](https://github.com/AgnostAI/improvemyagent): turn the corrections you keep repeating to your coding agent into AGENTS.md rules.
- [support-desk-bench](https://github.com/AgnostAI/support-desk-bench): frontier models answering 400 real Wix support tickets, judged against expert answers.
