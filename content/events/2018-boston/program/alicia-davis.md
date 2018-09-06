+++
Title = "Why we provisioned 37 Jenkins servers: How to architect your CICD pipeline to account for organizational maturity"
Type = "talk"
Speakers = ["alicia-davis"]
+++
Many times during DevOps transformation, creating a technology architecture comes first. Then the uphill battle of closing skill and process gaps during adoption begins, which forces people to adjust to the technology. What if this process were reversed? This talk describes a real-world experience about how our Platform team created a distributed and non-optimized toolset architecture that allowed for teams with varying maturity to rapidly adopt and transform without that uphill battle.

When you talk to anyone that has been through a failed attempt at implementing DevOps, you will usually get a resounding “it’s a culture/people” aspect that hindered adoption. Since one of the tenets of DevOps is to constantly change, why should that not also include evolving the architecture?

The outline of the talk will include: the background of the company in which we architected this toolset; size, industry, VM count & geographic distribution; application architecture & stack (high level), business-as-usual software development process (high level); and the technical and cultural team challenges. Also: Platform team background; the approach we took in architecting; overall architecture; Custom UI, Jenkins, Artifactory, SVN; the Platform team ‘Day 2’ operations optimizations for managing the toolset, including script promotion process, developer ‘onboarding kit’, Jenkins server provisioning/monitoring/maintenance, and developer onboarding guidelines. Examples of different team experiences during onboarding will be provided, along with process and organizational changes we implemented to help facilitate adoption. Finally, we’ll review our results after 2 years (hint: we were successful), lessons learned, and key success criteria

The audience will be able to identify with some, if not all, of the company characteristics and challenges discussed, and will be able to hear small, actionable steps they can implement in their own organization.
