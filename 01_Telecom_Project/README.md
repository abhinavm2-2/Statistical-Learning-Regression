# Beyond the R-Squared: A First Dive into Predicting Customer Value
*Exploring OLS Regression, Log-Transformations, and Business Inference in Telecom Data.*

### 📊 What the Data is Actually Telling Us

I built this model to see if we could predict a customer's value before they even think about leaving. After cleaning the data and fixing the math, here are the four "Aha!" moments:

* **The "SMS = Value" Signal:** 
    Every single text a user sends boosts their lifetime value by about **0.8%**. It’s a super clean, direct relationship. 
    * *Strategy:* If a user stops texting, they’re cooling off. We should nudge them the second their SMS count dips.

* **The "Long-Call" Disaster (Interaction Effect):** 
    I found a 'Frustration Multiplier'—the math proves that a dropped call during a long 20-minute session is exponentially more damaging to a customer's value than a quick 5-second glitch.
    * *Strategy:* We should have the AI send a huge apology and a credit specifically to people who got disconnected during a long, important call.

* **The "Loyalty Trap" (Tenure Paradox):** 
    Surprisingly, our oldest customers are worth **1.1% less** every month. They’re probably on old, cheap plans while using more resources.
    * *Strategy:* They are loyal, but we’re losing margin. Let’s offer them a "Modern Pro" upgrade so they’re actually profitable again.

* **My "Safety Buffer" Rule (Prediction Intervals):** 
    I learned that we can’t just guess what one person will do based on the "average." There's too much random human noise. 
    * *Strategy:* I calculated a "Worst-Case" prediction for every user. By using this "Safety Buffer," we can save customers before they even hit the danger zone.
