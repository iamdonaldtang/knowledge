# API Task Support

To enable more flexible task configurations, TaskOn provides two types of APIs: one to determine whether a user has completed a task and another to specify the number of points to be awarded. These APIs allow project teams to deeply integrate the task system with their business logic, enabling customized task and reward rules.

1. ✅ **User Task Completion Status Check (Check API)**\
   This API informs TaskOn whether a specific user has completed a task, ideal for scenarios where only the project team can verify task completion.\
   Common use cases include:
   * Users completing actions within the project team’s system, such as registering an account, passing verification, or reaching a specific level.
   * Users performing on-chain actions, such as staking, minting, or voting.
   * Task completion requiring cross-platform or multi-step verification, which the project team must validate.\
     When a user clicks _Verify_, TaskOn sends user information to your API, and you return the task status. If validated, the user receives a completion mark.
2. 🎁 **User Reward Distribution Confirmation (Reward API)**\
   This API distributes specified point rewards to users upon task completion, suitable for scenarios where you want to control the reward distribution logic.\
   Common use cases include:
   * **Trading Competitions**: You host an incentive campaign based on trading volume, requiring point rewards based on users’ trading performance.
   * **Referral Campaigns**: You set up a “referral registration” task, distributing points based on the number of successful referrals per user.
   * **Daily Check-in Tasks**: Users complete daily check-ins, with rewards determined by consecutive check-in days (e.g., 10 points for 3 consecutive days, 30 points for 7 consecutive days).
   * **Contribution Incentives**: Users engage in community or forum activities like posting or answering questions, tracked by your backend. When claiming rewards, points are awarded based on their recorded activity level.\
     When a user clicks _Verify_, TaskOn sends user information to your API, and you return the points the user should receive.
