# Show HN: Zero Waste Cloud – Finds 20-40% savings in AWS/GCP bills and CO2 impact

**Posted by Suedish on 2025-07-31**

Hey HN! I'm Mike, based in Stockholm, Sweden, and I’m the founder of Zero Waste Cloud ([zero-wastecloud.io](https://zerowastecloud.io)). It’s a tool that scans AWS and GCP infrastructure to identify cost optimization opportunities while calculating the environmental impact. Almost all businesses can save 20-40% of their cloud costs using this tool (sources at bottom).

## TL;DR
Sign up → Connect your AWS/GCP → Scan → Save 20-40% of your cloud spend.

## My Backstory
I’ve been a CISO and in IT management for a long time, constantly frustrated by the amount of waste in every environment—idle EC2 instances running 24/7, oversized RDS databases, forgotten storage volumes, test resources that never get removed. What bothered me also was that no one was tracking the environmental cost of this waste. Every unused resource consumes electricity and contributes to carbon emissions unnecessarily.

## What It Does
- Scans AWS accounts via IAM roles or access keys and GCP projects via service account keys.
- Identifies specific optimization opportunities, including unused EC2/Compute Engine instances, oversized databases, unattached storage, missed reservation opportunities, and more.
- Calculates financial savings and CO₂ reduction for each recommendation using region-specific grid emission factors.
- Supports multi-account and multi-project setups.
- Generates detailed, prioritized reports with actionable recommendations.

## Technical Details
Built with React/TypeScript for the frontend and Supabase for the backend. Uses AWS SDK for EC2, RDS, and Cost Explorer APIs, and GCP’s Compute Engine, Cloud SQL, and Cloud Billing APIs. The carbon impact calculations combine cloud provider PUE data with regional electricity grid emission factors from government sources.

## Try It Out
The onboarding process—from creation to your first scan—is only about 30 seconds. The scan itself is fully automated and typically completes within 5-30 minutes, depending on the size of your cloud environment. 

I’d love to hear your feedback—it just came out of beta a few days ago. If you find any bugs or have suggestions, please let me know!

## Connect
If you’re on LinkedIn, let’s connect: [https://www.linkedin.com/in/almstedt/](https://www.linkedin.com/in/almstedt/)

## Sources
- "Companies estimate that 21-50% of their cloud expenditure is wasted"  
  [https://www.techmonitor.ai/hardware/cloud/cloud-waste-hits-billions-as-78-of-firms-report-significant-expenditure-losses](https://www.techmonitor.ai/hardware/cloud/cloud-waste-hits-billions-as-78-of-firms-report-significant-expenditure-losses)

- "45% of cloud customer’s expenditures are spent on resources they will never use"  
  [https://www.sciencedirect.com/science/article/abs/pii/S2210537922000476](https://www.sciencedirect.com/science/article/abs/pii/S2210537922000476)

- "21% of enterprise cloud infrastructure spend in 2025 is wasted on underutilized resources"  
  [https://www.prnewswire.com/news-releases/44-5-billion-in-infrastructure-cloud-waste-projected-for-2025-due-to-finops-and-developer-disconnect-finds-finops-in-focus-report-from-harness-302385580.html](https://www.prnewswire.com/news-releases/44-5-billion-in-infrastructure-cloud-waste-projected-for-2025-due-to-finops-and-developer-disconnect-finds-finops-in-focus-report-from-harness-302385580.html)