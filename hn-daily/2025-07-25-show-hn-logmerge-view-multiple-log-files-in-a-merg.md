# Show HN: LogMerge – View multiple log files in a merged view

**Posted by faisalhackshah on 2025-07-25**

Hey HN!

I needed a tool to view multiple log files in a merged view and easily filter based on specified fields. After searching extensively, I couldn’t find any open-source tool that quite did what I wanted. So, I built a custom solution instead. I’d appreciate suggestions for tools with similar functionality.

I don’t have much experience with GUIs—most of my PC utilities are CLI-based—but I did have the following skills:
- Knowledge enough in Python to spot obvious issues
- Basic understanding of how to make programs performant
- Some tokens to burn :)

**GitHub:** [https://github.com/faisal-shah/pylogmerge](https://github.com/faisal-shah/pylogmerge)

**Usage Video:** [https://youtu.be/37V_kZO2TLA](https://youtu.be/37V_kZO2TLA)

## Key Features

- Merge and display multiple log files in a single, chronologically ordered view  
- Live log monitoring with auto-scroll  
- Add files individually or discover them recursively with regex filtering  
- Plugin-based system to support any log format (easy to extend!)  
- Filtering options: discrete values, numeric ranges, regex/text, and time-based queries  
- Color-coded file identification  
- Configurable columns and ordering  
- Built-in plugins for syslog, CANKing (CAN Bus monitoring tool), and a custom log format called dbglog

If you have any feedback or questions, let me know! Hope someone else finds it useful.