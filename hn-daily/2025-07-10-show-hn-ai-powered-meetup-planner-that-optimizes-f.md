# Show HN: AI-powered meetup planner that optimizes for fair travel times

**Posted by KApilmittal on 2025-07-10**

I got tired of the endless group chat debates about where to meet, especially when someone always ends up with a terrible commute while others walk five minutes.

So I built Midway@ — an AI that finds meeting spots where everyone's travel time is actually fair. It doesn’t just pick geographic midpoints (which are often terrible), but instead optimizes specifically for travel time equity.

## How it works:
- Enter each person’s starting location and preferred transport method (car/transit/walk/bike)
- Describe what you’re looking for (e.g., "coffee shop with WiFi," "restaurant with parking")
- AI analyzes thousands of venues using live traffic and transit data
- Returns locations where commute times are balanced across the group

## Technical details:
- Uses Google Maps APIs for real-time travel calculations
- Implements a custom algorithm that minimizes travel time variance within the group
- Handles mixed modes of transportation (some people drive, others take transit)
- Venue ranking considers both travel equity and suitability match

## Insights from over 10,000 groups:
- 67% of manually selected meetup spots have over 15 minutes of travel time imbalance
- The geographic center is the best location only 23% of the time
- Groups save an average of 47 minutes in coordination time

Built with Next.js and deployed on Vercel. I’d love to get feedback on the algorithm or UX improvements!

[Demo: midway.at](https://www.midway.at)