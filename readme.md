# 🌐 Web Wanderer 🕸️

Dive into the digital depths with Web Wanderer, your guide through the intricate web of online content. Our architecture is designed to navigate, understand, and interact with websites, harnessing the power of embeddings and Large Language Models (LLMs) to fulfill your digital quests.

## 🏗️ Overall Architecture

- Crawl & Capture: \
  Our system starts its journey by crawling through websites, capturing the essence of page content with precision.

- Text Transformation \
  We then transform the text, splitting it into segments of appropriate length to ensure digestibility for our next steps.

- Contextual Embeddings \
  Depending on your needs, we can feed the text through embeddings to extract the most relevant contexts, ensuring a tailored experience.

- LLM Integration \
   With the power of LLMs, we interpret the context, deciding on the next best action to take in the vast digital landscape. \

- 🧠 LLM Architecture \
  At the heart of Web Wanderer lies our LLM, a decision-making titan ready to interact with the web based on the given query and context. Here's how it navigates the digital terrain:

## Actions: LLM should be able to:

- 🖱️ Click
- ⌨️ Type
- 📜 Scroll
- ⏳ Wait (for loading)
- 🛑 Stop (when the task is completed)

  (certain actions like hover, select, resize for now)

## Output: Each iteration:

`action`: The next step to take.

`trigger`: Identifies which element to interact with, using a unique CSS selector. We might assign custom selectors for seamless interaction via tools like Selenium.

`is_end`: A flag to check if the task has reached its conclusion.

## Completion:

The journey concludes once is_end turns true, signaling the end of our digital expedition.
