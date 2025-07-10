# Show HN: A CUDA-Generating AI Agent

**Posted by atallahw on 2025-07-09**

MakoGenerate is an AI agent designed to convert any PyTorch code into optimized CUDA kernels. 

The process works as follows:  
- You can select a sample problem or input your own PyTorch code.  
- The agent generates CUDA kernels based on the input.  
- It compiles and validates the generated code.  
- Feedback from validation is used to improve subsequent attempts.  
- If the kernel doesn't work, the agent tries to fix it.  
- If it succeeds, it works to optimize the kernel further for speed.

You can configure the agent with specific model, hardware, or compute budget parameters. Additionally, there's an optional custom prompt feature, allowing you to add context—such as documentation, tutorials, or specific optimization techniques you want applied. Prompts can range from a single line to multiple pages.

Let me know what you think!