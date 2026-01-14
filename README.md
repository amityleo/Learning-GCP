# 🚀 Google Cloud Vertex AI

Welcome to the beginner-friendly guide for navigating the Google Cloud Vertex AI ecosystem. This repository helps new users understand which product to use for their specific artificial intelligence and machine learning needs. Often people confused which product to use and what is the difference between the products within the vertex AI and different use cases. Hence I am preparing this guide to understand the difference between the product and simple word describtions.

## Vertex AI Studio

This one build for playground  to test the models like Gemini without writing any code itself. Mainly for trying out ideas for the product to check if that works for user use case. The UI looks like a simple prompt section and config section on the right to adjust the temperature to customize the reply.

![Screenshot of the project](images/test.png)

## Vertex AI Agent Builder

Create agent based on the documents we want it to access, for an example a chat bot or IVR system that can only access company documents and database to answer queries. This not only access the files and access the sites, it can also book the appointments based on the requests. Best use case would be creating a customer service chatbot or an internal research assistant that knows your private business data.

## Vertex AI Search

This provides the same kind of google search like capacity to access the company internal resources and use those resources. Think of this as "Google Search for your company." The user can give it the website URL or a folder of PDFs, and it builds a search bar for you. No difficult coding config required. 

## Model Garden on Vertex AI

A library of 150+ ready-to-use models. It’s like an app store for AI. This garden contains Google's models (Gemini), open-source ones (Llama), or specialized ones for medicine or coding.

## Vertex AI Workbench

This part of the Vertex AI used for coding in the environment like Jupyter Notebook. This build in environment allows the users to code for Data Science to transform the data and prepare for the model input. Best use case would be for someone who know codes and wants to clean data for their specific projects to build a custom models. 

## Vertex AI Pipelines

Vertex AI pipelines is that conveyor belt for Machine Learning. If the user build the model manually, it allows users to connect different tasks—like "Get Data," "Train Model," and "Deploy Model"—into one automated workflow. The pipeline work anatomy would be 

> Data Ingestion $\rightarrow$ Transformation $\rightarrow$ Training $\rightarrow$ Evaluation $\rightarrow$ Deployment (model registry $\rightarrow$ endpoints)

## Vertex AI Vector Search

There is an important concept to clarify, "Vector Search". This is the "engine" under the hood. It uses complex math to find "similar" things (like finding a photo of a cat because it's "mathematically similar" to a photo of a kitten). You only use this if you are a developer building a custom system. Consider this as a high-performance database designed to store and search through "vectors" (mathematical representations of data). Since it build for the "PRO" developer, the user has to do all the heavy lifting. The user must also manually turn your text/images into vectors (embeddings), manage the database, and write the code to retrieve them. The AI convert everything into vector to characterize the product.


## 🔍 Deep Dive: Understanding "Vectors"

Search in Vertex AI relies on the concept of **Vector Search**. Imagine you want to describe a fruit to a computer using only two numbers: Sweetness and Crunchiness.

**The Fruit Analogy:**

Imagine describing a fruit using only two numbers: **Sweetness** and **Crunchiness**.
* 🍎 **Apple**: Sweetness (8), Crunchiness (9) $\rightarrow$ Vector: `[8, 9]`
* 🍌 **Banana**: Sweetness (7), Crunchiness (1) $\rightarrow$ Vector: `[7, 1]`
* 🍐 **Pear**: Sweetness (7), Crunchiness (6) $\rightarrow$ Vector: `[7, 6]`

If we plot these on a graph, the Apple and the Pear will be physically closer to each other than to the Banana. In AI, this "closeness" on a graph means the objects are semantically similar. But this is a very simple example to understand the vector concept. Like this, all works and text input converted into the vector representation. 

Similarly below is the just an example of words representing as vector:
* **Word:** "Hello" $\rightarrow$ `[0.1, -0.2, 0.5]` 
* **Image:** Sunset $\rightarrow$ `[0.9, 0.1, -0.4]`
