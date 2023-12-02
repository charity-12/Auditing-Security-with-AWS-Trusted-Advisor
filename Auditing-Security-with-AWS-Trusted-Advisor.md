

# Auditing Your Security with AWS Trusted Advisor

# Introduction
cat <<EOF
I embarked on a hands-on project as part of a free lab provided by AWS. This project aimed to offer practical experience and insights into AWS resources and best practices. Through a series of tasks and challenges, I delved into AWS Trusted Advisor, Amazon EC2 Security Groups, and the implementation of Multi-factor Authentication (MFA). These hands-on activities not only enriched my understanding of AWS but also allowed me to put theory into practice, improving my skills and knowledge in cloud management and security.

Amazon Web Services (AWS) is a global leader in cloud computing, offering a multitude of powerful and versatile services. However, the power and versatility of AWS come with a corresponding need for diligent security measures. AWS Trusted Advisor is a fundamental tool in your arsenal for achieving this goal.

AWS Trusted Advisor is an intelligent service that assesses your AWS environment, analyzing configurations and usage patterns. It identifies areas where security might be compromised, cost optimization could be achieved, performance could be enhanced, and fault tolerance could be increased.
EOF

# Objectives
cat <<EOF
Objectives:
• Use Trusted Advisor to perform a basic audit of your AWS resources
• Modify Amazon Elastic Compute Cloud (Amazon EC2) Security Groups to meet best practices
• Configure Multi-factor Authentication (MFA) (Optional, requiring installation of software on a mobile device)
EOF

# Task description
cat <<EOF
Task description:
Task 1: Check recommended actions with Trusted Advisor
1. Accessed the AWS Management Console and used the search bar to look for 'Trusted Advisor.'
2. Selected the Trusted Advisor service from the list of search results.
3. On the Trusted Advisor Recommendations page, I reviewed the Checks summary and the list of Recommended Actions, which are based on pre-defined checks for the AWS account. These recommended actions are categorized into three types:(Red) Critical – Action recommended (Orange) Investigation recommended (Green) No issues or concerns found
4. To gain further insights, I expanded each AWS Trusted Advisor check and examined the details. If there were items that were not green, I reviewed the criteria for the status and considered the provided Recommended Actions.

Task 2: Modify security groups with unrestricted ports
1. In the Trusted Advisor navigation pane on the left side of the page, I chose 'Security' under the 'Recommendations' menu.
2. Under the 'Checks' section, I expanded 'Security Groups - Specific Ports Unrestricted."
3. In the 'Security Groups' table at the bottom of this section, I identified the Security Group(s)
marked as "Red" in the Status column.
4. One of the items listed indicated that there was an unrestricted protocol/port (tcp/port 21). I received information from the security staff that this port was not currently needed and should be removed from the rules.
5. To locate the item that contained "tcp" in the Protocol column and "21" in the From Port column, I looked through the list. If I couldn't find the item with "tcp/port 21," I refreshed the "Security Groups - Specific Ports Unrestricted" item using the provided button.
6. Once I found the item, I chose the "WordPress Security Group" link to open the Security Groups page.
7. On the Security Groups page, I selected the "Inbound rules" tab.
8. Then, I clicked "Edit inbound rules" and followed these sub-steps:
For the rule related to port 21, I selected "Delete" to the right of the rule.
Finally, I selected "Save rules" to apply the changes.
EOF
