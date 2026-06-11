# SCM Assistant – Supply Chain RAG Chatbot
 
## Overview
 
SCM Assistant is a Retrieval-Augmented Generation (RAG) chatbot built using Flowise Cloud. The chatbot answers questions related to supplier performance, supplier governance policies, risk assessment, compliance, disruption management, and procurement analytics by leveraging both structured CSV data and policy documentation.
 
 
---
 
## Public Chatbot URL
 
https://cloud.flowiseai.com/chatbot/5a0bcba0-405e-49c2-aa43-f96cd2a4dbd2
 
 
---
 
## GitHub Repository
 
https://github.com/akshat6749/scm
 
 
---
 
## Technology Stack
 
- Flowise Cloud
 
- Google Gemini 2.5 Flash
 
- Gemini Embedding 001
 
- Astra DB Vector Store
 
- Retrieval-Augmented Generation (RAG)
 
 
 
---
 
## Data Sources
 
### Supplier Performance Dataset
 
- 2,000 purchase orders
 
- 116 suppliers
 
- Supplier risk indicators
 
- Compliance metrics
 
- Defect rates
 
- OTD (On-Time Delivery) metrics
 
- Regional and category information
 
 
### Supplier Governance Policy
 
- Supplier tier definitions
 
- SLA requirements
 
- Compliance controls
 
- Watch list policies
 
- Disruption response procedures
 
- Regional concentration limits
 
 
 
---
 
## Chunking Experiments
 
### Configuration 1
 
Chunk Size: 1000
 
Chunk Overlap: 200
 
 
### Configuration 2
 
Chunk Size: 500
 
Chunk Overlap: 100
 
 
#### Configuration 1 produced more complete responses for policy-related questions and was selected for the final implementation.
 
 
---
 
## Validation Questions & Responses
 
#### Q1. Which Tier-3 suppliers have active disruption flags and what response level applies?
 
The chatbot identified 11 Tier-3 suppliers with active disruption indicators:
 
- Dravex Components India
 
- Plataforma Metales SA
 
- Maghreb Castworks
 
- Helios Pack Greece
 
- Cerromax Mineria
 
- Orinoco Pack SAPI
 
- Quetzal Textiles
 
- Sibertek Molding
 
- Archipelago PCB Corp
 
- Varna Electronics EAD
 
- Deltaforge Vietnam
 
 
According to the governance policy, these suppliers fall under the High-Risk category and require a Level-3 response process. This includes escalation to procurement leadership and shifting at least 40% of supply volume to approved alternative suppliers.
 
 
---
 
#### Q2. Which suppliers qualify for the Volume Rebate Program?
 
The chatbot found 19 suppliers eligible for the annual rebate initiative, including:
 
- Borealis Composites
 
- Crestline Chemical Supply
 
- Fenwick Alloy Solutions
 
- Hanguk Circuit Works
 
- Hokkaido Alloy Tech
 
- Krauss-Polymex GmbH
 
- Lakeshore Components
 
- Lumivex Semiconductor NL
 
- Maplewood Polymer Corp
 
- Norbec Alloy Works
 
- Nordloom Finland Oy
 
- Orrentek Precision Mfg
 
- Ostwind Composites AG
 
- PrecisionForge Taiyuan
 
- Solveig Eco Packaging
 
- Straits Packaging Hub
 
- Tasman Circuit Boards
 
- Toreval Electronics
 
- Valdoro Special Alloys
 
 
Eligibility requirements include:
 
- Tier-1 supplier classification
 
- OTD of at least 93%
 
- Defect rate below 0.5%
 
- Sustainability score of 85 or higher
 
 
 
---
 
#### Q3. Which region has the highest total purchase order value?
 
EMEA recorded the highest procurement spend, totaling approximately $193.99 million.
 
This represents roughly 48.5% of overall spending and exceeds the policy threshold of 45%, requiring the organization to initiate a diversification strategy within the defined policy timeline.
 
 
---
 
#### Q4. Which suppliers are on the Supplier Watch List (SWL)?
 
The chatbot identified 11 suppliers with compliance scores below the acceptable threshold:
 
Deltaforge Vietnam
 
- Maghreb Castworks
 
- Helios Pack Greece
 
- Cerromax Mineria
 
- Orinoco Pack SAPI
 
- Varna Electronics EAD
 
- Quetzal Textiles
 
- Plataforma Metales SA
 
- Archipelago PCB Corp
 
- Dravex Components India
 
- Sibertek Molding
 
 
Under SWL rules, new purchase orders are restricted to 20% of the supplier's previous-quarter volume until performance improves.
 
 
---
 
#### Q5. Which product category has the highest average defect rate?
 
Mechanical Components showed the highest average defect rate at approximately 2.12% across the dataset.
 
Although it remains below the Tier-2 policy limit of 2.50%, it is approaching the threshold and should continue to be monitored.
 
 
---
 
## Deliverables
 
✔ Flowise Chatflow Export (scm_assistant.json)
 
✔ Public Chatbot Deployment
 
✔ Screenshots of Implementation Steps
 
✔ README Documentation
 
✔ Source Code Repository
 
✔ Configuration Details
 
 
---
 
## Future Improvements
 
- Hybrid search combining metadata filtering and vector retrieval
 
- Structured querying for CSV analytics
 
- Supplier trend dashboards
 
- Real-time supplier monitoring
 
- Enhanced policy citation support
 
- Advanced risk forecasting and alerting
 
 
 
---
 
## Author
 
Akshat Jaiswal
