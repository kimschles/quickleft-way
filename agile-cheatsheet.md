# Quick Left Developer Agile Process Cheat Sheet

Following a well-defined agile process keeps developers and clients happy.  What follows is a list of things to consider if you are running a project at Quick Left. This should be viewed as a resource, and not a prescriptive guide.

This cheat sheet is organized by timeline, beginning with the project inception and ending with handoff.

## BEGINNING OF PROJECT

### Inception Meeting

The inception meeting sets the tone for your relationship with the client for the rest of the engagement. Be excited, but don't promise more than you can deliver. Above all, have a plan.

The inception  meeting should include an expansive process, where you work together to discover their needs, and identify many things that _could_ be built. This should be followed by a contractive process, in which you work together to whittle down the ideas you've come up with into a set of features that can actually be completed. This initial release can be thought of as a _minimal viable product_ (MVP).

Ideally, you should come out this meeting with the full scope of the project expressed in the backlog as high level user stories. The client and QL should also be in agreement about the features that we are expecting to complete during the engagement.

User stories should be estimated and prioritized to allow you and the client to agree on timelines and milestones.

### Set Expectations

Set a tone of open and detailed communication from day one. Let the client know your expectations. Ask them to commit to attending standups and retros, accepting stories regularly, providing assets you need, and communicating early and often as requirements change or they feel that their expectations are not being met.

We are a time-and-materials based shop. We do not do fixed bids or not-to-exceed clauses. Ensure that the client understands that we are not promising an exact set of features by a certain date or for a certain cost. As our understanding of the project evolves, features may be cut, and budget or timelines may be extended. Prepare the client for the possibility of disappointment in these cases.

If a client has not participated in agile software development before, explain the purpose of each component (project management software, standups, retros, pairing, story acceptance). Explain the difference between a feature, a task, and a defect.  This conversation may also be valuable if their version of _agile_ is different than ours.

## DAILY

### Standups

Have a standup with your team each day

Each member should report on:
- what they've been working on
- what they plan to work on
- any blockers
- any schedule irregularities

Decide what level of pairing is appropriate

Make a plan for the rest of the day

### Client Communication

Be in contact with your client daily, either via a standup or on Slack

Keep clients updated on current velocity, work remaining and any scope or budget constraints they should be aware of.

Eliminate surprises by announcing any red flags as early as possible.

### Update Documentation

Make sure you keep your project's documentation up-to-date. Include steps for setup, compile and deploy, a description of the high-level architecture and gotchas as you notice them. It's much easier to do this as you go than it is to try to pull it all together in the last days of the project.

## WEEKLY / BI-WEEKLY

### Client Meeting / Retrospective

Each week, you should do a client retrospective meeting. This is the time to show off what we've been working on, plan for the future, manage scope expectations and reinforce a positive and communicative tone in the working relationship.

If necessary, reiterate that we are working on time and cost estimates based on the features currently agreed upon and that unknowns can cause timelines and budgets to increase.

Early in the project, you are likely to have to disappoint the client if you have discovered that the cost of certain features has been under-estimated. The goal of our agile process is to give a realistic picture of the work and find creative solutions to scope and budget issues we discover during the course of the project. We don't promise what we can't deliver.

Hold the client and the Quick Left team to their meeting attendance, story acceptance, asset provision and communication commitments.

If the client is new to agile, re-explain the meaning and purpose of each component as necessary.

Identify any tech / process / personnel issues that the client is having, if any. This is a good time to provide value to the client by giving them an outside perspective into their own process.

It's more important to listen and understand when working with a client than it is to educate. This is their business, we're here to listen, advise and implement. Keep client meetings on track, but not at the expense of client happiness. If things go really wrong, consider conducting a "5 Whys" retro with the client and our team.

### Demo & Acceptance

Each client meeting should include a project demo.

The most recently completed stories should be merged into the main Git branch and running on a staging server before the meeting.

Show the business value that was delivered in the sprint and the commitments that were hit by walking through the features in real time.

Ask client to accept each story after it is demoed. When they do, they are agreeing that you've built what you said you would and that it works. If the feature that satisfies the story isn't what the client anticipated, either move the story back into the backlog or add a new story that better explains expectations. Client acceptance can happen before a formal QA process. If QA finds a bug after the client as accepted the story, it should be filed and addressed as soon as possible. Agile gets things right through iteration. If something isn't right...iterate!

### Sprint Planning

After each sprint, you should plan the next one (with the client).  This is most likely to happen during the retrospective.

Identify high-level goal(s) for next sprint (it may be an epic), then select and groom stories whose collective completion will represent completion of the goal.

All those involved in the project should commit to do their part to finish these stories in the next sprint. This means both developers coding and clients providing assets or information needed to get the stories done.

### Backlog Grooming

As part of preparation for a sprint, you should groom the backlog.  Clarify whose responsibility this will be early on. It may be done by the team lead or the whole team. Get client sign-off where appropriate.

You may also want to groom the backlog continuously through the week as you work.

In either case, groom stories "just in time". If you groom too early, you run the risk of stories getting stale as requirements change, resulting in wasted effort.

A well-groomed backlog allows other developers joining the project to get to work more quickly and mitigates the effects of a knowledgable team member moving off of the project.

Groomed stories should have:
- acceptance criteria
- screenshots
- weighting
- client sign-off
- feature workflow described in detail (consider using [Gherkin](https://github.com/cucumber/cucumber/wiki/Gherkin))

## END OF PROJECT

### Last Weeks

As you enter the last weeks of your project, you should begin to work with client to prepare them for the handoff.

Prepare them for the fact that QL will not be available to fix bugs or add features after the handoff meeting unless a retainer contract was been negotiated.

Go through Sprintly with the client, ensuring that all of the required features and bugs are captured and on schedule to be completed by handoff. Additional stories can be captured for future work by Quick Left or someone else. Remind the client that they are always welcome to negotiate another SOW with sales if they desire additional features or wish to have devs available to put out fires at release time.

Schedule the handoff meeting if it's not already on the calendar.

### Handoff

When the project is complete, you should have a handoff meeting with the client to transfer ownership of the code to the client.

Celebrate what you've built together and demonstrate the business value of the project. Reiterate the business goals we set out to accomplish and reflect on the journey you took together to get to this point.

Come prepared with access keys, login credentials, server addresses and anything else that the client will need to manage their application. Have someone with access transfer ownership of the GitHub repository to the client before the end of the meeting.

Remind the client that QL support for the code and project ends after the meeting, unless other arrangements are made.

If there are any remaining features or bugs, make sure they have been captured in the tracker and that the client will continue to have access to it, so that she can manage them on her own as time goes on.

Find a way to end on a high note, bringing a sense of completion and a feeling that this project positive experience. We want our clients to be happy and refer us to their friends, or come back for more work.

### Example Handoff Checklist

This is an example for a Rails project hosted on Heroku

- Concurrent server on Heroku (e.g. Puma)
- Using background workers for blocking processes
- Redundant dynos for app and workers
- Production-grade database added
- Scheduled database backups
- Using AWS for asset storage
- Environment variables properly set up in Heroku config
- Using latest Ruby version
- SSLset up
- Deploy workflow documented clearly
- Performance monitoring set up (e.g. New Relic)
- Logging set up (e.g. Papertrail)
- Error reporting set up (e.g. Airbrake)
- GitHub repositories forked / tranferred to client's organization
- Sprintly ownership transferred to client
- Heroku ownership transferred to client (staging and production)
