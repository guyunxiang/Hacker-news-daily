# Show HN: Open-Source Alternative to Mercury

**Posted by ben_talent on 2025-07-11**

Hi, I’m Ben.

Today, I want to share something I’ve been building over the past few months.

**0.finance** is an open-source bank account.

You might wonder what I mean by “bank account” or how this could even be possible. The term is used loosely here. Essentially, we provide a UI on top of a crypto wallet.

We partner with some "on-/off-ramp" providers to make it easy to expose virtual accounts, including ACH details, creating a bank-like experience for the end user. 

Under the hood, we leverage recent advances in crypto user experience to ensure you don’t need to manage private keys directly. From the user’s perspective, it feels much like a traditional bank.

### The Future

And that’s just a glimpse of what we’re working on. We’re in the process of building an automation layer to help manage your entire financial stack gradually. For example:

- We created a small Gmail connector that automatically categorizes receipts from your incoming emails.
- We parse emails to auto-populate wire transfers, making it easier to pay vendors.

**P.S.** It’s currently possible to self-host 0.finance (though it’s a bit painful right now). This means you could, in theory, get paid on our hosted instance, then fork the code and continue on your own path.