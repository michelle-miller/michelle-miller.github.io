# Technical documentation

Find samples of help content for software users with various roles and experience levels.

- [User help](#product-user-help)
- [Developer help](#developer-help)
- [Administrator help](#administrator-help)

## User help

As a lead writer for the IBM watsonx.ai product, I created content that helped customers use foundation models in IBM watsonx.ai to improve their day-to-day business operations with generative AI.

The following table has links to content that was written by me and that illustrates various approaches for providing straight-forward, helpful information.

| Writing approach | Examples |
|------------------|----------|
| Incorporate images in conceptual information to illustrate concepts and explain processes. | [Model parameters for prompting (PDF)](https://michelle-miller.github.io/samples/wx-llm-parameters-sample.pdf){:target="_blank"} |
| Focus on user goals, not product features. | The following two samples show content for a tool called Content Miner in IBM Watson Discovery that I revised to be task-based:<br/> - [Before](https://michelle-miller.github.io/samples/contentmine-before.pdf)<br/> - [After](https://michelle-miller.github.io/samples/contentmine-after.pdf) |
| Describe and compare available options to help customers make good choices. | [Methods for tuning foundation models (PDF)](https://michelle-miller.github.io/samples/wx-tuning.pdf){:target="_blank"} |
| Single-source user content when possible to save time and resources. | The following online topics are single-sourced in Markdown:<br/> - Software as a Service: [Supported foundation models](https://www.ibm.com/docs/SSYOK8/wsj/analyze-data/fm-models.html){:target="_blank"}<br/> - On premises: [Supported foundation models](https://www.ibm.com/docs/SSLSRPV_latest/wsj/analyze-data/fm-models.html){:target="_blank"} |
| Write content that can be consumed by LLMs as part of a retrieval-augmented generation (RAG) pattern to return factual answers. | I authored content such that it could be returned in the IBM watsonx.ai LLM-based search app and regularly reviewed results and user feedback to improve content findability.<br/>Try it out: [Find information](https://dataplatform.cloud.ibm.com/docs/content/wsj/getting-started/welcome-main.html?context=wx){:target="_blank"}. |
{: caption="Documentation best practices" caption-side="bottom"}

Previous projects include product documentation for cloud services that help customers with search tasks and building chatbot dialogs.

- [IBM Watson Discovery](https://michelle-miller.github.io/samples/discovery-data-sample.pdf){:target="_blank"}
- [IBM Watson Assistant](https://cloud.ibm.com/docs/assistant?topic=assistant-index){:target="_blank"}

## Developer help

The following guidance augments the watsonx.ai API reference documentation:

- [Time series forecasting](https://michelle-miller.github.io/samples/wx-time-series-api-sample.pdf){:target="_blank"}
- [Reranking document passages](https://michelle-miller.github.io/samples/wx-rerank-api-sample.pdf){:target="_blank"}

This content helps low-code users implement a simple RAG pattern and chat about images:

- [IBM watsonx.ai: Chatting about documents and images](https://michelle-miller.github.io/samples/wx-chatting-sample.pdf){:target="_blank"}

These SpEL expression language descriptions and examples help chatbot builders implement more advanced logic in their dialog flows:

- [IBM Watson Assistant: Expression language methods](https://cloud.ibm.com/docs/assistant?topic=assistant-dialog-methods){:target="_blank"}

### API reference

This API reference is sourced from a JSON file that conforms to the OpenAPI specification:

- [Discovery API reference](https://cloud.ibm.com/apidocs/discovery-data){:target="_blank"}

Supplemental guidance for developers is available from the product documentatation. For example, [IBM Watson Discovery: Query overview](https://cloud.ibm.com/docs/discovery-data?topic=discovery-data-query-concepts){:target="_blank"}.

## Administrator help

The following content helps administrators install and manage the on-premises deployment of the IBM Watson Discovery service. The content is written in DITA with Oxygen XML Author.

- [Installing and administering IBM Watson Discovery in IBM Cloud Pak for Data](https://michelle-miller.github.io/samples/CP-Data-4.7.x-Admin-Disco.pdf){:target="_blank"}
