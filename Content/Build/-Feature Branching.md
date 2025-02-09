- This [[Anti-Patterns]] 
	- delays release of new code
	- accumulates multiple code packages into a big bang release
	- BUT is widely used in the industry and arguments can be made in favor of using it.
	- Can be relieved with [[Runtime Feature Flags]] but avoid [[Content/DevOps MindMap/Build/-Persistent Feature Flags|-Persistent Feature Flags]]
	- [Gitflow Workflow | Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)
- INCREASES [[Reduce Cognitive Load]]
	- Team members need to retain knowledge of multiple change sets over multiple weeks
- Debugging becomes complicated by
	- Which change could have caused XYZ?
	- What all did we change in the last 3 months?
	- OK, it's change X from 2 weeks ago, why did we do it -that- way?
- Often requires extra testing environments
	- further increasing [[Reduce Cognitive Load]] keeping track of multiple overlapping in time
		- We fixed that in change XYZ. Does that build include XYZ?

### Best Practice is [[Runtime Development Control Flags]]