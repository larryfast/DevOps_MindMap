### Env Security
[[Operations]]
[[CICD]]
[[OIDC - OpenID Connect]]
- Start by focusing on the Production Environment 
- You can't allow any old Joe to deploy new code into Production
- Ideally only the CICD pipeline can deploy changes to production
- Deploy requires often requires Root or other high privilege credentials
- Creds must be available automatically without a privileged user sign in
