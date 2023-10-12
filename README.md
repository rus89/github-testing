# Testing GitHub Actions

I want to set GitHub actions to prevent us from pushing branches that doens't satisfy name convention.

1. Insights:
- Action is working but it doesn't prevent pushing changes to default (develop) branch
	- It just throwing error message

2. Insight:
- PR
	- if you select someone to review it, it must be review by developer other than author
		- author can't review its own changes
	- Actions check is applied
	- it's possible to make automatic deletition of the branches after it is merged
	- it's possible to disable merging but to force squashing
	- if Action is failed, it won't prevend reviewer from squashing/merging (is this possible, or is it needed since the branch will be automatically deleted)
