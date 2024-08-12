# Addition of new promo/sale ending trigger message types

- Task: Introduce new trigger message types for expiring sales/promos on an item in a guest's cart.
- Importance: Our existing trigger messages were sent to a guest when an item in their cart qualified for a promo/sale. This change resulted in sending a different message to guests in the case that the promo/sale on the item in their cart was ending soon, impacting the sense of urgency to buy and increasing the message-to-sale conversion rate. 
- Learnings: 
  - Translate business requirements into logical code updates in our Kotlin-based triggers microservice triggers. 
  - Validated expected functionality of Kafka pipeline via logging.
  - Organized functional testing of various scenarios in our UAT environment to ensure a guest's selected message matched business expectations.