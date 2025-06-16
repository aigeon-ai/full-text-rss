markdown
# Full-Text RSS MCP Server

## Overview

The Full-Text RSS MCP server is a powerful tool designed to extract full-text articles from news sites and blogs. It simplifies the process of obtaining article content from web pages, providing clean and usable plain text or HTML for further use. This server employs a combination of automatic content detection and site-specific extraction rules to ensure accurate and reliable results.

## Features

### 1. Article Extraction

- **Extract Article**: This tool allows you to extract the full content of an article from a web page. The output is provided in JSON format, containing the complete content extracted from the input URL or HTML.

### 2. Feed Conversion

- **Convert Feed**: This feature enables the conversion of partial feeds into full-text feeds. It outputs an RSS 2.0 feed, either in XML or JSON format, containing the complete content extracted from the input URL. The input can be either a partial feed or a standard web page.

## Tool Descriptions

### Extract Article

- **Function Name**: `extract_article`
- **Description**: Extracts an article from a web page. Outputs JSON containing the full content from the provided URL or HTML input.

### Convert Feed

- **Function Name**: `convert_feed`
- **Description**: Converts a partial feed to a full-text feed. Outputs an RSS 2.0 feed (XML or JSON) with the full content extracted from the input URL, which can be a partial feed or a web page.
- **Parameters**:
  - **url**: (String, Optional) URL to a partial feed or a standard HTML page. The 'http://' prefix can be omitted.
  - **format**: (String, Optional) Default is RSS. Use 'json' for JSON output.
  - **max**: (Number, Optional) Maximum number of feed items to process. Default is 5.
  - **summary**: (Number, Optional) Set to 1 to include an excerpt for each item. Default is 1.
  - **use_extracted_title**: (Number, Optional) Use this to replace item titles with those extracted by Full-Text RSS. Default is 1.
  - **links**: (String, Optional) Preserve, remove, or convert links to footnotes.
  - **xss**: (Number, Optional) Enable XSS filtering. Default is 1.
  - **lang**: (Number, Optional) Language detection settings. Default is 2.
  - **accept**: (String, Optional) Specify expected response type (feed or HTML).
  - **content**: (String, Optional) Set output format to 'html', 'text', or specify text wrapping.
  - **parser**: (String, Optional) Choose parsing method: 'gumbo', 'html5-php', or 'libxml'.

## Usage

The Full-Text RSS MCP server is ideal for developers and businesses looking to streamline the process of retrieving and processing full-text articles from various online sources. Whether you need to convert partial feeds to full-text feeds or extract articles from web pages, this server provides efficient and reliable tools to handle these tasks.

Feel free to explore the various tools and parameters to customize the content extraction process according to your specific needs.