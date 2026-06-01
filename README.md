I got into AI and running LLMs and all that after Pewdiepie released the video about training his own model. At first I was trying out models like Qwen3.5 and Deepseek-R1, but quickly felt kinda disappointed with the UI that came with ollama. After a bit of looking around I discovered that no one even used ollama's UI and there were better options like open-webUI and anythingLLM. I tried giving open-webUI a shot but couldn't really wrap my head around all the options and settings. And realized that outputs were slowers while using it because by default open-webui has things like title generation and next query generation. I didn't feel like onfiguring all of those settings across 3 different pages so I gave up, especially since I wasn't even going to use most of the features that come with an advanced package like that. Then I created this.

The goal was to make an UI that's basic, lightweight, and easy eanough to use for someone who is just getting into running LLMs on their own machine using ollama.

BeigeUI is a barebones html interface that doesn't have persistent chat history, memory, search integration, RAG or anything at all. Just a messagebox, status sidebar and a field for system prompt if needed. This project was partially (and by partially I mean mostly) vibecoded with Claude over the span of 5 days.

Less than 24 hours after I was done with the final edits, Pewdiepie dropped another video, announcing Odysseus. If I knew he would release an Interface like this I wouldn't have really bothered going through all the hassle but now that it's done I'm uploading it anyway.

<img width="800" height="615" alt="gif" src="https://github.com/user-attachments/assets/d595e2bd-0534-42f9-92d2-bd755b6c2149" />
<br>
<br>
<img width="544" height="418" alt="brave_8LjwRF1JEy" src="https://github.com/user-attachments/assets/374390d7-9153-47c4-bd03-a10b1751bf61" />

Features:
- Automatically injects 'keep_alive = -1' on startup so your model doesn't offload after 5 minutes.
- Image input field for models that support it.
- Sidebar for info such as session token count and memory usage.
