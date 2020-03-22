# Interview Script

There is a moderator, interviewee, and listeners

1.       The moderator announces
á         the meeting title
á         the date and time of the meeting
á         that the meeting is being recorded for transcription purposes only
á         that the recording will be destroyed after 30 days

2.  Ask the attendees to announce their names and acknowledgment of being recorded.
3. Moderator hits *22 on conference line to start recording. (also pauses)
3. Moderator recaps purpose of the meeting: to gain more insight into architectural technical debt.

# Guidance for the interviewer
* Focus on examples where choices are deliberate, known or had some way of being informed of the problem
* Steer away from examples where whole context is changing
* During our interviews should we be listening for an opportunity to examine artifacts to see what portion of the Òdesign shortcuts with architectural implicationsÓ are represented in what they track and what impact do they have that the tool doesnÕt show (since all debt is treated equally).

# Context setting
Pre-interview, look for interviewee's responses to survey to confirm a) we have the data and b) what his/her context is.

If no answers exist or cannot be retrieved, go over survey questions on background questions 5-9.
5. What is size of system in LOC?
6. What is age of system, beginning from initial design?
7. What role do you play on the project?
8. How many FTEs are involved in project including non-technical staff?
9. What type of system is this? (Web site, real-time, IT, Integration, Data analysis)

Remind that we are referring to a given system (from survey) when answering specifics.

# Questions
1. Recall that technical debt was defined as a choice that is expedient in the short term but that creates a technical context in which the same work will cost more to do later than now. Our survey responses suggested design decisions (incl architectural decisions) can be a major cause of technical debt. Can you describe, as specifically as possible, one example of  a design decision that resulted in rework, higher than average bug rate, or other problems? DonÕt include cases where requirements changed later (if they do, get into why they think that is relevant - see 9 below)

As they discuss the example, explore the following, and as needed ask to expand on how/why they consider that TD:

2. If this was not answered in example description, how and when did this problem arise? What was the symptom or indicator? Was it a deliberate decision or not?
3. If the example is not allowing for understanding of architectural decision involved (too vague or unclear),
What subsystems or components were impacted by the change or by deferring work or ask about the quality of the code/programming see if that leads back to architecture.
4. Was there a quality attribute-related impact (modifiability, performance, scalability, etc.)?
5. Was there any value from the TD?
a. If so, how was it captured?
6. What tools and/or artifacts are used for technical debt tracking for this example?
a. Static Analysis tools
b. Defect tracker
c. Code comments
d. Change Management tools
e. Etc.
7. Do these tools effectively monitor for these issues?
8. We might say that ÔinterestÕ on TD is the extra cost associated with TD-laden code. For example, a defect density above average, code that takes longer to understand. Given these interest indicators, what ones would identify interest problems on your project?
9. Are you able to measure or monitor for indicators for the example described above, and if so what data did you use?  If you cannot, what would be useful if you had it?
10. We asked you for an instance of deliberate technical debt. What would you say is more important/significant/problematic: deliberate shortcuts or unintentional or accidental choices?

# Other questions if time
11. How closely related are design shortcut and lack of architectural knowledge, in your opinion?
12. In your experience how aware are customers of technical debt, e.g. from a sustainment perspective?
13. What mechanisms are in place to prevent or identify downstream technical debt?
14. What are your major goals with respect to managing TD?
15. Can you contrast architecture debt with other types of TD?
16. Do you see evidence that managing architecture-related technical debt is helping achieve your goals?
17. Was the potential debt/risk well understood before it was incurred? If yes, was the concern ignored or considered in some way? If ignored, why?
18. For any specific debt instances discussed, what was the root cause of the debt?

# Follow-up
1. Is there any question I should have asked but didn't?
Thank yous and possible mention of data-driven analysis - looking at code or architecture docs with tools.
