- Redeploying into a pre-existing Environment is often required but it's a DevOps [[Anti-Patterns]]
	- full clean deploy can be time consuming
	- if the goal is running a deploy+test cycle in under 15 minutes, building clean servers from scratch can take too long
- Mitigation
	- redeploy for in-day builds
	- clean rebuild every night