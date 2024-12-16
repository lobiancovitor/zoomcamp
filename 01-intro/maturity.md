## MLOps maturity model

Helps clarify the Development Operations (DevOps) principles and practices necessary to run a successful MLOps environment.

### Level 0: No MLOps (Manual process)
- Disconnection between ML and operations
- Data gathered manually
- Experiments aren't tracked
- Manual releases each time
- All code on notebooks

### Level 1: DevOps no MLOps
- Data pipeline gathers data automatically
- Experiments aren't tracked
- Release is handed off to software engineers
- CI/CD
- Application code has unit tests
- No reproducibility

### Level 2: Automated Training
- Convert experimentation code into repeatable scripts/jobs
- Training pipelines
- Experiment results tracked
- Training code and resulting models are version controlled
- Manual release (low friction)
- Model registry

### Level 3: Automated Model Deployment
- Automate model integration into application code
- Release managed by continuous delivery (CI/CD) pipeline
- Unit and integration tests for each model release
- Easy to deploy model (low human interferance)
- A/B tests: compare between models versions on deploy

### Level 4: Full MLOps Automated Retraining

- Highest level
- Post-deployment metrics gathering
- Retraining triggered automatically based on production metrics
- Less reliant on data scientist expertise to implement model
- Automatic training, retraining and deployment

#### Not everything need to be at level 3 or 4