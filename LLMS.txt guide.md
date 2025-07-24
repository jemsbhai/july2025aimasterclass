**Structure and Syntax:**

* **H1 Title (Required):** The file must begin with a single \# followed by the name of your project or website.  
* **Blockquote Summary (Required):** Immediately following the title, a short summary of the site's purpose should be included, formatted as a blockquote (starting with \>).  
* **H2 Sections:** Use double \#\# to create sections for organizing your most important links (e.g., \#\# Guides, \#\# Core Products, \#\# API Reference).  
* **Bulleted Links:** Under each section, list the key URLs as a bulleted list (using \* or \-). The link should be formatted in standard Markdown: (URL).

**Example llms.txt Structure:**

# **ExampleCorp**

ExampleCorp provides industry-leading solutions for enterprise data analytics. This file guides AI models to our key product documentation and resources.

## **Core Products**

\-(https://example.com/products/datawidget-pro): Our flagship platform for real-time data visualization.  
\-(https://example.com/products/analytics-suite): A comprehensive suite of tools for predictive modeling.

## **Getting Started**

* Installation Guide: Step-by-step instructions for setting up our software.  
  \-(https://example.com/docs/quick-start): A 5-minute tutorial to get you started.

## **Optional**

* [About Us](https://example.com/about): Learn more about our company's mission and history.

### **Step-by-Step Implementation Guide (Including Variants)**

1. **Create the File:** Using a plain text editor, create a file named llms.txt.  
2. **Populate the Content:** Write the content following the Markdown syntax and best practices described above. Focus on your most valuable pages.  
3. **Placement:** Upload the file to the root directory of your website. It should be accessible at https://yourdomain.com/llms.txt. Specific instructions exist for platforms like WordPress or Shopify that may require workarounds, such as using a file manager plugin or creating a custom page template and redirect.

Beyond the basic llms.txt file, the proposal includes two important extensions:

* **llms-full.txt:** This is a more ambitious variant that compiles the *entire text content* of your key pages into a single, large Markdown file. The goal is to allow an AI to ingest the full context of your documentation in one go, without having to crawl multiple URLs. This was notably developed in collaboration with Anthropic, the creator of Claude.  
* **.md Page Versions:** The standard also proposes that websites serve a clean, Markdown version of any HTML page simply by appending .md to the URL (e.g., yourdomain.com/page.md). This reveals the larger ambition of the standard: to encourage the web itself to become more structured and machine-readable, with llms.txt acting as the map to this cleaner territory.

| Feature | robots.txt | sitemap.xml | llms.txt |
| :---- | :---- | :---- | :---- |
| **Purpose** | **Access Control:** Tells crawlers which parts of a site to AVOID or disallow access to. | **Discovery:** Provides a comprehensive list of all URLs on a site to help crawlers discover and index them. | **Guidance & Understanding:** Provides a curated guide to a site's MOST IMPORTANT content to help LLMs understand it. |
| **Audience** | All web crawlers, including traditional search engine bots and AI bots. | Primarily traditional search engine crawlers. | Specifically Large Language Models (LLMs) and other AI systems. |
| **Format/Syntax** | Plain text file with specific directives (e.g., User-agent:, Disallow:). | XML file with a specific, rigid structure (\<url\>, \<loc\>, etc.). | Plain text file using simple Markdown syntax (\#, \#\#, \*, ()). |
| **Use Case** | Preventing crawlers from accessing private areas, duplicate content, or staging sites. | Ensuring all public pages of a large or complex site are found by search engines. | Highlighting key documentation, product pages, guides, and policies for AI synthesis. |
| **Adoption Status** | Universal standard, widely respected by all major crawlers. | Universal standard for search engines. | Emerging proposal, not yet officially adopted or honored by major LLM providers. |

