
# Inhouse-Project-Splunk-MCP-Via-Claude
I designed and implemented an AI-driven Security Operations workflow that integrates Splunk, Claude (via MCP), OpenAI, n8n automation, and Slack to create an autonomous SOC analyst capable of investigating, analyzing, and responding to security alerts in real time.  

Problem Statement

Traditional SOC environments suffer from:

High alert volume

Manual triage overhead

Slow investigation time

Analyst fatigue

This project was built to explore:

Can AI autonomously triage SIEM alerts?

Can LLMs convert raw logs into structured incident analysis?

Can automation reduce MTTR without removing human oversight?


Core Components
1️⃣ Splunk SIEM

Generates real-time alerts

Provides log data for investigation

Connected to Claude via MCP for contextual queries

2️⃣ n8n Automation

Listens for Splunk alerts (via webhook or API)

Formats alert payload

Sends structured data to OpenAI

Routes AI output to Slack

3️⃣ OpenAI – SOC Analyst Engine

Processes alerts and:

Classifies attack type

Assigns severity level

Maps to MITRE ATT&CK (when applicable)

Generates:

Incident summary

Timeline analysis

Root cause hypothesis

Mitigation recommendations

4️⃣ Claude + Splunk MCP

Allows natural language threat hunting:

Example prompts:

“When did this attack begin?”

“Show all failed logins from this IP.”

“Was lateral movement detected?”

“How should we mitigate this brute-force attack?”

Claude translates prompts into structured Splunk queries and returns contextualized results.

🤖 Agentic SOC Capabilities

Automated Level-1 triage

Attack classification

Log correlation

Threat hunting via natural language

Mitigation advisory generation

Slack-based SOC reporting
