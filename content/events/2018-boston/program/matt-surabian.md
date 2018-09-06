+++
Title = "Vault At Scale"
Type = "talk"
Speakers = ["matt-surabian"]
+++
As an organization with 25 production environments and over 6,000 containerized applications we have a lot of secrets to manage. Enough to run 12 geographically distributed HA Vault deployments across multiple cloud providers. Even though the Open Source community provides us with some really awesome tooling, managing that many Vault environments can be tricky.

This talk is about how we manage all those Vault servers and some of the unexpected bumps we’ve hit along the road to stability. We’ll cover standard outage events, bugs in Vault itself, dealing with unintended consequences of various authentication paradigms, and even migrating from one backend data store to another without needing to re-key.
