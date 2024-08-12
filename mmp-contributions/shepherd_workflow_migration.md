# Workflow migration to Argus/Shepherd

- Task: Migrate existing workflows for all of our automated processes to run via in-house Target workflow orchestration service.
- Importance: Teams were previously responsible for running workflows as they saw fit. Argus and Shepherd provided a streamlined, standardized way to run workflows across the business. This migration was important in order to modernize and normalize our processes to meet Target standards.
- Learnings:
  - Upgrading to Java 17 and Spark 3.5.1, including all necessary dependency upgrades (prerequisite for the migration).
  - Understand the Shepherd API to automate creating and updating workflows using HTTP requests via our CI/CD pipeline.
  - Learn how to leverage a new system to meet our team's needs using limited documentation.