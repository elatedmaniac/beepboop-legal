---
title: Terms of Service
permalink: /terms/
---
# Terms of Service

These Terms govern use of **BeepBoop** and its related research and analysis
services (the “Service”). They are between you and
**{{ site.operator_name | default: '[operator name pending]' | escape }}**,
based in {{ site.operator_location | default: '[operator location pending]' | escape }}
(the “operator,” “we,” or “us”). BeepBoop is an independent project, not an
official Discord or Google product. Discord and Google are not parties to
these Terms.

## Agreement and eligibility

By using the Service after these Terms are presented or made available to you,
you agree to them. If you do not agree, do not use the Service. You must be at
least **{{ site.minimum_age }} years old**, meet the applicable eligibility
requirements of Discord and Google, and be legally able to accept these Terms.
If acting for an organization, you must have authority to use and submit its
data and to agree on its behalf.

You must also follow [Discord's Terms of Service](https://discord.com/terms),
[Community Guidelines](https://discord.com/guidelines), and applicable provider
terms. These Terms do not override Discord's requirements or give you rights
to anyone else's accounts, systems or data.

## The research beta

BeepBoop provides experimental AI-assisted research, document retrieval, dataset
acquisition, code execution, charts, maps and related analysis. Features may be
limited by permissions, approved providers, session membership, capacity or
availability. The present deployment requires approved access and a linked
Google identity, including for private DMs. Installation alone does not grant
access. A feature description is not a commitment to build a future feature.

The beta is offered without a service fee. If paid features are introduced, we
will disclose their terms and obtain agreement before charging you. Third-party
services may have separate costs and conditions. There is no uptime, response
time, archival or continued-availability guarantee for the beta.

## Accounts, sessions and approvals

Use your own authorized accounts. Keep login credentials and authenticators
secure, and tell us promptly if you suspect misuse. Do not share access tokens,
impersonate another user, bypass permissions, or try to access another person's
private workspace.

Understand the space you are using: server conversations and shared research
can be visible to other authorized users. Invite only people who are authorized
to access a session's files. A private DM is separated from other application
users, but remains subject to the processing described in the
[Privacy Policy]({{ '/privacy/' | relative_url }}).

Review approval prompts before accepting downloads, execution or persistent
changes. Some operations are read-only or run under existing authorization and
do not require a new prompt each time. Approval authorizes the described
operation within your permissions; it does not establish that the operation is
accurate, lawful or safe for your intended use. Stopping a session may lose its
working Python state. Removing an input does not necessarily remove derived
outputs or copies already shared with others.

## Acceptable use

Use the Service only for lawful, authorized purposes. In particular:

- Conduct cybersecurity work only on systems, accounts and data you own or have
  permission to assess. Stay within the authorized scope. Do not use the Service
  for unauthorized intrusion, credential theft, malware deployment, disruption
  or evasion of another service's safeguards.
- Do not use it for fraud, harassment, stalking, doxxing, unlawful surveillance,
  exploitation, or other conduct prohibited by Discord. Do not scrape Discord
  or build profiles of its users or relationships from Discord API data.
- Do not submit passwords, API keys, authentication codes, financial account or
  payment-card details, protected health information, or other sensitive
  personal information whose processing through Discord is prohibited. Remove
  unnecessary personal information from logs and datasets before submitting them.
- Do not use outputs to make unlawful discriminatory decisions or to determine
  a person's eligibility for employment, housing, credit, insurance or similar
  important opportunities. Do not present generated claims as verified evidence
  about an identifiable person without independent verification.
- Respect copyright, privacy, dataset licenses, attribution requirements,
  website terms and rate limits. A public URL or successful download does not
  mean a file is freely licensed or that you may redistribute it.
- Do not sell or redistribute Discord API data, train models on Discord message
  content without Discord's express permission, circumvent download controls,
  or interfere with the Service or other users.

You may report a suspected vulnerability privately to the contact below. These
Terms do not themselves authorize security testing outside your own permitted
research environment.

## Your content and generated results

You retain the rights you have in the material you submit. You give the operator
a limited, non-exclusive permission to store, process, transform and transmit it
as necessary to perform your requests, provide the documented features and
secure the Service, subject to the Privacy Policy and applicable law. This
includes displaying results to the recipients in the conversation or shared
space you choose. It is not a license to sell your personal data or use it for
unrelated model training. Necessary provider processing is described in the
Privacy Policy.

When you contribute material to a public/shared dataset, research collection,
ticket or graph, your permission includes retaining and making that contribution
available to authorized users for the documented research purpose after your
account closes, to the extent permitted by its license, applicable law and
platform requirements. The operator curates the general collection and handles
requests for required removal or redaction. This does not waive privacy rights
or permit retention of personal information or Discord API data that must be
deleted. See the Privacy Policy for the request process.

Creator-owned session files, notebooks and artifacts are treated separately:
account deletion removes them even from shared research threads, without
transferring ownership to the operator. Other participants should not rely on
continued access to those files. Copies outside that session require separate
review.

You must have the rights and permissions needed for the content you submit and
the actions you request. Other contributors and source providers retain their
rights. We do not claim ownership of your inputs merely because you use the
Service. AI output may be similar to other output, include third-party material,
or lack copyright protection; we do not promise exclusive rights or a license
to third-party content. Check source licenses before reuse or publication.

## Verify outputs before relying on them

AI-generated text, code, citations, classifications and calculations may be
incorrect, incomplete, outdated or fabricated. Check original sources and
independently validate important results. Maps may use approximate coordinates,
incomplete observations or generalized boundaries; they are not suitable for
navigation, emergency response or operational targeting. Labels and apparent
precision do not prove accuracy.

Finance-related output is general research, not personalized investment,
trading, tax or legal advice. The Service does not act as your investment adviser
or promise profits. Cybersecurity output is not a professional certification or
a guarantee that a system is secure. Obtain qualified advice where your use
requires it. You remain responsible for deciding how to use and verify results.

## Suspension, termination and changes

You may stop using the Service at any time. `/deauth` disconnects your account
binding and initiates credential and session revocation, including Cloudflare
Access logout. A pending logout is not a completed sign-out. Your role and saved
data remain; contact us for a broader deletion request. Removing the app or
ending a session is not a complete data-deletion operation.

We may restrict or suspend access to address misuse, security concerns, platform
requirements, legal obligations or resource constraints. We may change or stop
experimental features. Where reasonably practicable, we will provide notice and
an opportunity to retrieve your available research before a planned shutdown.
Urgent legal or security circumstances may require immediate action. We will
handle retained data under the Privacy Policy and applicable requirements.

We will post updated Terms with a new effective date and provide appropriate
notice of material changes. If you disagree, stop using the Service. Any consent
or agreement required by law for a change will be obtained as required; merely
posting new terms does not override mandatory rights.

## Disclaimers and responsibility

To the extent permitted by applicable law, the experimental Service is provided
“as is” and “as available,” without warranties of accuracy, availability,
non-infringement, merchantability or fitness for a particular purpose. You should
keep independent copies of important work.

To the extent permitted by applicable law, the operator is not liable for
indirect or consequential losses, lost profits or lost opportunities arising
from use of the Service. Nothing in these Terms excludes liability that cannot
lawfully be excluded, or limits mandatory consumer rights, liability for fraud
or intentional misconduct, or other non-excludable obligations. These Terms do
not impose mandatory arbitration, a class-action waiver, or a requirement to
bring claims in a distant jurisdiction.

## Contact and disputes

{% if site.contact_email != "" %}
For support, abuse reports, privacy requests or concerns about these Terms,
contact [{{ site.contact_email }}](mailto:{{ site.contact_email }}).
{% else %}
**Draft: add a working public operator contact before publication.**
{% endif %}

Please describe the issue without including credentials or unnecessary sensitive
information. We will try to resolve concerns in good faith. Nothing here prevents
you from contacting a regulator or pursuing remedies available under applicable
law. If a provision is unenforceable, the remaining provisions continue to apply
to the extent lawful.

[Privacy Policy]({{ '/privacy/' | relative_url }})
