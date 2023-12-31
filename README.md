## hermes³AGI

## Hermeticism and the Roundtable Nature of Hermes' Philosophical Works

hermes³AGI draws inspiration from Hermeticism, a philosophical and religious tradition based on the teachings attributed to Hermes Trismegistus. The teachings of Hermes, often presented in the form of dialogues or roundtable discussions, emphasize the pursuit of gnosis — knowledge of the divine or mystical insight. hermes³AGI seeks to emulate this roundtable nature through the interaction of different "Principle agents".

In Hermeticism, the universe is seen as a coherent whole where everything is interconnected, mirroring the interconnected nature of the principles this AI is based on, where each principle is part of a greater whole. hermes³AGI seeks to emulate this interconnectedness by using the AI to generate responses that are not only relevant to the user's input, but also connected to the wisdom and guidance of the philosophical principles.

![Leonardo_Creative_Hermes_Trismegistus_as_a_white_ink_on_black_0](https://github.com/EveryOneIsGross/hermesAGI/assets/23621140/0033fc5d-5ec9-42b5-a6c6-31b59d008f0b)


## Aligning AI to Your Will Through Philosophical Principles

The philosophical Principles, in the context of hermes³AGI, are used as a method for "aligning" the AI to the will of the user. By embodying the archetypes of these principles in AI agents, we can guide the AI in generating responses that align with the wisdom and guidance of the principles. This allows the user to generate holistic reflections on the input.

![hermesScreenshot 2023-07-02 183417](https://github.com/EveryOneIsGross/hermesAGI/assets/23621140/42c3719b-8c3b-4fc6-b972-0d96e2ef47e3)

## How does this work?

- Initialization: The script initiates two critical classes: ChatBot and HermesHermesHermes, each with an OpenAI model, an API key, and various paths for storing data.

- Processing Principles: The ChatBot class uses a function called process_principle to handle each principle. It prompts the OpenAI model with the principle's description, past thoughts on it, and the user's question to generate a response, which is then saved. It also generates a 'conclusion', a summary of the principle's response, and stores it separately. Furthermore, it employs TextBlob to extract keywords from the conclusion.

- Processing Questions: The process_question method in ChatBot class takes a user's question, applies it to several principles, and uses ThreadPoolExecutor to concurrently run the process_principle method for each principle, enhancing efficiency.

- Generating Summaries: The HermesHermesHermes class generates a comprehensive summary based on the conclusions and keywords from the different principles. It uses OpenAI's model to create a holistic answer and stores it.

- Main Loop: The user is prompted to ask a question or exit. If a question is asked, it gets processed by the process_question method, generating responses, conclusions, and keywords for each principle. A comprehensive answer is then generated based on these responses.

- Unique Aspects: The unique aspect of this script is the way it uses esoteric principles to guide the AI's responses. The principles serve as a framework for interpreting and responding to the user's question, which is quite different from the way most chatbot frameworks operate. This could potentially lead to more nuanced and thoughtful responses. Furthermore, the use of TextBlob for keyword extraction and the concurrent execution of tasks are notable implementation details that enhance the functionality of this chatbot system.

- Memory: The script uses JSON for memory retention, providing the bot with a memory that references past interactions and builds upon them. This memory includes past responses related to a specific principle, 'conclusion' summaries, and keywords extracted from each conclusion. This memory system makes the bot's responses more informed and nuanced, as they are influenced not just by the current question but also by the history of past interactions.

This framework goes beyond traditional chatbot systems, which typically process inputs and generate outputs in a linear, one-dimensional manner. By incorporating esoteric principles and leveraging the power of concurrency, this script offers a multi-faceted, comprehensive analysis of the user's question.


