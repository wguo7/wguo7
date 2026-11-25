## William Guo

Math and computer science student at the University of Chicago, class of 2029. I research AI agent security at XLab and build backend and infrastructure software, with [more than 90 merged pull requests](https://github.com/search?q=author%3Awguo7+is%3Apr+is%3Amerged+-user%3Awguo7&type=pullrequests) in open-source projects. I am looking for summer 2027 software engineering and research internships.

[williamguo.xyz](https://www.williamguo.xyz) | [LinkedIn](https://www.linkedin.com/in/william-guo-4ab71a263) | wguo4@uchicago.edu

### Open source
Most of the merged pull requests are in LLM inference infrastructure: [llm-d](https://github.com/llm-d) (router and inference simulator, 42), [vllm-project](https://github.com/vllm-project) (guidellm, aibrix, speculators, 35) and [ray](https://github.com/ray-project/ray) (9).

### Research
- [deferred-execution-attacks](https://github.com/wguo7/deferred-execution-attacks): 1st place at Uncommon Hacks 2026. AI control setups have a monitor approve each command an agent runs. This project shows an agent with shell access can install something that runs later, such as a cron entry or a systemd timer, so the harm happens only after the monitor has approved the session and stopped watching. It also contains a monitor that catches these attacks by following each installed trigger to the action it will run.
- [llm-cartel-monitoring](https://github.com/wguo7/llm-cartel-monitoring): do monitors catch LLM sellers that collude in an auction? Cartels coached on how to hide were not reliably caught by the LLM judges reading their messages and trades, but two simple price statistics still flagged every cartel that had not been told about them. Written for the Apart AI Collusion Research Sprint in October 2026.

### Systems
- [shop-chat-agent](https://github.com/wguo7/shop-chat-agent): the AI shopping assistant live on the NextLED Shopify store, where it handles 600+ shopper chats a month. It started from Shopify's open-source template; my work is the grounding in product manuals and the live catalog, the catalog search and pricing fixes, and the admin dashboard.
- [raft-kv](https://github.com/wguo7/raft-kv): a linearizable key-value store replicated with Raft, written in Go, with gRPC between nodes and a Porcupine linearizability check in the tests.
- [order-entry-service](https://github.com/wguo7/order-entry-service): a REST service for entering, amending, canceling and filling stock orders in Java 21, Spring Boot 3 and Postgres. Each create carries an idempotency key, each change locks the order's row, and every change goes to an audit log.
