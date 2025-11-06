```markdown
<p align="center">
  <img src="assets/tango-logo.png" alt="Tango Logo" width="140" />
  &nbsp;&nbsp;
  <img src="assets/gdpr-badge.png" alt="GDPR Compliant Badge" width="220" />
</p>

# Tango — Discord Moderation Bot
Tango is a lightweight, privacy-first Discord moderation bot that helps server staff keep communities safe and civil. It scans messages where it has permission and performs configurable moderation actions, logging, and audits for transparency.

Effective date: 2025-11-06

---

## Quick Links
- Invite the bot: (add your invite link here)
- Support & data requests: https://github.com/mediumwarrior67/Tango---Terms-Of-Service-Usage-Policies/issues
- Source & contribute: https://github.com/mediumwarrior67/Tango---Terms-Of-Service-Usage-Policies

---

## Key Features
- Real-time message scanning and auto-moderation
- Moderation commands: ban, kick, mute, warn, etc.
- Configurable filters (profanity, spam, links, invites)
- Short-term message logging for moderator review (14-day retention)
- Audit logs and transparency tools
- GDPR-aware data handling and user rights

---

## Installation (Quick Start)
1. Clone the repo:
   - git clone https://github.com/mediumwarrior67/Tango---Terms-Of-Service-Usage-Policies.git
2. Install dependencies:
   - npm install
3. Create a `.env` file with your Discord bot token and configuration variables (see config.example or bot code).
4. Create an `assets/` directory and add the provided images:
   - assets/tango-logo.png
   - assets/gdpr-badge.png
5. Run the bot:
   - npm start

---

## Data, Privacy & Usage Policy (Terms of Service / TOS) — Summary
By inviting Tango to your server you accept these Terms for data processing performed by the bot on that server.

- What we collect: Discord user IDs and messages the bot can access.
- Why we collect it: moderation, logging, and moderator review.
- How long we store it: up to 14 days (two weeks).
- GDPR: Tango follows GDPR principles and supports data subject requests.

Full details follow in the Data & Privacy section below.

### What data Tango collects
- Discord user ID (for mapping actions and logs to users)
- Message content and metadata (only from channels where the bot has read/view permission)

No other personal data is intentionally collected (no emails or IP addresses by the bot itself).

### Purpose of collection
- Moderation: filter policy-violating content, detect spam, and enforce rules.
- Logging: create temporary logs for moderator review and appeals.
- Diagnostics: minimal metadata for troubleshooting.

Tango will not use message content for model training, analytics, or third-party processing without explicit per-server opt-in.

### Retention policy
- Messages and moderation logs are retained for up to 14 days from collection.
- After 14 days, message contents are deleted from active storage. Audit metadata (timestamp, action, moderator, short reason) may be retained longer for accountability but will not include full message content unless required by law.
- If required by lawful request, minimal required data may be retained; server owners will be notified where permitted.

### Storage & security
- Data is encrypted in transit and encrypted at rest where possible.
- Access is restricted to the bot process, designated server moderators (for their server) and authorized maintainers for troubleshooting.
- Data minimization: only data necessary for moderation is stored.

### GDPR and Data Subject Rights
EU data subjects may request:
- Access to data
- Rectification
- Erasure (subject to retention policy)
- Restriction of processing
- Data portability (where applicable)
- To object to processing

To exercise these rights: open an issue at the repo with your Discord user ID and request type. Mark urgent requests with “URGENT”.

### Opt-in for improvements
- By default, message content is not used externally.
- Explicit per-server opt-in will be requested for anonymized samples used to improve moderation heuristics.

### Third parties and sharing
- Tango will not sell your data.
- Data may be shared only when required by law, to protect rights/safety, or with explicit opt-in.
- Hosting/database providers used by the bot are expected to meet reasonable data protection standards.

---

## Usage Policies (Acceptable Use)
- Permitted:
  - Moderation and logging on servers where the bot has permission.
  - Server-level configuration of filters and retention within supported options.
- Prohibited:
  - Using Tango to collect data unrelated to moderation (advertising profiling).
  - Sharing raw message contents with third parties without consent.
  - Bypassing, tampering with, or disabling retention/deletion mechanisms.

Server owners must ensure they have the legal authority to run automated moderation tools in their community.

---

## Command Reference — Configuration & Moderation Examples
Tango supports both slash and prefix-style commands depending on server configuration. Replace placeholders like #mod-logs or @Moderator with your server-specific names.

Core commands:
- /tango help
  - Usage: /tango help
  - Description: Display help and command list.

- /tango status
  - Usage: /tango status
  - Description: Shows bot status, uptime, and current retention setting.

- /tango config set retention <days>
  - Example: /tango config set retention 14
  - Description: Set message retention in days (default: 14). Note: changes apply to future stored messages; previously stored data follows its original retention schedule.

- /tango config set logs_channel <#channel>
  - Example: /tango config set logs_channel #mod-logs
  - Description: Where moderation logs are posted.

- /tango config filter add <type> [sensitivity]
  - Example: /tango config filter add profanity high
  - Description: Add a content filter (profanity, spam, links, invites) and optional sensitivity level.

- /tango filter remove <type>
  - Example: /tango filter remove invites
  - Description: Remove a configured filter.

Moderation actions (moderator-only):
- /tango mod warn <@user> [reason]
  - Example: /tango mod warn @troublemaker “Repeated profanity”
  - Description: Issue a warning and log the event.

- /tango mod mute <@user> <duration>
  - Example: /tango mod mute @troublemaker 1h
  - Description: Temporarily mute a user.

- /tango mod ban <@user> [reason]
  - Example: /tango mod ban @troll “Harassment”
  - Description: Ban a user and log the reason.

Audit & retrieval:
- /tango audit fetch <messageID>
  - Example: /tango audit fetch 123456789012345678
  - Description: Retrieve moderation event details and stored message snippet (if within retention period).

Logs & exports:
- /tango logs export <start_date> <end_date>
  - Example: /tango logs export 2025-10-01 2025-10-31
  - Description: Export audit logs for a date range (server moderator only). Exports follow the same data minimization rules.

Notes:
- Only server moderators and administrators can change retention or export logs.
- Commands may vary slightly depending on bot version and server configuration. Use /tango help or the bot’s command list to confirm exact syntax.

---

## How to Request Data Access, Correction, or Deletion
1. Open an issue: https://github.com/mediumwarrior67/Tango---Terms-Of-Service-Usage-Policies/issues
2. Include:
   - Discord user ID (required)
   - Request type: access / delete / correct
   - Any relevant dates or message IDs (if known)
3. We will acknowledge and process the request in a timely manner. Urgent requests: mark the issue title with “URGENT”.

---

## Admin Controls & Per-Server Settings
- Server owners can configure filters, log channels, retention, and sensitivity through commands or the web dashboard (if available).
- For per-server adjustments outside GUI/commands, contact the maintainer and include server ID and justification.

---

## Contact & Support
Repository owner / bot maintainer: mediumwarrior67  
Support & data requests: https://github.com/mediumwarrior67/Tango---Terms-Of-Service-Usage-Policies/issues

---

## Contributing & Responsible Disclosure
Contributions, feature requests, and bug reports are welcome. When contributing examples or logs, remove/anonymize personal data unless you have permission. For privacy/security issues, open a “security” issue or contact the maintainer directly.

---

## Changelog
- 2025-11-06 — Updated policy language, added GDPR summary, clarified retention and commands.

---

## License
Choose a license (MIT, Apache-2.0, etc.) and include it here.
```
