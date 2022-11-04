### Runtime Development Control Flags
[[TODOs]]
[[Flikr Velocity 2009]]

- Alt name: Runtime Unreleased Development Flags
	- Feature Flags can be mishandled if they become persistent in the code and the application
	- For DevOps,[[-Persistent Feature Flags]] are an anti-pattern
- Feature Flags decouple [[Deploy vs Release]]
- While this helps with [[Backward Compatible]] the more important goal is [[Deploy Incomplete Code]]
	- A 1-2 day development package is rarely sufficient to complete a feature.
	- Minimally self-consistent but nothing near complete 
	- This is important for [[Tip Development]]
#### Runtime is important
- Allows a single build to be used in all environments
- Allows testing of Flagged feature in any environment, even production
- Flags can be coupled to Logins, or similar, to allow Testers or Beta customers to activate the code without exposing it to all customers
- build
#### Unreleased is important
- Once a block of code has been released and is always on in production, the Flag(s) should e stripped from code