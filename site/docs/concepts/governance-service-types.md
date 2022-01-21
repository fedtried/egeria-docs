<!-- SPDX-License-Identifier: CC-BY-4.0 -->
<!-- Copyright Contributors to the ODPi Egeria project. -->


There are seven types of governance services:

* [Open Discovery Service](open-discovery-service.md) for analysing the content of an [Asset's](asset.md) real-world counterpart in the digital landscape. (For example, if the asset describes a file, the discovery service analyses the data stored in the file).
  
* [Watchdog Governance Service](/egeria-docs/guides/developer/governance-action-services/watchdog-governance-service) for monitoring changes to open metadata elements and when certain changes occur (such as the creation of a new [Asset](/egeria-docs/concepts/asset)) the watchdog service requests action from other governance services by creating either a [Governance Action](/egeria-docs/concepts/governance-action), a [Governance Action Process](/egeria-docs/concepts/governance-action-process) or an [Incident Report](/egeria-docs/concepts/incident-report).
  
* [Verification Governance Service](/egeria-docs/guides/developer/governance-action-services/verification-governance-service) for testing the properties of specific open metadata elements to ensure they are set up correctly or do not indicate a situation where governance activity is required.  The [results](/egeria-docs/concepts/guard) returned from the verification service can be used to trigger other governance services as part of a [Governance Action Process](/egeria-docs/concepts/governance-action-process).
  
* [Triage Governance Service](/egeria-docs/guides/developer/governance-action-services/triage-governance-service) for making decisions on how to handle a specific situation or incident.  Often this involves a human decision maker.
  
* [Remediation Governance Service](/egeria-docs/guides/developer/governance-action-services/remediation-governance-service) for correcting errors in open metadata or the digital landscape it represents.
   
* [Provisioning Governance Service](/egeria-docs/guides/developer/governance-action-services/provisioning-governance-service) for configuring, enabling, provisioning resources in the digital landscape.  Often these provisioning services manage the cataloguing of new assets and the lineage between them.
  
* [Archive Service](/egeria-docs/guides/developer/archive-services/overview) for dynamically maintaining [open metadata archives](/egeria-docs/concepts/open-metadata-archive).

Related governance services are packaged together in a specific types of governance engine and enabled in one or more [Engine Host OMAG Servers](/egeria-docs/concepts/engine-host).  They run in the appropriate [Open Metadata Engine Service (OMES)](/egeria-docs/services/omes) as shown in the table below.

| Governance Service | Governance Engine type | Engine Service |
| :----------------- | :--------------------- | :------------- | 
| Open Discovery Service | [Open Discovery Engine](/egeria-docs/concepts/open-discovery-engine) | [Asset Analysis OMES](/egeria-docs/services/omes/asset-analysis/overview) |
| Watchdog Governance Service | [Governance Action Engine](/egeria-docs/concepts/governance-action-engine) | [Governance Action OMES](/egeria-docs/services/omes/governance-action/overview) |
| Verification Governance Service | [Governance Action Engine](/egeria-docs/concepts/governance-action-engine) | [Governance Action OMES](/egeria-docs/services/omes/governance-action/overview) |
| Triage Governance Service | [Governance Action Engine](/egeria-docs/concepts/governance-action-engine) | [Governance Action OMES](/egeria-docs/services/omes/governance-action/overview) |
| Remediation Governance Service | [Governance Action Engine](/egeria-docs/concepts/governance-action-engine) | [Governance Action OMES](/egeria-docs/services/omes/governance-action/overview) |
| Provisioning Governance Service | [Governance Action Engine](/egeria-docs/concepts/governance-action-engine) | [Governance Action OMES](/egeria-docs/services/omes/governance-action/overview) |
| Archive Service | [Archive Engine](/egeria-docs/concepts/archive-engine) | [Archive Manager OMES](/egeria-docs/services/omes/archive-manager/overview) |

--8<-- "snippets/abbr.md"