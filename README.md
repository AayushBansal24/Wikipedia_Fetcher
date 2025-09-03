# Wikipedia Fetcher API

This project provides a simple Java API to fetch and parse Wikipedia articles using HTTP requests and HTML parsing.

## Features

- Fetches Wikipedia article summaries.
- Uses Java's HTTP utilities and Jsoup for parsing.
- Returns results as Java objects.

## Main Files

- `WikiResult.java` — Data structure for Wikipedia results.
- `WikipediaDownloader.java` — Main logic for fetching Wikipedia articles.
- `HTTPUrlConnectionExample.java` — Helper for HTTP requests.
- `pom.xml` — Maven dependencies.

## Usage

Example usage in Java:
```java
WikiResult result = new WikipediaDownloader("Albert Einstein").getResult();
System.out.println(result.getText());
System.out.println(result.getImageUrl());
