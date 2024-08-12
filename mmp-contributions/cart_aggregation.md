# Cart Aggregation

- Task: Implement a Spark job to intake cart activity data (add, update, remove, purchase) for millions of guests and aggregate into a complete up-to-date cart snapshot.
- Details:  Based on the actions pertaining to each guest / cart id, I had to apply logic to find the resulting items in the cart based on each action and timestamp.
- Importance: Many of our messages pertain to guests' cart status, including abandoned cart reminders and sales/promotions on items in the cart. Our upstream data source only provides raw cart actions (i.e. when a guest adds an item to the cart). The aggregated cart snapshot allowed us to send trigger messages to guests according to our business requirements. For example, if a guest left an item in their cart for 2 hours, we sent a reminder message.
- Learnings:
  - Setting up a new repo from scratch via GitHub according to team standards.
  - Understand adapter/connector patterns to read from source databases and write to output tables.
  - Learned Spark / Scala on the job to implement the aggregation logic as part of a big data pipeline.
  - Practice testing a Spark job using BigRed3, Target's internal Hadoop data environment.