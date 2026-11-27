# Reverse Engineer Anything

## Ask before you start

- Ask EB for the target name and link and for the exact feature he wants rebuilt.

- Ask EB what the rebuilt version is for and who will use it.

- Ask EB which parts matter most and which parts he can leave out.

- Do not start an analysis until EB has named the target and the feature.

- Record the target, the feature and the wanted outcome in plain words before you do any analysis.

## Study what people can see

- Study the public website, the public screens, the user flows and the help pages first.

- List each screen, each step in each flow and each visible feature in plain UK English.

- Note where a feature starts, what it asks for, what it shows and what it returns.

- Compare the public behaviour with EB's own product and note the gaps in plain words.

- Stop when another look is unlikely to change the feature list.

## Use REA for deeper evidence

- Use REA only after the visible study is done and only for the feature EB named.

- Get REA from the official source at https://github.com/morluto/rea or from the rea-agents npm package.

- Run `npx rea-agents setup` from a trusted directory outside the project under analysis when REA is not yet set up.

- Run `npx -y rea-agents@latest analyze-javascript-application /absolute/path/to/app --json` for an extracted JavaScript or Electron app.

- Use REA to trace modules, imports, routes and Electron boundaries and to show the evidence for each finding.

- Report what REA found, what it did not find and what is still uncertain.

- Treat REA output as evidence for a fresh build, never as code to paste into EB's product.

## Build a clean room version

- Build EB's own original version from the feature list and the REA evidence.

- Use EB Wealth or Empowerment Body branding and plain UK English throughout.

- Write for a working parent audience with short sentences and everyday examples.

- Do not copy proprietary source code, branding, trademarks, logos or wording from the target.

- Do not break the target terms of service and do not bypass a login, a paywall or an access control.

- Do not decompile or analyse a binary or an app that EB does not own or does not have permission to analyse.

- Do not present a lookalike as the original product and do not claim EB's version is the original.

- Check the finished build against the feature list and fix the gaps before you show it to EB.

## Build the EB video call tool

- Build the video call tool from open components such as Jitsi or LiveKit rather than copying Zoom.

- Give EB a link he can send to a client so the client can join without an account and without paying for Zoom.

- Add recording, transcription and a short PDF summary after each call.

- Put the main points, the clarifications and the next steps in the PDF in plain UK English.

- Keep the PDF short enough to send in a message and clear enough to read without the recording.

- Ask EB before you choose a host or a paid service for calls, recording or storage.

## Limits of this skill

- REA needs Node.js 22, 24 or 26 plus npm, and this workspace has Node.js 24.22.1.

- Static JavaScript and .NET inspection work without a native analysis engine.

- Deep native analysis needs Hopper, Ghidra, IDA or Kuna, and none of those are installed in this workspace yet.

- REA analyses targets locally and returns pseudocode and assembly for native code, so the agent still writes and tests the fresh implementation.

- REA is not installed as an MCP server in Muse, so treat the commands in this skill as the way to run it from the terminal.

- If a target needs a tool that is not available here, say so plainly and offer the visible study plus a clean room build instead.

## Available connectors

- [GitHub](/opt/hatch/connectors/github/CONNECTOR.md) for reading public repos, files and issues, including the REA repo at https://github.com/morluto/rea.

- Use `muse.connector_search` to find other connectors and `muse.skill_search` to find related skills.

- If nothing here fits, look on the web for a maintained API or MCP server and set it up with [Custom Connectors and MCPs](/opt/muse/skills/custom-connector-setup/SKILL.md), or build a custom connector.

## Websites

- [REA](https://github.com/morluto/rea) for the REA source, README and guides. Carry the target name and the feature EB named into any reading and verify the setup steps there.

- [REA guides](https://rea.tools/guides/) for worked guides on targets, providers and evidence.

- [Jitsi](https://jitsi.org/) for open video call components. Carry EB's link based call and recording needs into any reading and verify the hosting options there.

- [LiveKit](https://livekit.io/) for open real time video components. Carry EB's link based call and recording needs into any reading and verify the hosting options there.

## Alternatives for better results

- Start with the visible study when EB only needs the feature list and a fresh build.

- Use an open component when a full rebuild would take too long and the open component already covers the core need.

- Ask EB for a short call recording or a screen walkthrough when the public pages do not show a feature clearly.
