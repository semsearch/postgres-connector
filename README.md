# Semantic Search API Service

The Semantic Search API Service simplifies the integration of advanced semantic search capabilities into your applications. By effortlessly setting up a semantic search endpoint, powered by PostgreSQL and OpenAI, you can retrieve contextually relevant information from your indexed data.

## Semantic Search: A Smarter Way to Retrieve Information

Semantic search is an innovative approach to information retrieval that goes beyond the limitations of traditional text-based search. Unlike traditional search methods, which rely on keyword matching, semantic search understands the context and intent behind user queries. This enables the service to deliver more accurate and contextually meaningful search results, providing users with the information they need even when the exact keywords aren't present.

## Why Semantic Search Matters

Semantic search offers several advantages over traditional text search:

- **Contextual Relevance**: Semantic search considers the context of a query, ensuring that search results are more relevant to the user's intent.
- **Natural Language Processing**: The integration of OpenAI's technology empowers the service to comprehend and interpret natural language, making searches more intuitive and user-friendly.

- **Reduced User Effort**: Users can express their queries more naturally, eliminating the need for precise keyword matching.
- **Better Information Discovery**: Semantic search can unearth hidden relationships between concepts, helping users discover information that may have been missed with traditional methods.

## Getting Started

1. **Fork and Clone the Repository**: Start by forking the Git repository and cloning it to your local machine.

2. **Install Docker**: Ensure you have Docker installed on your system. If not, you can download and install it from [Docker's official website](https://www.docker.com/get-started).

3. **Configure Environment Variables**: In the project directory, locate the `.env` file, and fill in the required environment variable values.

4. **Define Indexed Table**: In the `.env` file, specify the PostgreSQL table you want to index and the corresponding columns for semantic search.

5. **Configure OpenAI API key**: Also in the `.envz file, specify your OpenAPI key. The service uses OpenAPI embedding model _text-embedding-ada-002_.

6. **Launch the Service**: Run `docker-compose up -d` in your terminal to start the service.

7. **Access the Search Endpoint**: Utilize the search endpoint via HTTP at `localhost:5000/query?q=<search phrase>` requests to experience the benefits of semantic search. The endpoints retruns the top 10 results matching the search phrase.

Eample usage:

```bash
curl http://localhost:5000/query?q=I want to keep my beer cool at the park
```

**Remember, while we provide the tools and infrastructure to enable semantic search, you'll need to provide your own OpenAI API key. This key is used to generate embeddings and enhance your search experience. Please note that you'll be responsible for any costs associated with using the OpenAI API for embeddings.**

## Expanding the Possibilities

The PostgreSQL connector is just the beginning. We are committed to expanding the capabilities of the Semantic Search API Service, enabling you to seamlessly integrate semantic search into various platforms. Whether you're building apps, websites, online stores, or any other digital experience, we will be introducing additional features to make the process even easier. For more information visit [semsearch.org](https://www.semsearch.org/).

## User-Friendly Managed Service Coming Soon!

We're thrilled to announce an upcoming addition to our Semantic Search API Service: a fully managed service experience with an intuitive user interface. We understand that not everyone wants to deal with technical complexities, which is why we're making it incredibly easy for anyone to harness the power of semantic search.

Soon, you'll be able to add advanced search capabilities to your apps, websites, and more, regardless of your technical background. With our managed service, setting up semantic search will be a breeze, and you'll be able to provide your users with accurate and contextually relevant search results effortlessly.

**If you want to hear more and join our SaaS beta let us know at** beta@semsearch.org.

Stay tuned for updates as we roll out more integrations, enhancements, and the fully managed service experience.

## License

This project is licensed under the MIT License. For details, see the [LICENSE](link-to-license-file) file.

---

Elevate your application's search capabilities with the Semantic Search API Service. Semantic search, driven by context and natural language understanding, revolutionizes information retrieval, offering a more intuitive and effective way to find relevant content. Start enhancing your search functionality today!

For more information and support, contact us at contact@semsearch.org.
