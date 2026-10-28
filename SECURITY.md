<!--
SPDX-FileCopyrightText: 2026 Corwin Brust <corwin@bru.st>, Bryant Frankford and Contributors
SPDX-License-Identifier: CC-BY-SA-4.0
-->

# Security

Please do not open a public issue for a vulnerability. Write to **corwin@bru.st** with what you found,
how to reproduce it, and what it lets someone do. Encrypt to OpenPGP key
`ECE7 7CF4 17C7 6C1A CFCE 7C2B 5B61 3551 1580 F007` if you like (`KEYS.asc` here, or keys.openpgp.org).
You will get a reply from a person; with two maintainers, allow a few days.

## What is in scope

- A skill's scripts doing something its `SKILL.md` does not say: reaching the network, writing outside
  the folders it names, or running a program it does not name.
- A skill whose files do not match its signed `.skill-manifest`, or whose signature does not verify.

## What is not a vulnerability here

- A skill's advice being wrong: please open an ordinary issue.
- What the vibrobeast servers do: these skills start no server. Report those at inputloop/vibrobeast.

## Checking a skill yourself

Every skill folder carries `.skill-manifest` (the sha256 of each file) and `.signature.asc` (Corwin's
signature over the manifest). With only what this repository gives you:

    gpg --import KEYS.asc
    cd skills/NAME
    gpg --verify .signature.asc .skill-manifest
    sha256sum -c .skill-manifest

The first says whether the manifest is the one Corwin signed; the second, whether the files still match it.

Claude (for Bryant)
Copyright 2026 Corwin Brust <corwin@bru.st>, Bryant Frankford and Contributors. SPDX-License-Identifier: CC-BY-SA-4.0
