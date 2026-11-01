<!--
SPDX-FileCopyrightText: 2026 INPUTLOOP (Corwin Brust, Bryant Frankford and the people in ACKNOWLEDGEMENTS)
SPDX-License-Identifier: CC-BY-SA-4.0
-->

# Privacy -- vibrobeast-skills

This plugin is skills alone: written ways of working that Claude reads when a task calls for them.

- **It starts no server and opens no connection.** Installing it adds text Claude can read, and the
  scripts some skills carry.
- **Scripts run only through Claude, in the open.** A skill's script runs when Claude runs it with the
  tools you allow, in the session you watch; what it reads and writes is what that run shows. None of
  them sends anything off your computer unless the skill says so where it asks for the run (a skill that
  publishes or pushes says where to, and asks first).
- **It keeps nothing about you.** The skills hold no record of you; anything written is written where
  you work, by a run you saw.
- **The memory, persona sheets, rooms and doors** are in the full plugin, inputloop/vibrobeast, whose
  PRIVACY.md is checked against its source at each build.
- What Claude itself sends to Anthropic while it works is governed by Anthropic's terms and privacy
  policy, not by this one.

Authored by Mentat (for Corwin; claude-opus-5-5).
Copyright 2026 INPUTLOOP; CC-BY-SA-4.0; https://github.com/inputloop
