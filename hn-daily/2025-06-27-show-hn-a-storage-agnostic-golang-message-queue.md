# Show HN: A Storage-Agnostic Golang Message Queue

**Posted by fahimfaisaal on 2025-06-27**

Hello, everyone.

Three months ago, I started building my first GoLang package, VarMQ. In this short period, it gained significant traction from the community, earning over 140 stars on GitHub.

A week ago, to evaluate its performance, I ran benchmarks comparing it to Pond, a package that's been maintained for years. While Pond is not a message queue, it shares some similarities with VarMQ, especially in terms of storage system differences.

The benchmark results were surprising: VarMQ uses more than 50% less memory than Pond and demonstrates strong performance in I/O tasks. I’m glad to share these results with the community.

You can view the benchmark chart here: [https://varmq-benchmarks.netlify.app](https://varmq-benchmarks.netlify.app)

My goal is to increase adoption of this package, and I welcome any feedback. If you like this project, please consider starring it—your support helps it grow.

Thank you!