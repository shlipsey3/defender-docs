---
title: Microsoft Security Copilot Agents in Microsoft Defender
description: Learn about Security Copilot agents in Microsoft Defender that can help you perform your security tasks easily.
ms.service: defender-xdr
f1.keywords:
- NOCSH
ms.author: guywild
author: guywi-ms
ms.localizationpriority: medium
manager: deniseb
audience: ITPro
ms.collection: 
- m365-security
- tier1
- security-copilot
- magic-ai-copilot 
ms.topic: concept-article
search.appverid:
- MOE150
- MET150
ms.date: 09/17/2025
appliesto:
- Microsoft Defender XDR
- Microsoft Sentinel in the Microsoft Defender portal
#customer intent: As a security analyst, I want to know about the Security Copilot agents available in Microsoft Defender so that I can use them to perform my security tasks efficiently.
---

# Microsoft Security Copilot Agents in Microsoft Defender

[!INCLUDE [Microsoft Defender XDR rebranding](../includes/microsoft-defender.md)]

Microsoft Security Copilot agents are available in Microsoft Defender to help you perform your security tasks efficiently. Security Copilot agents are AI-powered assistants that can help you with various tasks by working seamlessly with Microsoft security products.

## Agents in Microsoft Defender

### Phishing Triage Agent

The [Phishing Triage Agent](phishing-triage-agent.md) helps security operations analysts to triage and classify user-submitted phishing incidents. The agent operates autonomously, provides a transparent rationale for its classification verdicts in natural language, and continuously learns and improves its accuracy based on feedback provided by analysts.

The agent autonomously analyzes the submitted email to classify them as either phishing or not phishing based on its training and the context of the organization. You must create the agent's identity and assign the appropriate permissions to the agent before starting the setup.

| Attribute | Description |
|---|---|
| Trigger | Triggered when a user in your organization submits a phishing incident |
| Permissions | Security data basics (read)<br>Email & collaboration content (read)<br>Email & collaboration metadata (read)<br>Security Copilot (read)<br>Alerts (manage) |
| Products | [Security Copilot](/copilot/security/get-started-security-copilot)<br>[Microsoft Defender for Office 365 Plan 2](/office365/servicedescriptions/office-365-advanced-threat-protection-service-description) | 
| Identity | Operates in the context of the identity you associate with it |
| Plugins | [Microsoft Defender XDR](security-copilot-in-microsoft-365-defender.md)<br>[Microsoft Threat Intelligence](/defender/threat-intelligence/security-copilot-and-defender-threat-intelligence)<br>[Phishing Triage Agent](phishing-triage-agent.md)|
| Role-based access | **Security Administrator** role is required to set up and manage the agent. Users with the same permissions as the Phishing Triage Agent can view the agent's activity and results, and provide feedback on the agent's classification verdict. |
 
