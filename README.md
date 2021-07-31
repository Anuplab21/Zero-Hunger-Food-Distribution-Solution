# Caliber 2021-ZERO Hunger Solution


Contents
Background	2
Idea	2
Solution Architecture & Functional Understanding	3
UI Design	3
Transaction Flow	3
Solution Development Roadmap	4
Feature Developed	4
Feature of future scope	4
References	4




# Summary of changes
Date	Author	Description
31-Jul-2021	Anuplab Chatterjee (Cognizant)
Shitlesh Bakshi (Cognizant)
Pranab Sasmal (Cognizant)	Document created
 

# Background
Hunger and Malnutrition is one of the greatest challenges in our time. Although the reason for such crisis are many, but availability or reachability of food to the needy people on the ground is one of major problem which greatly influences the Hunger crisis.
However, there are numerous voluntary or pro-active donations are available which requires technology-based system to connect with NGO/ any such organization who work for needy people for food distribution.
Therefore, there is need of IOT based system, establishing integration of different stakeholders – Donors and NGO/ Social Organization so as demand and supply chain is enabled to reach the foods to needy on the ground.

# Idea
To establish Technology-based solution to connect food supply and demand, UI based system to be developed which is named as ZERO HUNGER FOOD DISTRIBUTION SOLUTION.

This is UI based solution developed using Node-Red, available for both users – Donors (i.e., Provider) and NGO/ Social Organization (i.e., Consumer). Donation of food can be posted by donors in system so that Consumer can check and fetch the food items distributing the needy people. Thus, it ensures the highest possibility of food reachability at ground level needy people and off course, making supply more possibility highest.

•	Donors (Provider) – Represents any Individuals or organization or institutes who are interested to donate food for needy people, can post their donation in the system. Once, donation is posted in system, SMS notification will be sent to System admin.
•	System Admin – Represents owner of the site/ system who will authenticate the donation post and approve the request for back-end. Admin will receive SMS notification about the donation post i.e., Supply and delivery/ dispatch of food items.
•	NGO/ Social Organization (Consumer) – Represents NGO or any organization who work for noble cause in distributing the foods to needy people, they can see the food availability and accordingly, food items can be fetched for distribution.

 
# Solution Architecture & Functional Understanding

 
# UI Design
 

# Transaction Flow

1.	Provider/Donor will submit their food item Mobile Application or Website using their registered phone number. Provider/Donor will be having option to donate their food items anonymously. 
2.	System will trigger SMS function to Twilio Programming Message service for notifying System admin
3.	System admin will review the post and approve after the authentication of the post
4.	Approved post will be displayed in Consumer UI so that consumer can procure the food items
5.	After procurement, consumer will update the status and the donation is completed
6.	Donation records in system will flow with following logic
-	Submit fresh donation request – status is Pending and SMS will be sent to system admin
-	System admin will update status by approving and status is changed to “Approved”
-	“Approved” transaction will be displayed in Consumer page for procurement
-	After procurement, transaction status will be updated to “Transacted”
-	“Transacted” records will be considered as complete transaction i.e., donation has reached to needy people.

Solution Development Roadmap
Feature Developed
1.	Donation submission & SMS notification to admin
2.	Transaction approval through manual (by patching data from backend)
3.	Donation transaction display rule in respective pages – Consumer, Donor and System pages based on transaction status
4.	Transaction summary chart in respective pages.

Feature for future development
1.	UI enhancement for system admin to approve transaction
2.	Consumer page enhancement to block donation transaction for procurement
3.	SMS to system by Consumer after food distribution and BRE for updating transaction status to “Transacted”

# References
Code repository: https://github.com/Anuplab21/Zero-Hunger-Food-Distribution-Solution

