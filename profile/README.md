## Hi there 👋

our projects:

- LLM + LoRA: [DevTi](https://github.com/unit-mesh/devti)
- IDE plugin: [AutoDev](https://github.com/unit-mesh/auto-dev)
- VS Code plugin: [auto-dev-vscode](https://github.com/unit-mesh/auto-dev-vscode)

会议相关问题 --> [QCon](https://github.com/unit-mesh/conf)

```mermaid
sequenceDiagram
    participant Source Code
    participant Unit PreProcessor
    participant GPT
    participant Custom LLM
    participant Unit Prompter
    participant Unit Runtime
    participant Human

    Source Code->>+Unit PreProcessor: Source code
    Unit PreProcessor->>+GPT: Processed code
    GPT-->-Custom LLM: Data cleaned
    Unit Prompter->>+Custom LLM: Lora
    Human->>+Unit Runtime: Requirements
    Unit Runtime->>+Custom LLM: Prompt
    Custom LLM->>-Unit Runtime: Code snippets (Unit)
    Unit Runtime->>-Human: Services, component  (Unit)
    Human->>+Human: Test, verify and modify code (Unit)
    Human->>+SCM: Push code
```


<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
