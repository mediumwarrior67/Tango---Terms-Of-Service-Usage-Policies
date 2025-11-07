
# Tango — Terms of Service & Usage Policies

![Tango logo](imgs/logo_500x500.png)

## About Tango
Tango is a community-focused Discord bot that provides moderation helpers, utility commands, and engagement features for servers that invite it. This document contains the Terms of Service (TOS), detailed usage policies, data storage and GDPR-related information, and contact and appeals procedures.

## Quick summary
- Use Tango responsibly and lawfully. Server owners are responsible for configuration and moderation decisions. Misuse may result in removal of bot access or other enforcement actions.

## Table of contents
- Terms of Service
- Usage Policies
- Data collection, storage & GDPR rights
- Moderation, enforcement & appeals
- Contact

## Terms of Service
1. Acceptance of Terms
   - By inviting or using Tango you agree to these Terms of Service and to comply with applicable laws and Discord's Terms of Service. If you do not agree, do not use the bot.

2. Definitions
   - "Maintainers" refers to the creators/operators of Tango. "Server Owner" and "Moderators" refer to the Discord server's authorized administrators.

3. Permissions & Responsibility
   - Server owners are responsible for granting Tango the minimum permissions required for the features they enable. Do not grant admin-level permissions unless necessary and you trust the configuration.

4. Acceptable Use
   - Allowed activities include moderation, anti-abuse protection, community engagement, information lookup, and other utilities provided by Tango when used in good faith.

5. Prohibited Use
   - You must not use Tango to:
     - Harass, threaten, defame, or discriminate against individuals or groups.
     - Publish or distribute illegal content, including but not limited to instructions facilitating wrongdoing.
     - Upload, distribute, or link to sexually explicit content involving minors.
     - Perform spam, phishing, credential harvesting, or other forms of automated abuse.
     - Circumvent, disable, or abuse server moderation tools or the bot's protections.

6. Enforcement & Remedies
   - Maintainers reserve the right to suspend features, remove the bot from servers, or block users who violate these terms. For severe or illegal conduct we may report to Discord and/or law enforcement.

7. Intellectual Property
   - Tango, its assets, and code are owned by the maintainers unless explicitly licensed otherwise. You may not copy or redistribute the code or branding without permission.

8. Warranty & Liability
   - Tango is provided "as-is". Maintainers disclaim all warranties to the extent permitted by law. Maintainers are not liable for indirect, incidental, or consequential damages arising from use.

9. Changes to Terms
   - We may update these terms; continued use after changes indicates acceptance. Major updates will be announced when practical.

## Usage Policies
These policies explain how features should be used and what admins and members can expect.

1. Rate Limits & Abuse
   - Respect Discord rate limits and avoid automating excessive command usage. Do not implement loops or scripts that flood the bot with requests.

2. Moderation Tools
   - Tango provides moderation features (auto-moderation, bans, mutes, logs). Server moderators retain final responsibility for enforcement actions.
   - Automatic actions may be imperfect. Review logs and audit automated decisions before escalating.

3. Command Logging & Behavior
   - Some commands require inspecting or temporarily storing message content (for moderation, anti-spam, or context-aware features). Where possible, storage is minimized.

4. Custom Integrations & Bots
   - If you extend Tango with custom scripts or use third-party plugins, ensure they comply with these policies and applicable laws.

5. No Data Exfiltration
   - Do not use Tango to collect or exfiltrate sensitive information (credentials, private keys, financial data, health records) without explicit, lawful consent.

6. Developer & Operational Policies
   - Maintainers may disable features that cause instability, violate policy, or create legal risk. Feature rollout may be limited to reduce abuse.

## Data collection, storage & GDPR (detailed)
This section explains what data Tango may process, why, retention periods, and how we handle GDPR requests. These defaults may vary depending on hosting, region, or additional integrations.

1. Types of data collected
   - Identifiers: Discord server IDs, channel IDs, user IDs, and message IDs needed to perform features.
   - Message content: Messages inspected or flagged by moderation or anti-spam features. Only stored when required for functionality.
   - Usage logs: Command usage, timestamps, error logs, and aggregated analytics to monitor health and usage patterns.
   - Optional content: When a server enables features that store custom data (welcome messages, custom command data), that content is stored per server.

2. Purpose & lawful basis (GDPR)
   - Purpose: Provide bot functionality, moderation, abuse prevention, diagnostics, and feature improvement.
   - Lawful basis: processing is generally based on legitimate interests (maintaining service, preventing abuse) or consent where a user or server explicitly opts into a feature requiring extra data.

3. Retention periods (default)
   - Short-term logs (command and error logs): 30 days.
   - Moderation evidence (messages, flagged content): 90 days unless legal reasons require longer retention.
   - Backups and system snapshots: up to 180 days.
   - Aggregated, anonymized analytics: may be retained indefinitely.
   - Server-specific custom data: retained until removed by server owners or via deletion requests.

4. Data storage & security
   - Storage: Data is stored on the bot operator's hosting provider and may be processed in multiple regions depending on infrastructure.
   - Security: Reasonable administrative, technical, and organizational measures (encryption in transit, access controls) are applied. No system is perfectly secure; contact us if you suspect a breach.
   - Third parties: Some data may be processed by third-party services (hosting, analytics, crash-reporting). We use reputable providers and limit data shared to what is necessary.

5. Data sharing & legal disclosure
   - We do not sell personal data. We may disclose data to comply with legal obligations, respond to lawful requests, or protect rights and safety.

6. GDPR & EU data subject rights
   - If you are in the EU, you have rights including access, rectification, erasure (right to be forgotten), restriction of processing, data portability, and objection to processing.
   - To exercise your rights, contact support (see Contact below) and provide sufficient information (server ID, user ID, message IDs) to locate the data. We will respond within a reasonable timeframe and in accordance with applicable law (generally within 30 days).
   - Some requests may be limited where legal exemptions apply (e.g., to retain data necessary for legal defense, compliance, or detection/prevention of abuse).

## Moderation, enforcement & appeals
1. Enforcement actions
   - Actions include warnings, temporary or permanent removal of the bot from a server, or blocking a user from using the bot.

2. How to appeal
   - To appeal an action, contact support with:
     - Your server ID and name
     - A clear description of the issue and the action you are appealing
     - Relevant timestamps and message IDs
     - A preferred contact method
   - Provide evidence where possible. Appeals are reviewed by maintainers; timelines may vary.

3. Reporting abuse
   - To report abuse (illegal activity, CSAM, threats), provide message IDs, timestamps, and evidence. For emergencies or imminent threats, contact local law enforcement immediately.

## Contact
For support, data requests, or appeals, contact: support@tango-bot.com

---
This README is intended as a clear, practical summary and does not constitute legal advice. For jurisdiction-specific legal requirements (e.g., detailed GDPR compliance, CCPA, or other privacy laws) consult a qualified lawyer.

![GDPR Compliance badge](imgs/gdpr_compliant-1024x429.png)


## GDPR Notice

This project aims to comply with the EU General Data Protection Regulation (GDPR). The section "Data collection, storage & GDPR (detailed)" above describes the types of data collected, purposes, lawful basis, retention periods, and EU data subject rights. Below is a short summary and how to exercise your rights:

- Data controller: the bot maintainer/operator (contact: support@tango-bot.com).
- Data processed: identifiers (server, channel, user and message IDs), occasional message content for moderation/anti-spam features, command usage logs, and server-specific configuration data.
- Legal basis: legitimate interests (service operation, abuse prevention) or consent for optional features that require extra data.
- Exercising your rights: EU data subjects may request access, rectification, erasure, restriction, portability, or to object to processing. Provide server ID, user ID, and relevant message IDs where applicable. Requests will be handled in accordance with applicable law (generally within 30 days).
- Requests & complaints: to make a data request or complaint, email support@tango-bot.com. If unsatisfied, you may contact your local Data Protection Authority.

Note: Some requests may be limited where necessary to comply with legal obligations, ensure safety, or prevent abuse. For detailed GDPR compliance steps (data processing agreements, subprocessors, data transfer safeguards), consult a legal advisor or request more information from support.

