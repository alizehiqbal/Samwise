# SAMWISE

Samwise is an app that enables individuals with chronic illnesses to connect with patients like them, with similar conditions. Users can use the platform to ask questions and answer others' questions, engaging in a support network intended to make the journey through chronic illness a little more bearable. Patients are often the best experts of their diseases, and Samwise hopes someday to provide qualitative and quantitative data and information to providers in order to enhance quality and accuracy of care.  

## Background and Overview 

Chronic disease is a pervasive and expensive issue in the healthcare system. About half of US adults, or 117 million individuals, have at least one chronic disease, according to 2012 data from the Centers for Disease Control (CDC). This high volume of chronic illness accounted for approximately 86 percent of healthcare spending in 2010.

The management of chronic disease requires a suite of resources beyond just a physician's care, e.g. program adherence and behavioral/social support. Moreover, the majority of chronic diseases are either idiopathic (without a definitively proven cause) or lack a silver-bullet treatment/cure: much burden is placed on the patient to remain proactive and persevere through enduring, and often mystifying, symptoms. Samwise seeks to support a patient's journey to recovery by providing a resource for patients to ask questions, answer questions, and support others in their same boat.


Users can: 
  * Join groups by condition
  * Answer questions, ask questions
  * Query topics 
  * Provide support and encouragement to fellow patients
 
## Functionality and MVP

1. User Auth: 
  - [ ] user can sign up
  - [ ] user can log in
  - [ ] demo log in


2. Group:
  - [ ] User can create a new group and assign a user to be admin
  - [ ] User can join a grop
  - [ ] User can leave a group
  - [ ] Admin can delete the group
  - [ ] Admin can remove members from a group
  - [ ] Users can add others to group
  
3. Feed:
  - [ ] View posts/statuses of patient peers/follows
  - [ ] Post on feed page to have post visible in peers' feeds

4. Patient Recommendations:
  - [ ] user preferences questionnaire in user profile
  - [ ] user preferences calculated based on user behavior
  - [ ] recommend patient peers to follow based on similarity score between users

5. User profile 
  - [ ] list condition, symptoms, background
  - [ ] questions/interests of that user
  - [ ] contributions (user get a star every time they post) - works like Github green squares

6. Deploy to App Store
  - [ ] Apple App Store
  - [ ] Google Play Store
  
7.  Demo Page
  - [ ] has gif showing what the app does
  - [ ] has download link or QR code
  
8. Search
  - [ ] Users can search for groups with previously asked questions similar to their own.

9. Private Messaging
  - [ ] Users can directly message other patient peers.

10. Gratitude
  - [ ] Similar to a "like", users can click on an icon to say "thank you." 
  - [ ] Responses to questions/posts will be ordered such that those with the highest "gratitude score" appear first.
  

## Technologies 

Frontend: React/JavaScript 
Backend: Rails/Ruby 

Challenges include: 

  ### Recommendation Algorithm 
    In order to determine which patients should display in a user's recommended follows, and in what order, I will need to construct a sequencing algorithm similar, in a way, to a dating app's matching.  I will use linear regression modelling to account for factors that will weigh on a user's decision to select a peer, e.g. shared condition, activity patterns, age, and common connections. 
