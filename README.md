# Challenge project - Add image analysis and generation capabilities to your application

[Challenge overview](https://learn.microsoft.com/en-us/training/modules/challenge-project-add-image-analysis-generation-to-app/)

This project is a web application built with Blazor. It uses the Azure OpenAI API  to analyze and generate images based on provided prompts and URLs.

## Prerequisites

* Azure account
* Either [Azure OpenAI endpoint](https://customervoice.microsoft.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR7en2Ais5pxKtso_Pz4b1_xUNTZBNzRKNlVQSFhZMU9aV09EVzYxWFdORCQlQCN0PWcu) and apiKey or [OpenAI API key](https://platform.openai.com/docs/overview).
* VS Code
* Docker
* Dev Containers extension for VS Code

## Helpful Links

* Image Analysis [Quickstart: Image Analysis 4.0 ](https://learn.microsoft.com/en-us/azure/ai-services/computer-vision/quickstarts-sdk/image-analysis-client-library-40?tabs=visual-studio%2Cwindows&pivots=programming-language-csharp)

* Generate images with Azure OpenAI Service [Quickstart: Generate images with Azure OpenAI Service ](https://learn.microsoft.com/en-us/azure/ai-services/computer-vision/quickstarts-sdk/image-analysis-client-library-40?tabs=visual-studio%2Cwindows&pivots=programming-language-csharp)


## Installing

1. Clone the repository.
2. Open the project in VS Code.
3. VS Code will prompt you to open the project in a dev container. Click 'Reopen in Container'.
4. Restore the packages: `dotnet restore`
5. Set your environment variables
    * OpenAI API key or Azure OpenAI API key: `export AZURE_OPENAI_API_KEY=<your_api_key>`
    * Azure OpenAI endpoint (if you're using Azure OpenAI): `export AZURE_OPENAI_ENDPOINT=<your_endpoint>`
    * Azure Computer Vision API key: `export VISION_KEY=<your_api_key>`
    * Azure Computer Vision endpoint: `export VISION_ENDPOINT=<your_endpoint>`
5. Code in Home.razor
6. Run the project locally using `dotnet watch` 
6. Run the project: `dotnet run`

## Packages used

* [Betalgo OpenAI](https://github.com/betalgo/openai)
* [Azure OpenAI](https://www.nuget.org/packages/Azure.AI.OpenAI/1.0.0-beta.10)
* [Azure.AI.Vision.ImageAnalysis](https://www.nuget.org/packages/Azure.AI.Vision.ImageAnalysis/0.15.1-beta.1)