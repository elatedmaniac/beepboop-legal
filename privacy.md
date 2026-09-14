---
title: Privacy Policy
permalink: /privacy/
---
# Privacy Policy

This policy explains how **BeepBoop** (the “Service”), operated by
**{{ site.operator_name | default: '[operator name pending]' | escape }}**
(“we,” “us”), handles information when you use the bot, its account-linking flow
and its related research services. The operator is based in
{{ site.operator_location | default: '[operator location pending]' | escape }}.

{% if site.draft %}
**Current implementation limits:** the operator has confirmed that service-held
data is not encrypted at rest. An owner-approved deletion workflow is being
validated; automated cleanup does not cover every log, backup, export or
third-party copy. A complete linked-account exercise remains outstanding. This
draft is not evidence that those protections or full erasure have been verified.
{% endif %}

## Information we process

**Discord account and conversation information.** We process Discord user IDs,
usernames or display names, relevant server memberships and roles, channel and
thread IDs, message IDs and timestamps, commands, messages directed to the bot,
and attachments you submit for processing. We may read a limited recent history
of the conversation, including other participants' messages and the opening
message of a research thread, to understand follow-up requests. Other
participants' contributions may therefore be processed even when they did not
send the latest command. This is not a feature for collecting unrelated Discord
conversations.

**Sign-in and access information.** Google sign-in is currently mediated by
Cloudflare Access. We receive a verified email address and, when available, a
display name and identity/session claims. The account-linking record associates
your verified email with your Discord ID and records link and expiry times.
Older records may contain profile details such as an avatar URL. We also store
permission tiers, session ownership and invitations, and access/approval audit
records. BeepBoop does not receive your Google password or request Gmail, Drive
or Calendar contents through this sign-in flow. Google and Cloudflare handle
credentials and any authentication methods you enroll with them.

**Research and analysis content.** We process prompts, generated responses,
submitted documents, extracted text, searchable representations of documents
(including embeddings), sources and citations, dataset references, downloaded or
uploaded files, code, execution results, notebooks, maps and other artifacts.
Server research may also create shared work tickets, progress summaries and
graph records. Embeddings and summaries can still relate to you or contain
information from your documents; they are not inherently anonymous.

**Operational and support information.** Logs may include identifiers and email
addresses, request and session IDs, timestamps, tool names, approval decisions,
file paths, content hashes, errors, and short snippets of tool inputs or code.
We also process messages you send for support or privacy requests. Our hosting,
network and authentication providers may process IP addresses, browser/device
information, HTTP requests, cookies and security events when you use related
web pages or sign in.

## Why we use information

We use this information to authenticate you, enforce permissions, answer
requests, retrieve relevant research, carry out authorized analysis, preserve
work you choose to save, deliver results, provide support, manage resources,
and investigate faults, abuse or security incidents. We may use aggregated or
de-identified operational information to improve reliability and usability.

We do not sell personal information or Discord API data, use it for targeted
advertising, or disclose it to data brokers. We do not use Discord messages or
Google sign-in information to train or fine-tune AI models. Processing a prompt
to generate a response or indexing a document for retrieval is different from
training model weights.

Where applicable law requires a legal basis, we rely on what is necessary to
provide the service you request, our legitimate interests in operating and
securing it where permitted, legal obligations, or consent where required. You
may withdraw consent where it is the basis for processing; this does not change
the lawfulness of earlier processing and may prevent the affected feature from
working. Acceptance of the Terms is not blanket consent to unrelated data uses.

## Where content goes and who can access it

**The local research service.** The language model and research storage are
currently self-hosted. The language model processes the conversation context and
relevant tool results. This does not make the whole workflow offline: external
research and authentication features still contact other providers.

**Shared and private spaces.** Replies in a server thread are visible according
to Discord's permissions. The shared research library can be read by authorized
service users and is curated by its owner. Shared tickets and research graph
records can be accessed through the service by users whose permissions allow
it. Analysis session members can use that session's files.

A private DM uses your personal library and an owner-only analysis session.
Shared graph, browser and work-ticket tools are excluded from private mode.
Private content is not automatically published to the shared library. However,
Discord still delivers and stores the conversation, and the operator and trusted
administrative services can access underlying files, databases and logs when
needed to operate, support or secure the Service. The Service does not provide
end-to-end encryption against its operator. An ephemeral command reply limits
its visibility in Discord; it does not erase a saved dataset or make shared
session files private from that session's members.

**External services.** Depending on the feature you use:

- **Discord** receives messages, responses and attachments delivered through the
  bot and processes platform account and usage data.
- **Google and Cloudflare** process sign-in and access-security information.
  Cloudflare also provides DNS, edge delivery and security for related sites.
  Email sent to our privacy contact is forwarded through Cloudflare to the
  operator's Gmail inbox, so these providers also process those support messages
  and their attachments.
- **Tavily** may receive search terms generated from your request or page URLs
  when web search or its page-extraction fallback is used.
- **Hugging Face, Kaggle, geographic-data providers and visited websites** may
  receive search terms, resource identifiers, URLs and network request metadata
  when the Service retrieves information. Information entered into a website
  through a browser action is received by that website.
- **GitHub Pages** hosts this public information site. Requests to it are handled
  by GitHub and, where configured, Cloudflare. The site itself contains no
  analytics script, advertising tracker or tracking form. Hosting/security
  providers may still keep access logs or use necessary security cookies.

Do not include secrets or unnecessary personal information in research queries:
query text can be sent to the selected provider. Some read-only research steps
run automatically within your permissions; not every external request produces
an individual approval prompt. Provider credentials configured by the lab
operator are not given to the analysis worker.

We disclose information only as necessary for these service functions, at your
direction, to authorized recipients in the space you use, or as required by law.
We do not automatically transfer private research to an unrelated new owner or
use it for an unrelated purpose. A material change requires an updated notice
and any consent required by law or platform policy. Third-party services also
apply their own privacy policies and terms.

## Retention

Different records have different lifecycles:

- Recent conversation context is loaded as needed. Ending a turn or expiring an
  in-memory session does not delete Discord's messages or saved research.
- Account links remain until unlinked; an expired link cannot authorize new
  use, but expiry alone does not purge all associated records.
- Documents, searchable representations, tickets, graph records, notebooks,
  assets and their provenance can persist for ongoing research. These stores
  currently do not all have automatic age-based deletion. We retain information
  only while needed for the stated functions or legally required. Removal
  requests require manual review across the relevant stores.
- Contributions to a public/shared dataset, research collection, ticket or
  graph may remain available to authorized readers after the contributor
  deletes their account, where continued retention is permitted for ongoing
  research. Account deletion does not automatically withdraw those shared
  contributions. The operator remains the curator of the general collection.
  This does not override required deletion of personal information or Discord
  API data: the owner reviews and removes or redacts such content as required.
- Account deletion includes the creator's session files, notebooks and artifacts,
  even when they belong to a shared Discord research thread. These files are
  deleted, not transferred to the operator; other participants may lose access.
  Copies in another person's session require separate review.
- Minimal deletion-request evidence and hashed account suppression identifiers
  may remain to document handling and prevent accidental re-admission or
  restoration. These hashes are pseudonymous, not anonymous. Retention is
  limited to those purposes and remains subject to applicable deletion duties.
- Central operational logs are configured to expire after approximately
  30 days. Separate account/source audit records and backups have different
  lifecycles; the log setting is not a promise that every copy expires then.

We are required to promptly delete Discord API data when you or Discord request it, when it is
no longer needed for permitted functionality, or when the Service stops
operating, except where retention is legally required. A deletion request also
requires review of derived records and backups we control. We will explain any
legally required retention and how backup copies are handled. We do not treat
an old backup as permission to restore deleted information into active use.

## Your choices and deletion requests

{% if site.contact_email != "" %}
Email [{{ site.contact_email }}](mailto:{{ site.contact_email }}) to request
access, correction, an available export, or deletion of your information.
{% else %}
**Draft: a working public contact email for access, correction, export and
deletion requests must be supplied before publication.**
{% endif %}

Provide your Discord user ID and the relevant thread, document or asset IDs if
known. Do not send a password, API key, login code or full identity document.
We will verify the request using proportionate information, avoid disclosing
another person's data, and respond without undue delay within any applicable
legal deadline. Explain if you need to contact us after losing access to the
bot; you do not need an active bot session to make a request.

Where available, `/privacy request` records a deletion request. The operator
reviews the scope and approves a maintenance plan; deletion begins only when an
authorized administrator runs it on the lab host. The request itself does not
delete data. The workflow removes account access, the private research workspace
and creator-owned session files. Shared corpus contributions remain by default;
required shared-content removals are handled by the owner. Logs, backups, exports,
Discord messages and other residual copies require separate review and evidence.
Owner approval is an operational safeguard, not a waiver of deletion rights or
a reason to delay handling beyond applicable requirements.

`/unlink` disconnects the Discord/Google binding; it does **not** erase saved
research, audit records or Discord messages. Removing a bot from a server,
revoking Google access, stopping a Python worker or deleting a Discord message
also does not automatically erase all service-held copies. Where available,
`/data remove` withdraws one session asset; derived files and other records can
remain. Use a privacy deletion request for a broader cleanup.

Depending on your location and the laws that apply, you may also have rights to
restrict or object to processing, obtain portable information, appeal a privacy
request decision, or complain to a competent supervisory authority. We do not
penalize you for exercising applicable privacy rights. Some information is
necessary to provide the Service, so deleting it can end your access.

## Security, transfers and age limits

We use access controls, verified sign-in, scoped sessions and isolated analysis
workers to reduce unauthorized access. No system can guarantee complete
security. If an incident affects your information, we will investigate, take
appropriate remedial steps, and notify affected users and Discord as required
by applicable law and platform obligations.

The operator is based in the location identified above; hosting, authentication
and research providers may process information in other countries. Where
applicable law requires safeguards for international transfers, those
requirements must be met for the relevant processing.

The Service is intended for people aged **{{ site.minimum_age }} or older** who
also meet Discord's and Google's eligibility requirements. We do not knowingly
provide it to younger users. Contact us if you believe a child below the
applicable minimum has supplied personal information so we can investigate and
remove it as appropriate.

## Changes and contact

The effective date appears at the top of this page. We will post revised policies
here and provide notice through an appropriate service channel when changes are
material. Where consent is required for a new use, we will seek it before that
use begins.

{% if site.contact_email != "" %}
Privacy contact: [{{ site.contact_email }}](mailto:{{ site.contact_email }}).
{% else %}
Privacy contact: **[pending operator confirmation]**.
{% endif %}

[Terms of Service]({{ '/terms/' | relative_url }})
