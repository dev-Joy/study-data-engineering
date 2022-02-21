# My approach for getting a 230k offer from Non-FAANG as a DE with 1 YOE (Zero Leetcode prep)

I made a post a few days ago, and a lot of people have reached out to me about it for advice and asking how I got this offer. I ended up turning it down, and I’ll explain more below. This post is mainly directed towards the <2 YOE crowd, I’m not trying to be all preachy or be like “I found the secret sauce,” so feel free to comment with additional advice or counterarguments to this post. I’m just posting my approach since it turned out successful, and I thought I’d share it with the community.
About me

1 YOE as a DE in corporate dev. First job out of college, 22 years old. Undergrad degree unrelated to CS (though I minored in it). Recently got an offer for 230k (Big Tech but non-FAANG) as a DE among several other offers. I cold-applied (without a referral) and most reached out to me within a week or two after that.

Even though I only have 1 YOE, I got a ton of exposure and valuable experience in this past year. Worked on tons of high-impact projects across different teams and business units, and got the opportunity to punch above my weight class very early on, and I was basically kicked to mid-level after 2-3 months.

My tech stack is Python, Spark, and SQL. My previous company contracts a proprietary version of Airflow and Tableau (Not any of these 2, but similar, closed-source tools). Zero experience in Cloud in a production setting but I’ve toyed around with it in my free time. I also did zero Leetcode prep.
My Approach

Like many of you, I believe Leetcode is a complete waste of time. It provides zero business value, and I personally don’t believe it is a strong indicator of success. ESPECIALLY for such a specialized role like DE. My thought process was like this: Why would I spend hundreds of hours on these algorithm puzzles when I could be spending that time learning things that actually provide business value? Things like cloud computing, the modern data stack, data team strategy, etc.

I am pretty confident in my technical abilities. I would say that I’m at least average in Python and SQL, but I am confident that I have the core proficiency for most DE jobs (designing a pipeline, implementing it, managing stakeholders), and I can learn any specific tools or niches on the job. For every interview across the 6 or so companies I spoke with, I asked each interviewer the following question "What challenges has your team been facing recently?" Over 90% of the responses were related to organizational issues. Things like mounting tech debt, dumbass MBA stakeholders, unstable leadership, unreasonable timelines, high pressure, poor infra, not having a seat at the table, etc. Less than 10% answered with technical difficulties. As such, I decided to focus my studies on good DE practices, team process/strategy, stakeholder management, and some surface-level technical stuff sprinkled in. I spent A LOT of time reading and watching videos on these subjects.

Some specific subjects include:

    Data Security and Privacy Regulations (GDPR, India’s new laws, Australia, etc..) and strategies for dealing with these challenges in our system design (data localization, right to request, etc.)

    Clean code, how to write good technical documentation, and strategies for technical debt.

    Snowflake basics and core concepts

    Basic understanding and limited hands-on experience with Cloud Services used for DE (AWS and GCP mainly).

    “The Modern Data Stack” — Fivertran/Stitch, DBT/Spark, Redshift/BigQuery/Snowflake, Mode/Looker — What are each of these tools, what problems do they solve. Then I spent a weekend for each tool using their free trial, clicking every single button and skimming through all documentation, etc. Just touching it, doing some walkthroughs, tutorial, etc. The goal here is to be able to talk about these things and even though I’ve never used these tools in a prod setting, nevertheless I get bonus points for proactively seeking out these skills.

    A shit ton of blogs about data teams and processes (Locally Optimistic, Luminous Men, DBT Labs Blog, Erik Bernhardsson personal blog, Dataversity, Maxime Beauchemin personal blog, among others); I especially tried to identify common organizational challenges that data teams face across the industry and some strategies for dealing with them.

    Skimming and/or reading Core DE/programming Books (DDIA, TDWTK, Storytelling with Data, the Pragmatic Programmer, Peopleware, the Mythical Man-Month)

    Watching recorded talks from DE conferences (Coalesce, Spark Summit)

    Other (Office politics, stakeholder management, dealing with red-tape, and social skills, etc.).

For the 230k offer, I got 1 Leetcode medium, 2 SQL medium, and 1 mock code-review. In addition to these technical assessments, there were 3 non-coding rounds. I completely winged it on the live-coding sessions and did somewhere between bad and average on the Leetcode and SQL stuff, but I killed it on the code-review and all of the non-coding + system design stuff. I set myself apart by strongly presenting three qualities: product-sense, “give-a-shit”, and leadership.

Product-sense: I want to understand and focus on how we create business value.

“Give-a-shit”: I want to be a great contributor to my team and org. I don't just want to cash a check and climb the ladder.

Leadership: I try to be someone that others want to have on their team.
Product-sense

Often, interviewers asked me “how” questions. “How” do we implement this feature? “How” do we architect this pipeline with these requirements? This is the technical sense. While delivering an approach is good, nevertheless, I always counter with “why?” Why are the requirements like this? What business value does this feature or pipeline provide? Why is that the timeline? Is that a hard deadline? Can we provide a minimum viable product with fewer features? Who is the end-user? How do they intend to consume this product?

This is intended to send a strong signal that I can manage upwards and can carry my own weight. It also indicates that I think about the tasks we do in how they relate to the business and that I have my eye on the prize (generate revenue, reduce losses, or cut down man-hours) as opposed to just abstract JIRA tickets.

Now, the interviewer may not answer any of these questions and say “It’s totally open.” Well, no, it never is in real life. I would never start development on any project with “totally open” requirements. My experience in DE has been that it’s super critical to nail down requirements and not let stakeholders walk all over me, and I could tell that this kind of thinking resonated with my interviewers, as DE’s often do not have their voice heard. I digress, if the interviewer won’t give me specifics, then I create the context myself and explain to them along with my tailored solution:

End-User
Another Data Engineer
Executive or Senior Management
Data Analyst or Scientist
Non-Technical Product manager
Technical product managers
Customer
Client
Vendor
Timeline, hard or soft
End of Day
1 week
2 weeks
1 month
Consumption
BI Tool
Code Repository
Report
Dashboard
API
Presentation
Business Value
Loss-Reducing
Revenue-Generating
Reduced Man-hours
Product Delivery Model
Dummy Prototype/Mockup
Prototype or Proof-of-Concept
Minimum Viable Product (some features cut)
Full Product (all features)

From here, I defined 6 core concepts I consider in my approach, and I prioritized them based on all the information I had gathered:
Reliability

How fault-tolerant is this design?
Maintainability

How much technical debt does this design take out?
Scalability

How well will this design handle terabytes of data?
Extensibility

How easy will it be to add additional features as the scope of the project increases?
Security

How safe does this data need to be? What extra measures (if any) need to be applied?
Operability

How easy will it be for the end-user to consume it in the intended manner?

I came up with one to three examples for each of these points in my framework that are tailored to the context I created above. I then emphasized how my solution creates business impact within the given timeline and added that there are additional features we could add to improve the product in future versions.
“Give-a-shit”

I wanted to use the word ambition, but I don’t think that’s fitting. To me, “Give-a-shit” means that I actually take some pride in my work. I care about the quality/readability of my code, the end user’s experience, my documentation, change management/tech debt, my interactions with stakeholders, I want to support my teammates’ success, etc. Anyone on a DE forum in their free time like this probably already possesses this quality. But it doesn’t mean working long hours with an “always-foot-on-the-gas” mentality. I’ve just met so many people who really just want to do the absolute bare minimum for 8 hours and then log off. I tried to present myself as someone who is engaged with the industry at large and its emerging trends, wants to improve my craft, wants to punch up, and is empathetic and curious.

I did this by giving some praise to my current teammates, dropping in some knowledge from the blogs I’ve read and/or discussing my sources of info (specific blogs or books), talking a LOT about my strategies to deal with tech debt and documentation, talking about the projects that I’m proud of and focusing on the business value they created (even if my work didn’t directly affect the bottom line).
Leadership

You don’t have to be a boss or have many YOE to be a leader. You can be a leader in different ways. You can set an example by writing clean code, good documentation, and using best practices. You can raise the bar by identifying or creating new best practices. You can advocate for a teammate whose voice is not being heard. You can mentor new grads or interns. You can create really crisp presentations of your team’s work (solved a unique technical challenge, did something with high business impact, etc.) and share them with your team, leadership, or cross-functional teams. You can call out the excellent and hard work done by a teammate. You don’t need to be the boss or step on any toes to do any of these things, but all of these things will get you clout. I spent the past 6-8 months focusing on these things, trying my best to be a “go-to” guy for my current team. Again, I’m a mediocre developer. I still have a ton to learn tech-wise, but I got glowing references from my teammates and a ton of genuine experience to talk about in my interviews.
Asking Good Questions

The last thing I did was come prepared with good questions. I didn’t do this to look good, I did it because the last year in corporate dev has sucked, and I am super sensitive in my criteria for my next job. But it got me lots of bonus points anyway as well as great data points on the company I'm interviewing for and whether or not it's the right fit for me.

    How does this role create value?

    What does success look like in this role? How is it measured?

    What is your/your team’s strategy for handling tech debt?

    Why did you choose this interview format (Leetcode, whiteboarding, code-review, etc.)?

    What are some challenges that your team has been facing recently?

    What does the onboarding strategy look like?

    How much confidence do you have in the org’s leadership?

These are great jumping-off questions and will get you real good bonus points, and it kind of turns the tables onto them. I dug deeper with some follow-up questions based on the responses, and I was really trying to dig into the shit for each company I interviewed with. Some of those questions may seem impertinent, but I got some very interesting responses for all of these questions (especially the ones about leadership), and no one really seemed offended. Depends on your attitude and how you deliver it, I guess.
End

That’s pretty much it. I got offers from all the companies I interviewed with, the highest being 230k annual. They were pretty aggressive in trying to bring me on, but I ended up turning it down because they don't have their shit together. I would've made bank, but I'd be chained to my desk and do nothing but firefighting day-in and day-out. I went with another offer for 140k at a company that’s super organized, aligns with my lifestyle and work philosophy, and appears to be a rocketship with amazing growth opportunities and better exit ops after a few years
