# LLMs don't understand my code, cuz I didn't comment  
**Posted by fdlinly on 2025-06-20**

Wanted to share this small but mighty lesson with y'all.

I wrote a clever code to solve a problem using a greedy approach, and had GPT, Gemini, and Claude review it. Gemini said my code is functionally correct but the logic isn't right. The other two LLMs said my code was wrong, even though my code produced correct outputs for all of their test cases.

Thankfully, I trusted my judgment, reviewed my logic again, and started adding comments. After doing so, they finally understood. All of them agreed that it's a smart approach and 100% correct.

**Lesson:** Always comment your code! Not just for your future self, but also for LLMs. Plus, it helps reduce unnecessary inference costs by avoiding endless back-and-forth clarifications.