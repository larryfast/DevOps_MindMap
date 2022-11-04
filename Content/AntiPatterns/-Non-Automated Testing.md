### -Non-Automated Testing
[[Anti-Pattern]]
- All too often manual testing is unavoidable.
	- Legacy Systems
	- No budget for automation
	- Difficult to automate because development did not bulid for [[Design for Automated Testability]]
- CICD goes from minutes to days when manual testing is required in the pipeline

#### Mitigation
- Prioritize Automated Sanity Testing, then Regression Testing
- Automation's first priority is ensuring that existing functionality is not broken

- New code matters much less than the stability of existing code
	- [[DevOps Handbook]] Biz Case Ref???
		- Company XYZ was rotating through 3 weeks of manual regression tests. 
		- They built their first CICD pipeline with just 12 automated sanity testcases. That was enough to ensure baseline product quality. 
		- Eventually they had hundreds but 12 was enough to start.
- [[Runtime Development Control Flags]] are important for ensuring new code does not impact existing product.

- Non-automated tests are OK as long as they do not gate the CICD pipeline
- some manual testing of new features is OK - nobody depends on those features