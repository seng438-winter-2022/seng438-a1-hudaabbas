>   **SENG 438 - Software Testing, Reliability, and Quality**

**Lab. Report \#1 – Introduction to Testing and Defect Tracking**

| Group \1:       |              |
|-----------------|--------------|
| Student Names:  | Rajpreet Gill (30086659)|
|                 | Nuha Shaikh (30084641)  |
|                 | Huda Abbas (30087827)   |
|                 | Lubaba Sheikh (30090885)|

**Table of Contents**

(When you finish writing, update the following list using right click, then
“Update Field”)

[1 Introduction	1](#_Toc439194677)

[2 High-level description of the exploratory testing plan	1](#_Toc439194678)

[3 Comparison of exploratory and manual functional testing	1](#_Toc439194679)

[4 Notes and discussion of the peer reviews of defect reports	1](#_Toc439194680)

[5 How the pair testing was managed and team work/effort was
divided	1](#_Toc439194681)

[6 Difficulties encountered, challenges overcome, and lessons
learned	1](#_Toc439194682)

[7 Comments/feedback on the lab and lab document itself	1](#_Toc439194683)

# Introduction

We all understood that exploratory testing entailed conducting various tests manually and without a pre-planned script. Precisely, this type of testing consists of executing the test cases once, unless a defect is identified, the tests may be repeated. Further, we understood that exploratory testing is unstructured and, as a result, is frequently criticized. However, this can be viewed as an advantage to this type of testing. It allows testers to focus on finding the major issues within the program and motivates testers to test various program functionality. The team also understood that exploratory testing differs from regression testing in that the latter focuses on a specific issue with detailed steps on how to replicate the problem. In contrast, exploratory testing is more flexible and does not necessarily focus on the replication steps of a particular situation.

In terms of the manual functional testing, we all had an understanding that this type of testing entailed greater detail and attention towards designing the test cases before the execution steps were conducted. In contrast to exploratory testing, one criticism towards manual functional testing is that it restricts the tester’s mind and prevents them from using their creativity to test various software program functionality. Despite this, we all understood the benefits of manual functional testing, such as how it allows test cases to be readily replicated as the replication steps are recorded to create the same fault again in the program.


# High-level description of the exploratory testing plan

We intend to test the system using a general approach by targeting the main functions specified in the general requirements and looking for non-expected functionality.

The following is a general list of the functions we will look to target:
All four transactions
Transfer of money between any two accounts linked to the card
Withdraw cash from any suitable account linked to the card in multiples of \$20
Deposit to any account linked to any card
View any balance inquiries for each account
The system should tell the user whether their credit card PIN is correct or incorrect
Be able to abort a transaction in progress by pressing Cancel
The operator must be able to system startup and shutdown

In general, the approach we are taking is that we will look to try to test most functions a little bit to get a general idea of the entire system. By testing every account type and card combination for all the tasks mentioned above, we hope to catch most bugs by getting a general idea for the majority of the possible functionality. We checked all messages displayed by the ATM for invalid inputs, error messages, receipts, and balance amounts for all functions.

When coming up with test cases, we want to find bugs that most users are likely to encounter; therefore, testing the basic functionality using the most common paths is where we started. After thoroughly testing common pathways and the basic functionality, we will try distinctive approaches, including edge or boundary cases. This is where we are likely to find more failures and defects, like selecting an account type that isn’t associated with a specific card.


# Comparison of exploratory and manual functional testing

Benefits: The benefits of exploratory testing compared to manual testing is that the latter consists of being extremely familiar with the system's requirements. It requires an in-depth understanding of all the functionalities that the system must carry out to allow for further replicating of tests. The exploratory testing step allowed us to develop a testing plan that the testing team can follow, including the functions being tested, the approach to be taken when trying them, and a method to come up with the test cases. This allowed us to initially explore the ATM system without a pre-planned script. A big benefit of starting with exploratory testing, especially for a system that we have never used before, is that freely trying different functionalities allowed us to become familiar with the application so we could truly grasp the requirements more and more as time went on. Manual scripted testing enabled us to perform the tests systematically, covering all the functionalities with steps on how to recreate them, making it a more rigorous and detailed form of testing. With manual testing, we were able to easily delegate and perform tests using a clear testing suite, which saved time and resources ensuring there was no duplication of tests.

Trade-Offs: Manual scripted testing is more effective and efficient since it outlines steps to recreate each functionality that the QA team could test. However, with that comes the trade-off of a strict testing suite that can fail to uncover some of the more exceptional pathways that exploratory testing may uncover. A given testing suite restricts the ability to find any bugs other than the set ones outlined in the test cases. Exploratory testing allowed us to find more bugs in the system due to its flexibility, which we did not see through manual scripted testing however it was ineffective since it was more of a trial and error approach for testing the system's functionality. Without a clear testing plan and with many team members working on the same application we found that there was some duplication of tests and an overlap in defects found. At times it was also difficult to trace back and replicate the steps once a bug was found, as a combination of a lot of previous steps could have been performed which were not systematically thought out before being performed, so it relied on good memory to be able to document the bug. The ad-hoc approach definitely affected the conciseness of our reported defects, as later on when looking at the provided test cases, some of our bugs documented were actually a combination of a few smaller test cases from MST.

Effectiveness: Since exploratory testing was our initial trial and error phase of executing tests during a 30-minute time frame, this made it less effective. With only a high-level testing plan, a lot of the time spent during exploratory testing was reviewing the bugs found and removing duplicates before reporting them. Additionally, because exploratory testing was performed first and we were still getting familiar with the ATM system a lot of the time spent during our tests was double-checking the requirements in turn making it less effective. However, in the end we did uncover quite a few defects from exploratory testing so it proved somewhat effective, it just required more time and review. Manual scripted testing allowed for a systemic approach when tackling all the system's functionalities. It had initial states and steps to reproduce the errors with expected outcomes outlined, which produced more effective test cases. However, due to the restrictive nature of MST some of the bugs discovered in exploratory testing were not outlined in the test cases and therefore missed. When comparing effectiveness it all comes down to the provided testing suite versus the thoroughness of one’s exploratory testing. The more effort and time given to exploratory testing the more effective it may become. We tried all combinations of accounts and cards for almost every type of function, therefore uncovering a lot of the same defects found with MST but in a longer amount of time. Whereas a given testing suite will always have the same effectiveness no matter the person reproducing the test, as all test cases are clearly outlined and already set.

Efficiency: Manual scripted testing was more efficient since it clearly had the steps to recreate each functionality, allowing us to perform the tests in a more scripted manner. This made each test case more replicable with the provided expected outcomes. Additionally, with four team members and a given test suite, we were able to quickly divide and conquer the provided test cases by executing them in groups of ten. This methodology did however affect the order of tests, as test cases 1 to 40 were not all performed in sequential order at once and instead 1 to 10, 11 to 20, 21 to 30, and then 31 to 40 were performed in separate systems. Exploratory testing was overall more inefficient compared to MST because both groups found the same errors, which led to repetitive test cases and it took a longer time to uncover some of the same defects due to this overlap.



# Notes and discussion of the peer reviews of defect reports created by each pair in a group.

During the peer testing that was conducted, one person focused on performing the tests while the other focused on analyzing and reviewing the tests that were performed. During the discussion of the defect reports created by each group, we had to ensure there were no repetitive tests being reported on the backlog by both groups. Some notes that were recorded from the analyzer during the tests consisted of comments on clarifying the initial state of the system in the defect reports, writing a clearer summary and including further information on the exact input for recreation purposes. When reviewing the defect reports, we also noticed that some of the test cases could be broken down into two separate bugs due to its complexity and interference with other functionalities. We also recognized the value communication held as both pairs ensured to update each other about the specific test cases performed, results obtained, and any technical issues encountered. The peer review method also worked quite well for our group as we all took equal responsibility in our work and performed the tasks associated with our role.


# How the pair testing was managed and team work/effort was divided 

Text…

# Any lessons learned from your teamwork in this lab?

As a group, we could replicate how a QA team would work in a natural work environment, providing valuable real-world experience for when we enter the job market. We learned that it was more time-efficient to break up the various functionalities of the system between the two pairings when it came to exploratory testing. This way, we covered all potential bugs in the system through a divide and conquered method. However, this did result in some overlap of the bugs found, which was an ineffective use of our time. For manual scripted testing and regression scripted testing, we divided the functionalities being tested; thus, none of the team members duplicated the work, which is essential in an efficient work environment. A big lesson we learned was distributing and delegating work for the team's efficiency effectively. We found that the team very much exercised our leadership skills during this lab since we all had to take charge of our responsibilities and work together to ensure that the group was on track. Furthermore, as a team, we learned about the importance of communication when clarifying tasks to ensure everyone is on the same page. With some of the confusion we had with the steps outlined in the lab document, as a team, we came together to discuss and conclude what our next steps were.

# Difficulties encountered, challenges overcome, and lessons learned

One of the difficulties we encountered when performing this lab was that with a team of four busy individuals, it was challenging to find the time for all of us to meet, come together and discuss our progress, difficulties that each member had while working through their components and things we needed to accomplish next. We overcame this by sharing our respective calendars to find times that worked for all of us effectively and efficiently.

We also had some difficulty following some of the instructions in the lab document as each of us had different interpretations of some of the steps, which caused some division in the team. We overcame this by having a civil discussion about our thoughts, and after this, we were able to come to a common ground. We learned that it is essential to communicate effectively and listen to everyone's opinions to ensure the whole team's success.

Additionally, we did encounter some difficulties when first using the Backlog program. When using a new application, there is always a learning curve to get used to the functionality and instructions. When creating our groups and team login, we ran into some challenges in the signup process as we did not have a group number. It was challenging to understand which log in to use, where to see our issues when initially creating them, and how to assign different versions. In the end, after some trial and error as a team, we figured it out and got familiar with the defect tracking system.


# Comments/feedback on the lab and lab document itself

The lab document was comprehensive and easy to follow, especially when including images and examples along the way. It was a bit long, but we feel all the sections provided clarity and needed a better background and understanding of the lab. Some parts of the document were a little harder to follow due to some ambiguous language, but after consultation with TAs, the TA's cleared up our questions. The steps for regression testing were slightly hard to follow; thus, a suggestion for future labs is that it may be of interest to clarify a few of those steps to ensure our Backlog project follows what is asked.

The lab itself was beneficial; utilizing Backlog made the lab a lot more engaging and realistic. Executing the three different types of testing strengthened our knowledge of the differences between exploratory, manual scripted, and regression testing by allowing us to test the ATM system in a hands-on environment interactively. Using an industrial tracking system and getting familiar with reporting the issues was an extremely vital practice. It could have also been very beneficial for the lab to collaborate with an entirely different group to see how different exploratory testing plans may uncover various defects that others could have missed.

