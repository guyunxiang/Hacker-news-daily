# Production Data Access Is Broken for L3 Incidents

**Posted by addieg on 2025-07-09**

It's 2 AM, your biggest customer is down, and support knows exactly which database query will resolve the issue. 

But first: you need to write a sanitization script, get legal approval, provision replica access, and then wait for queries on a 20-minute-lagged replica, which takes 8 minutes per query. 

Three hours later, support finally begins debugging. The actual fix takes just 30 minutes. Meanwhile, your SLA has already been missed.

You're caught in a frustrating cycle: either you're the engineer frantically writing data masking scripts while a customer is losing money, or you're the support person who knows the exact query to run but can't safely touch production data.

We spend more time gaining access to the data than actually fixing the problem. The entire system feels backwards.

Does anyone else deal with this madness? Or have you found a way that doesn't suck?