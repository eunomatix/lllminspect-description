<div align="center">
  <img width = "25%" src="https://eunomatix.com/img/logo-meerkat-llminspect-black-small.png">
</div>
![Alt text](./resources/splash.png?raw=true "Title")

![screenshot](resources/splash.png)
<img src="resources/splash.png" width="128"/>

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=sass,docker,aws,gcp,openshift,kubernetes,redhat,ubuntu,windows&theme=light" />
  </a>
</p>


## What is LLMInspect
With the rise of GenAI, most of the enterprises want to use LLMs to enhance their productivity, by enabling their employees to grant them access to public LLM providers (like ChatGPT, Gemini, etc). Though this definitely improves the overall productivity of the employees in their routine operations, however this capability posses several threats to the enterprise as mployees are sharing the intellectual property of the organization with these public entities, and thus opening a new avenue of data leakage threats.

**LLMInspect** GenAI Gateway is a one stop solution to all those problems, as it massively enhances the enterprise AI experience and cyber safety. From one application users can interact with different public and private LLM models, and control what is being sent to these models. Using **LLMInspect**, SOC Analysts can also view the employee GenAI usage and discover any LLM related Security Threats. **LLMInspect** also brings very interesting capabilities to its users, e.g. rate limit the GenAI queries or even re-route external LLM queries to enterprise's private LLMs.

**LLMInspect** is a comprehensive system for managing large language models and their related services. The `eunomatix/llminspect` repository contains submodules for various microservices required for this product, alongside a `docker-compose.yml` file and an example override file.

## LLMInspect Architecture
LLMinspect is designed from the ground up keeping in mind the requirements of modern enterprise deployments. Based on the principles of service-oriented architecture LLMinspect can be comfortably deployed both in the cloud and on prem. LLMinspect enables clients from various modalities to interact with public LLM providers in a safe and secure manner such as chat clients using our flexible web interface which allows a user to fully exercise various features of LLMs for example conversational AI image generation, code generation and retrieval augmented generation. Regardless of the source all LLM interactions are guarded and logged by LLMInspect. 

Once the requests reach LLMInspect , LLMinspect masks all personally identifiable information so that such information will not leave the enterprise premises in parallel our sentiment analysis service detects and logs the sentiment of the text. During this process detailed logs, chat text , images as well as transaction metadata are kept for analysis in the InspectDB service. SIEM dashboards provide by LLMinspect enable SOC analysts to analyze this information. Finally, the masked text is sent to the upstream LLM of user’s choice.    
![image](https://github.com/user-attachments/assets/e79da9dd-167f-4095-a3c1-8945756423f5)

LLMinspect provides dedicated desktop and mobile clients for easy interaction with LLMs and freedom from the browsers.
![image](https://github.com/user-attachments/assets/ca9a1b43-e2fd-4932-ad0a-82c371eb7038)

Llminspect operated without the need for clunky web proxies, enables end-users to choose their desired models, maintains indefinite chat history for each user. LLMinspect provides subscription aggregation across an enterprise to reduce cost. Llminspect is also able to rate limit LLM interactions. Finally the user may export their chat into a separate document.
![image](https://github.com/user-attachments/assets/9193aded-47a0-4eba-a54a-25b4fb3cb521)

It’s a ChatGPT Type user-friendly interface and easy adaptable by users.You can select different on-perm and public LLMs of your own choice.
![image](https://github.com/user-attachments/assets/53e7e9dd-ab55-4c6c-91c8-cc1c2e86880f)


![image](https://github.com/user-attachments/assets/70611f4d-3f3c-43b9-b455-809a6e63380a)

## LLMInspect & RAG
LLMinspect supports retrieval augmented generation in various modalities. A user can upload custom documents to enhance an LLMs response or process a document alternatively it also provides an identity aware RAG called secureRAG. SecureRAG supports separation of concern between different organizational units in conjunction with the enterprise identity provider to ensure that document access is secure and only authorized users are able to access documents in the RAG store.
![image](https://github.com/user-attachments/assets/1684be29-2272-40c2-b161-385c71424288)

## LLMInspect Guardrails
LLMINSPECT now supports multiple Guardrails to detect, quantify and mitigate the presence of specific types of AI risks including prompt injection, PII/BII Masking, LLM DDoS and Negative Business Sentiments inline with MITRE ATLAS Framework; and supports Guardrails AI integration
![image](https://github.com/user-attachments/assets/6ff35155-8a91-4ca9-a85c-70512417f68a)

# LLMInspect Integration with Splunk
To increase observability effectiveness Llminspect provides plugins for easy integration with splunk and elastic. These plugins reduced the need for custom tooling and seamlessly integrate with existing SOC (security operation center) solutions.

# LLMInspect Dashboards
