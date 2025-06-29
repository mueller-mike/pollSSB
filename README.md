# pollSSB -- based on tinySSB

## Overview
The project tinySSB (Tiny Secure Scuttlebutt) is a minimal, experimental version of the Scuttlebutt protocol designed for constrained environments such as embedded devices. PollSSB extends tinySSB by adding structured voting mechanisms, enabling users to propose polls and cast votes, all while preserving the append-only, gossip-based, and cryptographically secure nature of the underlying protocol.

## Objectives
- Enable decentralized polling functionality over tinySSB.
- Ensure tamper-proof vote recording through append-only logs.
- Maintain low resource usage and compatibility with embedded systems.
- Preserve the core principles of tinySSB: no global state, no central server, and local-first data handling.

## Features
- Poll Creation: Users can create a poll message in a chat with a title, description, and set of options.
- Integrity: All votes are cryptographically signed and timestamped.
- Vote Counting: Nodes independently compute results by traversing the log.
- Offline-first: Works in disconnected environments; votes sync when peers come online.
- Voting: Participants can vote by appending a vote message referencing the poll and their chosen option.

## Authors
This project is developed as part of a course on internet and distributed systems at university basel. Contributors include:
- Gioia Almer
- Yanick Spichty
- Max Reinert
- Mike Müller

## License
This project is licensed under the MIT License.
