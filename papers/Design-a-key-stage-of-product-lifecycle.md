# Design a key stage of product lifecycle
Gero’s FBS model contains few aspects which needed to be updated for a usage of model-driven engineering in the context of Conceptual design

![](https://i1.wp.com/media.tumblr.com/d021548eb4cfeeb76c9b154193a4401b/tumblr_inline_mhejieWcay1qz4rgp.png)

#### Key Points
- R (Requirements): requirements and use case diagrams
- F (Functions): represented with internal block diagram (black-box model: function-flow)
- Be (Expected behaviour): activity, sequence and statemachine diagrams
- Bs (Behaviour of the system): parametric and same diagrams as Be
- GS (Generic Structure): class diagram (with abstract
classes)
- S (Structure): class, components and deployment diagrams

#### The NPD Best Practices Framework
![](npd-best-practices.jpg)

#### Four cornerstones of Resilience
![](http://www.kitchensoap.com/wp-content/uploads/2012/06/Screen-Shot-2012-06-12-at-8.43.57-AM2.png)

<b>Anticipation</b>
1. Functional and Architectural Reviews These are meetings open to all of engineering that we have when there’s a new pattern being used or a new type of technology being introduced, and why. We gather up people proposing the ideas, and then spend time shooting holes into it with the goal of making the solution stronger than it might have been on its own. We’d also entertain what we’d do if things didn’t go according to plan with the idea. We take adopting new technologies very seriously, so this doesn’t happen very often.

2. Go or No-Go Meetings (a.k.a. Operability Reviews) These are where we gather up representative folks (at least someone from Support, Community, Product, and obviously Engineering) to discuss some fundamentals on a public-facing change, and walk through any contingencies that might need to happen. Trick is – in order to get contingencies as part of the discussion, you have to name the circumstances where they’d come up.

3. GameDay Exercises These are exercises where we validate our confidence in production by causing as many horrible things we can to components while they’re in production. Even asking if a GameDay is possible sparks enough conversation to be useful, and burning pieces to the ground to see how it behaves when it does is always a useful task. We want no unique snowflakes, so being able to stand it up as fast as it can burn down is fun for the whole family.

Questions needs to be answered

1. Recognize when adaptive capacity is failing – Example: Can you detect when your team’s ability to respond to outages degrades?
2. Recognizing the threat of exhausting buffers or reserves – Example: Can you tell when your tolerances for faults are breached? When your team’s workload prevents proactive planning from getting done?
3. Recognize when to shift priorities across goal trade-offs – Example: Can you tell when you’re going to have to switch from greenfield development, and focus on cleaning up legacy infra?
4. Able to make perspective shifts and contrast diverse perspectives that go beyond their nominal position – Example: Can Operations understand the goals of Development, and vice-versa, and support them in the future?
5. Able to navigate interdependencies across roles, activities, and levels – Example: Can you foresee what’s going to be needed from different groups (Finance, Support, Facilities, Development, Ops, Product, etc.) and who in those teams need to be kept up-to-date with ongoing events?
6. Recognize the need to learn new ways to adapt – Example: Will you know when it’s time to include new items in training incoming engineers, as failure scenarios and ways of working change in the organization and infrastructure?

<b>Monitoring</b>
This is knowing what to look for, and dealing with the critical in systems. Not just the mechanics of servers and networks and applications, but monitoring in the organizational sense. Anomaly detection and metrics collection and alerting are obviously part of this, and should be familiar to anyone expecting their web application to be operable.

But in addition to this, we’re talking as well about meta-metrics on the operations and activities of both infrastructure and staff.

Things like:

1. How might an team measure its cognitive load during an outage, in order to detect when it is drifting?
2. Are there any gaps that appear in a team’s coordinative or collaborative abilities, over time?
3. Can the organization detect when there are goal conflicts (example: accelerating production schedules in the face of creeping scope) quickly enough to make them explicit and do something about them?
4. What leading or lagging indicators could you use to gauge whether or not the performance demand of a team is beyond what could be deemed “normal” for the size and scale it has?
5. How might you tell if a team is becoming complacent with respect to safety, when incidents decrease? (“We’re fine! Look, we haven’t had an outage for months!”)
6. How can you confirm that engineers are being ramped up adequately to being productive and adaptive in a team?

<b>Response</b>
This is knowing what to do, and dealing with the actual in systems. Whether you’ve anticipated a perturbation or disturbance, as long as you can detect it, than you have something to respond to. How do you? Page the on-call engineer? Are you the on-call engineer? Response is fundamental to working in web operations, and differential diagnosis is just as applicable to troubleshooting complex systems as it is

<b>Learning</b>

This is knowing what has happened, and dealing with the factual in systems.  Everyone wants to believe that their team or group or company has the ability to learn, right? A hallmark of good engineering is empirical observation that results in future behavior changes. Like I mentioned above, this is the place where Post-Mortems usually come into play. At this point I think our field ought to be familiar with Post-Mortem meetings and the general structure and goal of them: to glean as much information about an incident, an outage, a surprising result, a mistake, etc. and spread those observations far and wide within the organization in order to prevent them from happening in the future.

I’m obviously a huge fan of Post-Mortems and what they can do to improve an organization’s behavior and performance. But a lesser-known tool for learning is the “Near-Miss” opportunities we see in normal, everyday work. An engineer performs an action, and realizes later that it was wrong or somehow produced a result that is surprising. When those happen, we can hold them up high, for all to see and learn from. Did they cause damage? No, that’s why they “missed.”

One of the godfathers of cognitive engineering, James Reason, said that “near-miss” events are excellent learning opportunities for organizations, because they:

Can act like safety “vaccines” for an organization, because they are just a little bit of failure that doesn’t really hurt.
They happen much more often than actual systemic failures, so they provide a lot more data on latent failures.
They are a powerful reminder of hazards, therefore keeping the “constant sense of unease” that is needed to provide resilience in a system.

#### Resources
1. [](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=17&ved=0ahUKEwicncnEhc_TAhVI04MKHZU1DaI4ChAWCE0wBg&url=https%3A%2F%2Fwww.unf.edu%2F~broggio%2Fcen6016%2Fclassnotes%2F1-SoftwareEngineeringandBestPractices.ppt&usg=AFQjCNE1AymHU77LZBIGOWFNxfCOBo179A&cad=rja)

2 [USE method](http://www.brendangregg.com/USEmethod/use-linux.html)
