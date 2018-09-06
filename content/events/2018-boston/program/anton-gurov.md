+++
Title = "Anatomy of an AWS Account Cryptojack"
Type = "talk"
Speakers = ["anton-gurov"]
+++
This is a story about a cryptojack security incident involving one of CHT customers’ AWS development accounts. I will discuss not only the incident and response, but also some of the ways to prevent this type of event from occurring, how to detect it, and forensics data for which to look.

It’s a personal story/lesson from the field and I would like to share it with people in the industry to help them avoid this pitfall.

About a year ago I was a part of an incident where one of our customers reported a security event involving one of their numerous AWS accounts used for development purposes. The AWS account in question already generated about $40k worth of EC2 compute charges when they discovered this breach. There were about 100 or so top-end, CPU-heavy Windows machines spread out across the world running at 100% CPU for over 2 weeks, all apparently mining bitcoin.

No CloudTrail audit configuration was enabled for this account so there was no audit data available to identify what happened and who did what.

Our Cloud governance platform captures the state of AWS accounts and configurations, and historical data for some of these settings. Our team spent a few days reconstructing the state of things and how events transpired by looking at our backup data on a timeline. It was clear from our data that one of their admin employee account AWS credentials got compromised/leaked and were used to spin up all these resources. It also appeared that this attack was entirely automated and only needed sufficient AWS credentials as an input. An attacker also covered up their tracks and tried to “frame” another innocent user!

Luckily, the data we had cleared this user’s name and the customer received full AWS credits for the breach to cover the loss, but this was an important lesson for us and for our customer. This was an entirely preventable incident.

We saw a similar pattern/attack on our own infrastructure. The attempt failed due to some simple security measures we’ve taken. I’ll talk about some of the ways to prevent this event from occurring, how to detect it, and the forensics data to look for: things like enforcing MFA, using external Idp, removing the need for the AWS key and secret key by leveraging roles and instance profiles to grant permissions, etc. I will also talk about the importance of having the CloudTrail audit feature enabled by default in AWS.
