# Club Zero

SPIFFE and SPIRE are important infrastructure projects. As such, to be truly successful, they should be “boring”. What does that mean? It means they should be foundational, seamless, and ubiquitous. To the point that you almost forget they exist. SPIFFE should be the default, not a decision point. SPIRE should be the default OSS way to get there..

We are not there yet. How do we turn this vision into reality? Enter Club Zero. Here, we will gather People, and other resources to try and move the ecosystem around SPIFFE and SPIRE towards this goal.

To achieve this goal, we must build a vibrant ecosystem, and not just look at contributing directly to the SPIFFE or SPIRE projects.

# Personas

We need your help to make the vision a reality. We’ve come up with some ways folks can help based on personas.

* [End Users](#end-users) \- I would like my communications secure
* [System Administrators](#system-administrators) \- I need to maintain systems (in a secure way)
* [Security Professionals](#security-professionals) \- I’m on the hook to ensure things are secure
* [OS Distribution Providers](#os-distribution-providers) \- I provide software packages for others to use
* [3rd party Packagers](#3rd-party-packagers) \- I provide packages when Distributions do not yet
* [Documenters](#documenters) \- I write documentation for software
* [Influencers](#influencers) \- I help others become aware of important things
* [Translators](#translators) \- I make inaccessible knowledge accessible
* [Software Developers](#software-developers) \- I make the impossible possible
* Other \- Did we miss you? Please let us know.

# Bootstrapping the ecosystem

The biggest impediment to achieving the vision is inertia. We need to describe the problem before we can work on fixing it.

No one really deploys infrastructure just to deploy it. They deploy it to solve a particular part of a bigger problem. Solving the bigger problem is the thing they really care about.

There tends to be a self reinforcing situation in infrastructure around sysadmins, developers, and security professionals that we need to overcome.

All three personas may push back against SPIFFE for the reason that they will be betting on a standard, and unsure if SPIFFE is the most widely adopted and mature one.

For a system administrator, they would deploy SPIFFE and/or SPIRE if one of the following were true:

1. Software they or their users want to use requires it
2. Management or the Security Team requires a capability provided by it
3. Contracts or other B2B relationships require it
4. If it provided significant security benefits for minimal extra effort

Reasons they push back adopting SPIFFE:

1. If self maintaining
   1. Concern that Managing PKI is hard
   2. Another thing to learn
   3. Difficulty in configuration
   4. Another thing to maintain
   5. If there are too few things that need the dependency, its hard to justify
2. If outsourcing responsibility
   1. Who do I call for support
   2. More vendors support traditional PKI then SPIFFE

For Developers, they would add SPIFFE and/or SPIRE as a dependency if:

1. It enabled easier to setup identity management with little code change required
2. It allowed rotation of credentials without having to manually do so
3. It allowed them to no longer need to think about credentials
4. It stops the security team from bothering them

Reasons they push back:

1. Desire not to add additional dependencies
2. Thinking system admins won’t want to maintain the dependency.
3. Too hard to change the existing code to match the SPIFFE model.
4. Security Professionals / System administrators not requiring tighter security. “Good enough” security.

Security Professionals would want to recommend or require SPIFFE and/or SPIRE if:

1. It enhances the organization's security posture
2. It allows them to meet a policy or regulations

Reasons they push back:

1. Overly burdensome on system administrators or developers
2. Possible bad relationship with engineering

# Strategic project contribution

We will initially have limited resources in Club Zero. If there are particular applications you want to work on, please work on those. But if you are looking for something to work on, we can be more strategic. Strategic contributions to key applications will accelerate adoption. We will keep a list of such projects in the club zero issue tracker.

# How can I help

Join us on SPIFFE Slack in \#clubzero. Here we can talk to each other on what we can do to help.

Here are some ideas oh how you can help, per persona.

## End Users

Make it known you want end to end encryption for safety. Ask about security of the systems you use. Ask if SPIFFE or SPIRE is being used.

Back to: [How can I help](#how-can-i-help)

## System Administrators

Try deploying SPIFFE based technologies such as SPIRE. If anything is harder then you expect, please let us know where the pain points are. We believe we have addressed the pain points already to make an easy to use system, but may have missed some and would love to work with you to identify and fix any such issues for you. Also, work with your security and developer teams to raise awareness of SPIFFE. Ask your Distribution support channels for direct support.

Back to: [How can I help](#how-can-i-help)

## Security Professionals

Encourage System Administrators and Developers to use SPIFFE ecosystem tools to secure their systems. Consider suggesting, or requiring better than 1+ year wildcard certificates for security. Recommend killing off all passwords wherever possible. Request additional security in the form of additional attestation (EX: The TPM attested for the physical node. The cloud provider attested that the VM is in their datacenter)

Back to: [How can I help](#how-can-i-help)

## OS Distribution Providers

Consider packaging and supporting SPIFFE ecosystem projects, including SPIRE.

Back to: [How can I help](#how-can-i-help)

## 3rd party Packagers

If your favorite Distribution does not have native support for SPIFFE ecosystem projects, help us package them up and keep them up to date.

Talk to the developers you work with about adding SPIFFE support directly to their projects. Talk to the system administrators you work with about deploying SPIFFE infrastructure such as SPIRE or SPIRL

If the developers don’t plan to quickly support SPIFFE, sometimes it can be solved using bridge technologies from within the packaging. Consider implementing this where possible. (EX: Adding SPIFFE support to a helm chart via spiffe-helper)

Back to: [How can I help](#how-can-i-help)

## Documenters

We could use your help writing easier to understand / use documentation for all parts of the ecosystem. The easier to understand / deploy, the sooner we solve difficult to otherwise solve security problems helping everyone.

Back to: [How can I help](#how-can-i-help)

## Influencers

Security is a critically important part of computing, but few people understand it or know what great tooling is available. You can help us raise awareness of the problem space, and help work to get everyone on the same page towards solving really important security problems.

Videos or blogs can be created talking about particular functionality, how to do something, how to debug something, etc.

Back to: [How can I help](#how-can-i-help)

## Translators

Even if we have content, it isn’t very useful if folks can’t understand it. Making it available to more folks in their native languages is a significant contribution.

Back to: [How can I help](#how-can-i-help)

## Software Developers

Software Developers often have many different ways of developing. We’ve further broken down some ways you can help based on what you're working on.

Back to: [How can I help](#how-can-i-help)

### If your producing a product / work on an open source project

Strongly consider how support SPIFFE could help make security better while at the same time, reducing the amount of effort it will take you and your users to manage that security. If you work with system administrators or security professionals, help raise awareness of SPIFFE and SPIRE as a solution to their security related needs.

### If you’re looking for a project to work on

Please consider the strategic project list above or chat with us on the \#clubzero slack channel

### If you’re looking for other infrastructure to help out with

Consider adding easy to use SPIFFE support into your favorite language libraries or platforms.

While the ideal is for projects to directly support SPIFFE, sometimes that can be hard to do for non technical reasons. Consider contributing to bridge technologies such as spiffe-helper, ghosttunnel, etc. These projects enable the ecosystem to grow even without direct support.

Back to: [How can I help](#how-can-i-help)
