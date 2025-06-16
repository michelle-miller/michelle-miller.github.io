# Security and privacy for foundation models

Your work with foundation models is secure and private, in the same way that all your work on watsonx is secure and private. IBM cannot access your prompts or tuned models.

[<- Back](https://michelle-miller.github.io/user-help.html#target-diverse-learning-methods){: .amini}

The following table summarizes the privacy and security of your foundation model work in watsonx.

| Item | Accessible by you | Accessible by IBM or anyone else | Privacy and security details |
|------|-------------------|----------------------------------|------------------------------|
Prompt for foundation model input (text and parameters)	| Yes | No | - IBM does not use your work to improve IBM models.<br/> - Text that you add to or submit in the Prompt Lab or API is not stored unless you save it. <br/> - IBM does not monitor or log foundation model input. <br/> - If watsonx.governance is provisioned, you can optionally monitor foundation model input. |
| Prompt in transit | Not applicable | No | - Prompt remains encrypted while in transit. <br/> - The foundation models are hosted in IBM Cloud; your prompts are not sent to third-party platforms. |
| Foundation model output | Yes | No | - IBM does not monitor or log foundation model output. <br/> - Foundation model output is not stored unless you save the prompt that elicited the output as a prompt session asset. <br/> - IBM does not claim ownership rights to foundation model outputs. <br/> - IBM does not use your model outputs to improve IBM models. <br/> - If watsonx.governance is provisioned, you can optionally monitor foundation model output. |
| Prompt saved as a prompt template asset | Yes | No | - A saved prompt template asset is stored in a dedicated, secure storage bucket.
| Prompt saved as a prompt session asset | Yes | No | - A saved prompt session asset is stored in a dedicated, secure storage bucket.
| Prompt saved as a notebook asset | Yes | No | - A saved notebook asset is stored in a dedicated, secure storage bucket.
| Prompt Lab text in web browser cache | Not applicable | No | - Unsaved prompt text is kept in the web page until the session expires or the page is refreshed, at which time the prompt text is deleted. <br/> - You can delete the browser cache. |
| Tuned foundation model | Yes | No | - Your tuned model is saved as a model asset and is stored in a dedicated, secure storage bucket. <br/> - Your tuned foundation model is not accessible or used by IBM or any other person or organization. <br/> - IBM does not use your tuning experiment work to improve IBM models. |
| Tuning experiment | Yes | No | - Your tuning experiment is saved as an experiment asset and is stored in a dedicated, secure storage bucket. |
| Training data for tuning | Yes | No | - The training data that you use for training is saved as a data asset and is stored in a dedicated, secure storage bucket. |
{: .tableimg}

## Foundation model privacy and security

Foundation models that you interact with through watsonx are hosted in IBM Cloud. Your data is not sent to any third-party or open source platforms.

The foundation model prompts that you create and engineer in the Prompt Lab or send by using the API are accessible only by you. Your prompts are used only by you and are submitted only to models you choose. Your prompt text is not accessible or used by IBM or any other person or organization.

The tuned foundation models that you create in Tuning Studio or by using the API are accessible only to you. Your tuned foundation models are not accessible or used by IBM or any other person or organization.

You control whether prompts, model choices, and prompt engineering parameter settings are saved. When saved, your data is stored in a dedicated IBM Cloud Object Storage bucket that is associated with your project.

The tuning experiment, tuning parameters, and training data that you use to tune a foundation model are accessible only by you. Tuning experiment and training data assets that you create are stored in your project storage bucket.

Metadata about your data assets is stored in a multi-tenanted database. Metadata includes the asset name, description, and tags. The asset data itself is stored in a single-tenant instance of an IBM Cloud Object Storage bucket that is associated with your account and is not shared. Each bucket in the instance is further isolated by permissions. Two projects that use the same IBM Cloud Object Storage instance cannot view each other’s asset data, for example. Data that is stored in your project storage bucket is encrypted at rest and in motion, optionally with your own key. You can delete your stored data at any time by deleting the associated asset from your project or by deleting the project.

IBM does measure foundation model usage by account for the purposes of billing, infrastructure planning, and model lifecycle management.

## Privacy of text in Prompt Lab during a session

Text that you submit by clicking **Generate** from the prompt editor in Prompt Lab is reformatted as tokens, and then submitted to the foundation model you choose. The submitted message is encrypted in transit.

Your prompt text is not saved unless you choose to save your work. Unsaved prompt text is kept in the web page until the session expires or the page is refreshed, at which time the prompt text is deleted.

## Privacy and security of saved work in Prompt Lab

How work that you save in the Prompt Lab is managed differs based on the asset type that you choose to save:

- Prompt template asset: The current prompt text, model, prompt engineering parameters, and any prompt variables are saved as a prompt template asset and stored in the IBM Cloud Object Storage bucket that is associated with your project. For a prompt that you create in chat mode, the foundation model output is saved also. Prompt template assets are retained until they are deleted or changed by you. When autosave is on, if you open a saved prompt and change the text, the text in the saved prompt template asset is replaced.

- Prompt session asset: A prompt session asset includes the prompt input text, model, prompt engineering parameters, and model output. After you create the prompt session asset, prompt information for up to 500 submitted prompts is stored in the project storage bucket where it is retained for 30 days.

- Notebook asset: Your prompt, model, prompt engineering parameters, and any prompt variables are formatted as Python code and stored as a notebook asset in the project storage bucket.

Only people with Admin or Editor role access to the project or the project storage bucket can view saved assets. You control who can access your project and its associated Cloud Object Storage bucket.

## Logging and text in the Prompt Lab

Nothing that you add to the prompt editor or submit to a model from the Prompt Lab or by using the API is logged by IBM. Messages that are generated by foundation models and returned to the Prompt Lab are also not logged.

## Ownership of your content and foundation model output

Content that you upload into watsonx is yours.

IBM does not use the content that you upload to watsonx or the output that is generated by a foundation model to further train or improve any IBM-developed models.

IBM does not claim to have any ownership rights to any foundation model outputs. You remain solely responsible for your content and the output of any tuned or untuned foundation models that you work with in watsonx.

## Privacy and security in watsonx.governance

If watsonx.governance is provisioned, you can choose to enable evaluation and monitoring of foundation models to support governance functions such as drift detection and explainability. When enabled, the request payloads of foundation model input and output are stored in a watsonx.governance database that you administer.

You own the data in the database and you control who is allowed to access the data. To meet added encryption or access control needs, you can choose a setup method that gives you more control over the database and deployment space assets that are used.

Any stored data is purged when monitoring is disabled or when the monitored prompt template asset or model deployment is deleted.