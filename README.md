# ADK A2A Agent Quickstart

This repository is the companion to the [Surprisingly Simple A2A Agents with ADK using to_a2a()](https://mandieq.medium.com/surprisingly-simple-a2a-agents-with-adk-using-to-a2a-deploy-to-cloud-run-and-gemini-enterprise-e815bdef4a32) blog post. This shares the end to end process for creating an [Agent2Agent (A2A)](https://a2a-protocol.org/) agent using the [Agent Development Kit (ADK)](https://google.github.io/adk-docs/) framework. Specifically using the `to_a2a()` wrapper from ADK which makes this process super straightforward. I show how to deploy to [Google Cloud Run](https://docs.cloud.google.com/run/docs/overview/what-is-cloud-run) and, as a side mission, surface it within [Gemini Enterprise](https://cloud.google.com/gemini-enterprise) (Google’s AI platform for business users). 

Please see the blog for specifics of this repository's contents and deployment instructions.

## Configuration

When working with Vertex AI on Google Cloud, ADK requires a `.env` file with the following content:
```
GOOGLE_GENAI_USE_VERTEXAI=1
GOOGLE_CLOUD_PROJECT=<your-project-name>
GOOGLE_CLOUD_LOCATION=<your-region>
```
Application Default Credientials are a good way to authenticate locally for testing with ADK. See [Set up ADC for a local development environment](https://docs.cloud.google.com/docs/authentication/set-up-adc-local-dev-environment) for more details.

See the [ADK documentation](https://google.github.io/adk-docs/get-started/python/) for wider details of how to get started with ADK.

## Key framework versions used

```
a2a-sdk                                  0.3.25
google-adk                               1.28.0
google-cloud-aiplatform                  1.143.0
uvicorn                                  0.42.0
```

## Note

This is not an officially supported Google product. This project is not
eligible for the [Google Open Source Software Vulnerability Rewards
Program](https://bughunters.google.com/open-source-security).