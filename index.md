# Technical documentation

As a lead technical writer for IBM Data and AI and IBM Cloud software services, I created content that helped customers complete goals such as these:

- Use foundation models in IBM watsonx.ai to improve day-to-day business operations with generative AI. See [IBM watsonx.ai](https://www.ibm.com/docs/SSYOK8/wsj/analyze-data/fm-overview.html){:target="_blank"}.
- Analyze and visualize enterprise data. See [IBM Watson Discovery](https://cloud.ibm.com/docs/discovery-data?topic=discovery-data-about){:target="_blank"}.
- Build AI chatbots. See [IBM Watson Assistant](https://cloud.ibm.com/docs/watson-assistant?topic=watson-assistant-about){:target="_blank"}.

Find samples of help content for software users with various roles and experience levels.

- [UI content](user-interface-content)
- [User help](#user-help)
- [Developer help](#developer-help)
- [Administrator help](#administrator-help)

## User interface content

| Tooltips | ![Foundation model benchmark summary](https://michelle-miller.github.io/samples/ui-help-metrics-def.png)<br/>Keep helpful information in reach whenever possible. |
| *Learn more* links | ![Learn more link from the model parameters pane](https://michelle-miller.github.io/samples/progressive-disclosure-model-params.png)<br/>Implement a progressive disclosure model that lets users control when they get more information. |
| UI walkthroughs | ![Comments for the designer about a description for an Agent Lab screen](https://michelle-miller.github.io/samples/agent-lab-add-tools.png) <br/>Walkthroughs are a great way for users to get familiar with new tools. |
| Collaboration in Figma | ![language suggestions made to the designer in Figma](https://michelle-miller.github.io/samples/agent-lab-desc.png)<br/>Work with UI designers to craft UI language that supports the task workflow. |
{: caption="UI content examples" caption-side="bottom"}

## User help

The following table has links to content that was written by me and that illustrates various approaches for providing straight-forward, helpful information.

Note: Most of the content is shared as PDFs rather than links to online help pages so that I can illustrate *my* work and distinguish it from work that other writers are contributing to the current online help content.

| Writing approach | Examples |
|------------------|----------|
| Incorporate images in conceptual information to illustrate concepts and explain processes. | [Parameters for prompting foundation models](https://michelle-miller.github.io/samples/wx-llm-parameters-sample.pdf){:target="_blank"} |
| Focus on user goals, not product features. | The following two samples show content for a tool called Content Miner in IBM Watson Discovery before and after I revised the information to be task-based:<br/> [Before](https://michelle-miller.github.io/samples/contentmine-before.pdf) & [After](https://michelle-miller.github.io/samples/contentmine-after.pdf) |
| Describe and compare available options to help customers make good choices. | [Methods for tuning foundation models](https://michelle-miller.github.io/samples/wx-tuning.pdf){:target="_blank"} |
| Single-source user content when possible to save time and resources. | The following online topics are single-sourced in Markdown:<br/> - Software as a Service: [Supported foundation models](https://www.ibm.com/docs/SSYOK8/wsj/analyze-data/fm-models.html){:target="_blank"}<br/> - On premises: [Supported foundation models](https://www.ibm.com/docs/SSLSRPV_latest/wsj/analyze-data/fm-models.html){:target="_blank"} |
| Write content that can be consumed by LLMs as part of a retrieval-augmented generation (RAG) pattern to return factual answers. | I optimized the documentation for retrieval by the IBM watsonx.ai LLM-based search app and regularly reviewed search results and user feedback to improve how the help content performs.<br/>Try it out: [Find information](https://dataplatform.cloud.ibm.com/docs/content/wsj/getting-started/welcome-main.html?context=wx){:target="_blank"} |
{: caption="Documentation best practices" caption-side="bottom"}

## Developer help

I created the following guidance to augment the watsonx.ai API reference documentation:

- [Time series forecasting](https://michelle-miller.github.io/samples/wx-time-series-api-sample.pdf){:target="_blank"}
- [Reranking document passages](https://michelle-miller.github.io/samples/wx-rerank-api-sample.pdf){:target="_blank"}

This content helps low-code users implement a simple RAG pattern and chat about images:

- [IBM watsonx.ai: Chatting about documents and images](https://michelle-miller.github.io/samples/wx-chatting-sample.pdf){:target="_blank"}

These SpEL expression language descriptions and examples help chatbot builders implement more advanced logic in their dialog flows:

- [IBM Watson Assistant: Expression language methods](https://michelle-miller.github.io/samples/assistant-spel-sample.pdf){:target="_blank"}

### API reference

I created this API reference from a JSON file that conforms to the OpenAPI specification:

- [Discovery API reference](https://cloud.ibm.com/apidocs/discovery-data){:target="_blank"}

I added supplemental guidance to the product documentatation to help developers use the API effectively, such as [IBM Watson Discovery: Query overview](https://michelle-miller.github.io/samples/discovery-data-query-api-sample.pdf){:target="_blank"}.

## Administrator help

The following content helps administrators install and manage the on-premises deployment of the IBM Watson Discovery service. The content was written in DITA with Oxygen XML Author.

- [Installing the IBM Watson Discovery service in IBM Cloud Pak for Data](https://michelle-miller.github.io/samples/CP-Data-4.7.x-Admin-Disco.pdf){:target="_blank"}
