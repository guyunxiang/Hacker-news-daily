# Show HN: A different kind of AI Video generation

**Posted by fcpguru on 2025-06-26**

Hello! I'm Andrew Arrow, a developer and Final Cut Pro user. My history with FCP goes back many years. I briefly pursued a career in video editing but ultimately became a software developer. I purchased the full version of Final Cut Pro a long time ago, and to Apple's credit, I still have access to download it from the App Store on any Mac I use — probably 20 or 30 Macs over the years.

Recently, I downloaded FCP again and noticed the XML Export feature. 

Wow, there's a lot there. The XML format is extensive and detailed, capable of describing any timeline, effect, or animation imaginable. I started playing around with generating XML, and that experimental phase led to this project:

[GitHub README](https://github.com/andrewarrow/cutlass/blob/main/README.md)

Read through the go structs and XML tags. Keep going — the format is very sophisticated, and it never stops evolving. Apple's documentation is scattered and incomplete, and the XML can be finicky; a single wrong attribute can crash your import.

With Claude, or other AI models of your choice, you can have your AI write complex Go code using Cutlass. For example:

```go
// Generate a timeline with precise keyframe animations
video := fcp.Video{
    Ref: assetID,
    Offset: "0s",
    Duration: fcp.ConvertSecondsToFCPDuration(10.0),
    AdjustTransform: &fcp.AdjustTransform{
        Params: []fcp.Param{
            {
                Name: "position",
                KeyframeAnimation: &fcp.KeyframeAnimation{
                    Keyframes: []fcp.Keyframe{
                        {Time: "0s", Value: "0 0"},
                        {Time: "240240/24000s", Value: "100 50"},
                    },
                },
            },
        },
    },
}
```

I haven't been writing code like that manually. Instead, I tell Claude the video I want to create, and it utilizes the Cutlass library to accomplish it. I'm connecting FCP directly to Claude — a different kind of AI video generation.

Would love feedback. Thanks for reading this far!

— aa