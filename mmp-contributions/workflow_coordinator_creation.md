# Workflow and coordinator creation for email content aggregation

- Task: Implement an Oozie workflow and coordinator to run our email content aggregation Spark job daily.
- Importance: Our message decisioning capabilities rely on up-to-date personalized recommendations for each active Target guest. The processes that select message content for each guest pull from the output of the email-content-aggregation pipeline, which must be run daily via this workflow in order to keep the aggregated data fresh.
- Learnings:
  - How to utilize the team's internal "OozieGen" framework to produce an Oozie workflow.
  - How to set up the coordinator and environment-based configs to run the job at a certain time and with specific parameters.
  - Manual testing of a workflow via Target's internal Hadoop data environment.
  - Validating the setup and running of the workflow after being deployed via our CI/CD pipeline.