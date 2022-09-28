### Blue Green deploy
[[Operations]]
[[Backward Compatible]]
- deploy into new clean instance 
	- Preferred
	- new system = BLUE
	- OR recycle an olderenvironment
- Retain existing functional system
- When BLUE passes all tests
	- Switch Load Balancer to BLUE
- Any Problems? 
	- rollback to previous instance
- Blue is now the new Green
- Decommission old Green
- 
