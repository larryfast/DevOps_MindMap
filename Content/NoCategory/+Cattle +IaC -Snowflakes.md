### +Cattle +IaC -Snowflakes
- Back in the day we used to configure servers by hand and invent a unique name for each. 
- Generically we call them Snowflakes. Each is unique. 
- Product would get deployed and redeployed onto a Snowflake. 
- The server config was manually upgraded incrementally
- Snowflakes are expensive to maintain
	- Since there's no standard, every issue must be investigated manually
- Snowflakes are very hard to replace
	- Nobody knows the configuration
- If a Snowflake is critical to Operations, it becomes irreplaceable
- Snowflakes are boat anchors that prevent modernization

- Is Cloning Good Enough? No!
	- You get identical servers but can you repair, replace or upgrade the original Image?
	- 
- [[Infra as Code IaC]]
	- Build each server from scratch with code that defines the exact configuration.
	- Anyone can read how the server is configured
	
- Treat servers like Cattle
	- Each gets a number, not a name.
	- Build them identically from IaC
