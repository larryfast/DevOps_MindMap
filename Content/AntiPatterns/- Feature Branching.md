### Feature Branching 
- This [[Anti-Pattern]] 
	- delays release of new code
	- accumulates multiple code packages into a big bang release
- INCREASES [[Reduce Cognitive Load]]
	- Team members need to retain knowledge of multiple change sets over multiple weeks
- Debugging becomes complicated by
	- Which change could have caused XYZ?
	- What all did we change in the last 3 months?
	- OK, it's change X, why did we do it -that- way?
- Often requires extra testing environments
	- further increasing [[Reduce Cognitive Load]] to keep track of multiple overlapping in time
		- We fixed that in change XYZ. Does that build include XYZ?

### Best Practice is [[Runtime Development Control Flags]]