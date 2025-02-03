---
date:
  created: 2025-02-01
tags:
  - brog
  - announcement
---

# Announcing Brog 
## An open source GitOps tool for bootc systems.

Over the past year at [Mehal Technologies](https://mehal.tech/) we've been deploying [bootable containers (bootc)](https://docs.fedoraproject.org/en-US/bootc/getting-started/) at the edge in production environments. Bootc is a massive productivity boost and as outlined in [the documentation](../../overviews/why-bootc.md) it improves deployment cycles by **80%** even in scenarios where hardware peripheral integration is a key part of the validation cycle

This enables our partners to get to market faster.

Given the success we've had with the provisioning during development we want to use the same techniques in production but we came across some potential issues.

1. **Configuration management**: Operations and developments teams using a container registry to understand what has been deployed to the estate is clumsy and error prone.   
   
1. **Auditability**: Extending the audit mechanism to the container registry is problematic as the authorization to deploy is implicit in the push to the registry rather than an explicit decision to push to the estate. 

1. **Failed update management**: No matter how careful a company is during updates there is always potential for machines to become unusable. This problem hit the headlines in 2024 with the [CrowdStrike outage](https://en.wikipedia.org/wiki/2024_CrowdStrike-related_IT_outages) and while bootc has an automated rollback feature that prevents this from becoming a prolonged issue our partners would prefer not to have to deal with the flood of support calls creating a [thundering herd](https://en.wikipedia.org/wiki/Thundering_herd_problem). 

Given the above issues we decided to build [brog](https://github.com/ubiquitous-factory/brog) - gitops client for bootc. 

Brog directly addresses items 1 and 2 and we will be making further announcements on how brog integrates with [clos - the mehal cloud platform](https://mehal.tech) to provide incremental roll outs (A.K.A Canary Deploys) to solve for item 3 end to end. 

A tutorial on how to use brog is [available](../../howto/getting-started.md) and there will be making further announcements in the near future.

If you want to know more about the brog roadmap or need help deploying it then please reach out to admin@mehal.tech.
