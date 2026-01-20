# API Support for Flexible Task Configuration

To enable more flexible task configurations, TaskOn provides two types of APIs: one for verifying user task completion and another for determining the number of points to be awarded. These APIs allow project teams to deeply integrate their task systems with custom business logic, enabling tailored task and incentive structures.



1. ✅ **User Task Completion Verification (Check API)**<br>

This API is used to notify TaskOn whether a specific user has completed a task, ideal for scenarios where task completion can only be validated by the project team.<br>

**Common Use Cases**:

* Users complete actions within the project’s system, such as registering an account, passing verification, or reaching a specific level.
* Users perform on-chain actions, such as staking, minting, or voting.
* Task completion requires cross-platform or multi-step validation, which must be uniformly assessed by the project team.\
  When a user clicks _Verify_, TaskOn sends user information to your API, and you return the task status. If validated, the user receives a completion mark.



1. 🎁 **User Reward Distribution Confirmation (Reward API)**<br>

This API facilitates the distribution of specified point rewards to users upon task completion, suitable for scenarios where you wish to control the reward distribution logic.

\
**Common Use Cases**:

* **Trading Competitions**: You host an incentive campaign based on trading volume, distributing point rewards according to users’ trading performance.
* **Referral Campaigns**: You create a “referral registration” task, awarding points based on the number of successful referrals per user.
* **Daily Check-in Tasks**: Users complete daily check-ins, with rewards determined by consecutive check-in days (e.g., 10 points for 3 consecutive days, 30 points for 7 consecutive days).
* **Contribution Incentives**: Users engage in activities like posting or answering questions in communities or forums, tracked by your backend. When claiming rewards, points are awarded based on their recorded activity level.\
  When a user clicks _Verify_, TaskOn sends user information to your API, and you return the points the user should receive.
