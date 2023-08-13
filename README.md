# notes-sc-400
A mindmap for SC-400 Microsoft Information Protector Administrator using markmap
# Introduction to information protection and data lifecycle management in Microsoft Purview
## Know your data
Data classification
- Sensitive information types
  -  a pattern that can be identified by a *regular expression* or *function*
- Trainable classifiers
  -  trainable classifiers, use artificial intelligence and machine learning, training a classifier to identify an item based on what the item is, not by elements that are in the item
- Labels
  - Manual labeling on all platforms
  - Automated labeling in Office for the web and Windows
  - Automated labeling on content stored in OneDrive, SharePoint, and Exchange
- Policies
   - Sensitivity label policies
   - Data loss prevention (DLP) policies
   - Retention policies and retention label policies
## Protect your data
### data loss prevention (DLP) solution
- Data source `which user can share what`
- Data destination `who to share with`
- Amount shared `single credit card number vs 1000`
- Exposure impact `prompt the user with a tool tip to educate them about the consequences`
## Govern your data
Data Lifecycle Management
Records management
- Streamlined administration `one policy across multiple services`
- Automation at scale `policy work automatically and applied organization-wide`
- Tailored workflows `custom events: eg departure of an employee`
# Classify data for protection and governance
## Sensitive information types (SIT)
- Built-in SITs `such as social security numbers, credit card numbers, and email addresses, can't be edited, can serve as templates for creating custom sensitive information types`
- Named entity SITs `such as person names, physical addresses, or medical terms and conditions, predefined and can't be edited or copied`
- Custom SITs
- Exact data match (EDM)-based SITs `built from scratch`
### SIT consists
- Name
- Description
- Pattern
  - Primary element
  - Supporting element
  - Confidence Level
  - Proximity
### Creation
`By UI, EDM, Powershell`
## Classify data using trainable classifiers
- Pre-Trained Classifiers
- Custom Trainable Classifiers `A one-time scan must be completed before creating any custom trainable classifiers. This process takes 7 to 14 days.`
  - Seed
  - Test
  - Publish
## Review sensitive information and label usage
![The Overview page](/figs/data-classification-overview.png)
