## 📑MLOps Maturity Model

Reference: [MLOps Maturity Model: Microsoft Docs](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/mlops/mlops-maturity-model)

|Level|Description|Overview|When Should You Use?|
|---|---|---|---|
|0️⃣|No Automation 😢|<ul><li>All code in Jupyter Notebook</li><li>No pipeline, experiment tracking, and metadata</li> </ul>|<ul><li>Academic projects</li><li>Proof of Concept is the end goal, not production-ready models</li></ul>|
|1️⃣|Yes! DevOps😀, No MLOps|<ul><li>Best engineering practices followed</li><li>Automated releases</li><li>Unit \& Integration Tests</li><li>CI/CD pipelines</li><li>No experiment tracking and reproducibility</li><li>Good from engineering standpoint, models are not ML-aware yet!</li></ul>|<ul><li>Moving from proof of concept to production</li><li>When you need some automation</li><ul>|
|2️⃣|Automated Training 🛠|<ul><li>Training pipelines</li><li>Experiment tracking</li><li>Model registry (track of currently deployed models)</li><li>Data scientists work in tandem with the engineering team</li><li>Low friction deployment</li></ul>|<ul><li>When you have increasing number of use cases</li><li>Three or more use cases, you should definitely consider automating!</li><ul>|
|3️⃣|Automated Deployment 💬|<ul><li>Model deployment simplified!</li><li>Prep data >> Train model >> Deploy model</li><li>A/B testing</li><li>Model X: v1, v2 >> v2 is deployed; how to ensure v2 performs better?</li><li>Model monitoring</li></ul>|<ul><li>Multiple use cases</li><li>More mature + important use cases</li><ul>|
|4️⃣|Full MLOps Automation ⚙ |<ul><li>Automated training</li><li>Automated retraining</li><li>Automated deployment</li></ul>|<ul><li>Check if level 2, 3 won't suffice</li><li>Should model retraining and deployment be automated as well?</li><li>Super important to take a pragmatic decision! Do you really need level 4?😄</li><ul>|
