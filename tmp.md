1. no auto, no empty policies for  
2. Cloud App Security currently supports applying Azure Information Protection classification labels for the following file types: Word, Excel, PowerPoint, PDF, The policy will classify only 100 files daily.
3. The max size for the OME encryption functionality is 25 mb and all file extension are not covered by the OME encryption. You can only encrypt docx files, powerpoint files and excel files. The following are the one supported,
Old file extension such as xls, doc and ppt are not supported.
5. You cannot apply watermarks to email, so the header will only get applied.
But you can for sure add both watermarks and headers to documents located at Sharepoint.
6. You can create a sensitivity label named Passport Number and configure it to apply encryption and a watermark to the content. You can also choose to restrict access to specific users or groups, or block external sharing.
You can create an auto-labeling policy named Passport Number Policy and select the Passport Number label to apply automatically. You can also choose the locations where you want to apply the policy, such as Exchange Online, SharePoint Online, and OneDrive for Business. You can then define a condition to match the content that contains passport numbers from the United States, Germany, Australia, and Japan.
7. Sublabels don't inherit settings from their parent label
, when you remove a label that applied encryption to a document you don't necessarily remove the encryption.
8. Resumes, Source code, Harassment, Profanity, Threat are pre-trained classifiers that exist already in Microsoft 365 -> Source code is correct
9. NEW tenant - Global admin is required to opt in
    While Compliance Administrator role is required to train a classifier
11. Create a trainable classifier: 
    - Collect between 50-500 seed content items.
    - Place the seed content in a SharePoint Online folder that is dedicated to holding the seed content only.
    - Sign in to the Microsoft Purview compliance portal with either Compliance admin or Security admin role access and navigate to Data classification > Classifiers.
    - Within 24 hours the trainable classifier will process the seed data and build a prediction model. 
    - Collect at least 200 test content items (10,000 max) for best results.
12. You should run the New-OMEConfiguration cmdlet to create a new OME configuration. Then, modify the branding template using Set-OMEConfiguration cmdlet. OME(Office Message Encryption), Information Rights Management (IRM)
13. You can upload data with the EDMUploadAgent to any given data store only twice per day. EDM(Exact Data Match)
14. you should create a mail flow rule that applies the Encrypt action to all email messages sent to fabrikam.com. You can use the Apply this rule if… condition to specify the recipient domain. (needs recheck)
15. you cannot modify a policy template in MCAS. You can create policies from policies templates. (nice question)
16. Unlike manual labeling or auto-labeling with Office apps, PDF attachments as well as Office attachments are also scanned for the conditions you specify in your auto-labeling policy. When there is a match, *the email is labeled but not the attachment*.
17. The keywords for your dictionary could come from various sources, most commonly from a file (such as a `.csv` or `.txt` list) imported in the service or by PowerShell cmdlet.
18. You can revoke a mail that you sent to a single recipient that uses a social account such as gmail.com or yahoo.com. In other words, you can revoke an email sent to a single recipient that received the link-based experience.
You cannot revoke a mail that you sent to a recipient that uses a work or school account from Office 365 or Microsoft 365 or a user that uses a Microsoft account, for example, an outlook.com account.
19. (outdated)
20. (outdated)
21. Mail Flow rule will fit the bill.
22. requires revisit
23. https://www.examtopics.com/discussions/microsoft/view/64731-exam-sc-400-topic-1-question-23-discussion/
24. 
    