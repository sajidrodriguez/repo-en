# Intelligent systems

[← Back to the overview](./README.md)

## What I solve

I design assistants that recognize intent, retrieve information, use tools and
know when to hand control back to a person. AI operates within a business
system with clear boundaries.

Mobilec project status refers to my employment there, which has ended;
it does not imply that I currently maintain those systems.

## Selected implementations

### AI conversational assistant with human handoff · production

Conversational orchestration for customer service and support. It connects
customer requests with operational capabilities through a separate middleware
application. It includes handoff to human teams and actions involving physical
devices.
I used OpenAI with tool calling and conversational memory to connect the
conversation to authorized capabilities while retaining human handoff.

### Real-time voice · implemented and tested

During my employment at Mobilec, I implemented and tested the voice experience
in a controlled environment with Twilio Media Streams and WebSockets.

### Virtual agent · operational

Jit De Flou's virtual agent connects to a support inbox where I can take over
conversations and continue them personally. The agent and inbox are operational.
It can be explored through the [Jit De Flou website](https://jitdeflou.com).

### TopBot · historical

My first conversational system: JavaScript and Node.js on Google Cloud.
It began as sales follow-up automation and opened the path toward development,
APIs and infrastructure.

## Decisions and trade-offs

- Separate conversation from critical integrations.
- Retain human validation for actions involving physical devices.
- Allow optional capabilities, such as voice or proactive monitoring, to be
  disabled without stopping the conversational core. This does not imply fault
  tolerance across all critical components.

## Public evidence and boundaries

- Conversational systems in production.
- Integration of AI, operational data, human support and telemetry.
- A real-time implementation tested in a controlled environment.
- No proprietary code, operational prompts, payloads or customer data.
