# async-team

Some documentation about how to run an async team (e.g. a remote team in different places). 

### About

Most of this is inspired by how we run the [dat project](http://dat-data.com), as well as lots of lessons learned from years of open source development. Currently the dat project has 7 paid contributors (team members) who work on dat related projects a lot, and hundreds of open source contributors who make smaller contributions infrequently.

### Stuff we use every day

#### [github](https://github.com)

We have a github org called `datproject`, and a repo under there called `discussions` that is used as a team-wide mailing list. For example, we have an issue for the high level project roadmap that has a markdown checkbox list where each item corresponds to a more detailed issue in another repository somewhere.

If you 'Watch' a repository on GitHub you will get notified when someone comments on a commit, issue or pull request. The default notification is to get an e-mail, but you can turn this off. You also get notifications when someone `@-mentions` you in a comment. This makes GitHub issues a pretty good replacement for a traditional mailing list.

Individual projects get their own repositories, preferably created and owned by the team member who is the BDFL on the project. For example if we wanted to make a new project to e.g. demonstrate how to run Dat in Docker, and the point-person on the project is going to be `@mafintosh`, then he should create a repo at `https://github.com/mafintosh/dat-docker-example`, rather than `https://github.com/datproject/dat-docker-example`.

It can cause delays to have to ask permission first to do something, especially when the person you are asking persmission of is asleep in a different time zone. The combination of BDFL owned personal repositories and splitting projects up into small modules allows us to minimize the amount of synchronization overhead.

We use the `datproject` organization to house repositories that don't make as much sense to have individual ownership.

Using GitHub issues effectively on a remote team takes some work. One skill you learn from doing tech support and/or participating on open source is how to write up a reproducible test case. You want to make sure that when the person you are asking a question of wakes up in 4 hours, and you have gone to bed, that your question has all of the information needed for them to give you a good answer.

Another advantage of many small repositories is that opening issues on a repository will only notify those who are watching it. By contrast, if you have one huge repository that everyone commits to, opening issues will notify everyone watching it, which is likely the entire team.

#### [irccloud](https://irccloud.com)

Cons of IRC: Most IRC clients are notoriously hard to use for beginners. IRC runs on a port that is blocked on some WiFi. You can run your own IRC 'bouncer' but that requires sysadmin skills. Terminal IRC clients also require CLI skills to use and don't work on smartphones. Registering a nickname requires knowledge of custom IRC commands.

Pros of IRC: Most open source projects have chat on freenode. Chat is public and often logs are kept and logs are searchable/indexed by Google. 

To solve the usability issues of IRC we all use IRCCloud, and pay the $5/month fee to have IRCCloud keep each of us logged in all of the time. The persistent idling combined with the excellent iOS/Android IRCCloud apps mean that we can ping each other in the `#dat` channel on by PM and know the person we are pinging will get a push notification (if they want to). Honestly, without IRCCloud, we would probably not use IRC as much.

### Stuff we use a few times a week

#### [slack](https://slack.com)

Slack is great if you need your conversations to be private, but since our project is a grant funded open source project, the only thing we really use Slack for is the rare occasion where we have team-only matters to discuss like e.g. paychecks. 99% of our communication happens in IRC. The few things that Slack does better than IRCCloud don't outweigh the benefits of being in the public.

#### [screenhero](https://screenhero.com)

We like Screenhero because it does one thing well. It lets you invite someone to view your desktop, have their own mouse + keyboard on your desktop, and also does voice chat, but no video (which is good because you honestly don't need video for remote pairing). The two main developers on our team have the $10/month upgraded Screenhero accounts, which lets them invite other members of the team (who all have free accounts) to have Screenhero sessions. We look forward to the future version of Screenhero that has multi-user team-wide screen sharing, at which point we will likely upgrade to their Team plan. 

#### Google hangouts

When we have to do group video chat we choose Hangouts. It works on smartphones and generally works pretty well (including screen sharing!). We don't do a lot of these, as any time you have meetings with more than 2 or 3 people it tends to waste a lot of time.

##### Hangouts On Air

Every few weeks we do a big technical discussion call. Recently we started doing them in the open and inviting the public to participate. We create an issue about a week before the call on our discussions repo (example here: https://github.com/datproject/discussions/issues/19) and we use that to set the agenda and get questions from people, as well as share basic information like how to connect and listen to the call.

We use [Hangouts On Air](https://plus.google.com/hangouts/onair), which is nearly the same as Hangouts except it lets you live-broadcast to YouTube. Only Dat team members and others on the agenda will be invited to join the Hangout so they can broadcast voice and video. Hangouts only supports about 10 people max, but the youtube stream can support an unlimited amount of viewers.

Hangouts On Air automatically archives our call on youtube (up to 6 hours long). Here's an example of a recent call: https://www.youtube.com/watch?v=4J9CSoQ-4-0

It's really nice to be able to link to specific parts of the discussion, e.g. https://www.youtube.com/watch?v=4J9CSoQ-4-0&t=30m20s

### Stuff we consciously do not use

#### E-mail

We don't issue team e-mail accounts so that we don't rely on 1-on-1 e-mail for getting things done. We think it's much better to use GitHub issues, that way anyone on the team or the wider open source community can help answer.

### Travel

Note that there are a lot of people who write about remote working on the internet, and this does not claim to be authoritative on the subject, I am just sharing what works for us.

Everyone on our team lives in a different city, and we are in many different time zones. Choosing when and where we work is great for a while, but it's also nice to balance that out with intense periods of face-time. We try to meet up 6 times a year for between 2 and 4 weeks at a time and hack in-person. These trips are not mandatory, and there are no quotas, but we like to encourage these 'hacker visitations' as much as possible.

We generally rent a whole apartment on AirBNB and house 1-2 out of towners there, and pick a location where one of the other team members lives so they can be the local guide. I'm actually currently writing this from a pancake restauraunt in Taipei, which is an excellent city for remote working due to it's low cost and large number of cafes. Nobody from our team lives here, but two of us who normally live in different cities are currently visiting and working together here.
