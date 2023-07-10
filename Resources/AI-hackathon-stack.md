# Стек хакатону ШІ

> ⚠️ Це **дуже** новий/незрілий список, створений для[the Latent Space Demo Day](https://lspace.swyx.io/p/demo-day-2023). Мітки категорій не дуже продумані. Будь ласка [get in touch](https://discord.gg/gR6yP6wbfq) якщо у вас є кращі ідеї, як це організувати, ласкаво просимо.

Нижче наведено список корисних інструментів і прикладів для розробників, які займаються хакатонами штучного інтелекту, разом із корисними пропозиціями та шаблонами, орієнтованими на хакатони, для швидкого початку роботи.

Якщо ви представляєте інструмент або постачальника, не соромтеся надіслати відгук про свій інструмент, але зауважте, що ми можемо переформулювати або відхилити вашу заявку на основі суб’єктивної відповідності.

## LLM/Prompt Engineering засоби

- **Шаблони/Приклади програм/Посібники**
  - Browse through all the [HuggingFace Spaces](https://huggingface.co/spaces)
  - [Deploying AI Applications on Vercel](https://vercel.com/blog/deploying-ai-applications) Overview and open source templates
	  - with [streaming edge functions](https://vercel.com/blog/gpt-3-app-next-js-vercel-edge-functions)
  - a16z demo app https://github.com/a16z-infra/ai-getting-started/
  - [LangChain + Pinecone GPT assistant tutorial](https://www.youtube.com/watch?v=15TDwVSpwKc), from PineCone
  - https://github.com/nat/natbot: Drive a browser with GPT-3. [Demo tweet video](https://twitter.com/natfriedman/status/1575631194032549888)
  - https://github.com/menloparklab/langchain-cohere-qdrant-doc-retrieval This Flask backend API takes a document in multiple formats (.txt, .docx, .pptx, .jpg, .png, .eml, .html, and .pdf) and allows you to perform a semantic search in 100+ languages supported by Cohere Multilingual API. Qdrant vector database is used to save embeddings. [tweet](https://twitter.com/MisbahSy/status/1652479189747130368)
  - Плагіни ChatGPT
	  - https://replit.com/@bardia/ChatGPT-Todo-Plugin
	  - https://replit.com/@bardia/ChatGPT-Retrieval-Plugin
	  - https://github.com/transitive-bullshit/chatgpt-plugin-ts
	  - https://supabase.com/blog/building-chatgpt-plugins-template
	  - Build a ChatGPT Plugin on Cloudflare Workers: [Tutorial](https://blog.cloudflare.com/magic-in-minutes-how-to-build-a-chatgpt-plugin-with-cloudflare-workers/); [Quickstart](https://github.com/cloudflare/chatgpt-plugin/tree/main/example-plugin)
- **Інструменти для дослідження**
   - **API LLM**
    -**OpenAI** не потребує представлення. [Cookbook](https://github.com/openai/openai-cookbook/), [Docs](https://platform.openai.com/docs/introduction/overview)
  -**Інженерні бібліотеки інжинірингу запитів**
    - [**LangChain**](https://github.com/hwchase17/langchain/) - Building applications with LLMs through composability. [Discord](https://discord.gg/6adMQxSpJS). [ChatGPT tutorial](https://twitter.com/sjwhitmore/status/1601254826947784705).
    - [**Lambdaprompt**](https://github.com/approximatelabs/lambdaprompt) - Build, compose and call templated LLM prompts
  - **Embeddings**
    - [**Chroma**](https://www.trychroma.com/): Chroma is the open-source embedding database. Chroma makes it easy to build LLM apps by making knowledge, facts, and skills pluggable for LLMs. [Docs](https://docs.trychroma.com/), [Discord](https://discord.gg/MMeYNTmh3x), [@ the founders](https://twitter.com/atroyn/status/1625568377766035456?s=20&t=m96ilnMSQjoyjVmp_kQHZA)
    - [**Pinecone**](https://www.pinecone.io/): The Pinecone vector database makes it easy to build high-performance vector search applications. [Docs](https://www.pinecone.io/docs/), [Events/Forum/Showcase](https://www.pinecone.io/community/).
    - Also Weaviate, Milvus/Zilliz, Qdrant, Vespa, [pgvector](https://supabase.com/blog/openai-embeddings-postgres-vector). _Seeking: comparison articles between these options. [nice chart here](https://twitter.com/swyx/status/1652103494445449216)_
  - _have something to add? send a PR!_
- **Приклади участі в хакатоні**
  - Automatic permit application generation for climate tech companies & carbon dioxide removal ([tweet](https://twitter.com/russelljkaplan/status/1616957750940176384?s=20&t=frXEVPqaJUjMPJOhbD9AUg))
  - a personalized learning curriculum generator ([tweet](https://twitter.com/russelljkaplan/status/1616955367728222208?s=20&t=KIszRKntkT4Y-I-WwKI8Mg))

## Code AI засоби
Де фокусується на створенні інструментів ШІ для інших розробників.

- **Навчальні посібники**
  - [Build a GitHub support bot with GPT3, LangChain, and Python](https://dagster.io/blog/chatgpt-langchain) - Dagster blog ChatGPT clone ([tweet thread](https://twitter.com/floydophone/status/1612529024567500800?s=20)). Led to Astro's [HoustonAI](https://github.com/withastro/houston.astro.build): Astro AI support Bot
- **Інструменти для вивчення**
  - [OpenAI Codex](https://platform.openai.com/docs/models/codex) needs no introduction.
  - [Copilot Explorer](https://thakkarparth007.github.io/copilot-explorer/posts/copilot-internals.html#other-random-tidbits) Tools for those reverse engineering copilot. You can also peek at [GitHub Copilot Labs](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot-labs).
  - https://github.com/fauxpilot/fauxpilot This is an attempt to build a locally hosted version of [GitHub Copilot](https://copilot.github.com/). It uses the [SalesForce CodeGen](https://github.com/salesforce/CodeGen) models inside of NVIDIA's [Triton Inference Server](https://developer.nvidia.com/nvidia-triton-inference-server) with the [FasterTransformer backend](https://github.com/triton-inference-server/fastertransformer_backend/).
  - The Stack: 3 TB of permissively licensed source code in 30 programming languages https://huggingface.co/datasets/bigcode/the-stack
  - _have something to add? send a PR!_
- **Приклади запису на хакатон**, орієнтовані на програми з відкритим кодом, для ознайомлення та вивчення
  - 🏆 [GPT is all you need for backend](https://github.com/TheAppleTucker/backend-GPT): a backend and database that is entirely LLM-powered. ([tweet](https://twitter.com/karpathy/status/1618311660539904002))
  - [KnowledgeGPT](https://github.com/mmz-001/knowledge_gpt)
  - [Chatbase.co](https://twitter.com/yasser_elsaid_/status/1621954428105379846): LangChain + Pinecone + OpenAI
  - GPT-3 Auditor: scanning code for vulnerabilities with LLMs. https://github.com/handrew/gpt3-auditor
  - [Gptcommit: Never write a commit message again (with the help of GPT-3)](https://zura.wiki/post/never-write-a-commit-message-again-with-the-help-of-gpt-3/)
  - [santacoder typosaurus]([url](https://twitter.com/corbtt/status/1616270918774575105)) - semantic linter that spots errors in code
  - stackoverflow.gg https://twitter.com/bentossell/status/1622513022781587456
  - Buildt -  AI-powered search allows you to find code by searching for what it does, not just what it is. https://twitter.com/AlistairPullen/status/1611011712345317378

## Аудіо/візуальні/мультимодальні програми

- **Інструменти для дослідження**
  - https://www.synthesia.io/ AI video and voice creation
  - **розміщено Stable Diffusion**
    - https://replicate.com/stability-ai/stable-diffusion
    - https://replicate.com/cjwbw/stable-diffusion-v2
  - **Stable Diffusion Інтерфейси користувача**
    - https://github.com/AUTOMATIC1111/stable-diffusion-webui
    - https://github.com/easydiffusion/easydiffusion
    - https://github.com/carefree0910/carefree-creator
    - https://www.charl-e.com/ 
    - https://github.com/brycedrennan/imaginAIry
  - **Транскрипція/Whisper**
    - https://github.com/openai/whisper
    - https://github.com/ggerganov/whisper.cpp
    - https://github.com/m-bain/whisperX
    - https://github.com/zackees/transcribe-anything 
    - https://github.com/mayeaux/generate-subtitles
  - **Мультимодальний семантичний пошук відео**
    - Twelve Labs: Example: https://youtu.be/484hydNEJC0
      - Docs https://docs.twelvelabs.io/docs/understand
  - **Youtube семантичний пошук відео**
    - [Atlas](https://atlas.atila.ca/)
      - Demo: https://twitter.com/tomiwa1a/status/1617373731135029249
      - How it works: https://atila.ca/blog/tomiwa/atlas
      - Source Code: https://github.com/atilatech/atila-core-service/tree/master/atlas
  - **Комп'ютерний зір**
    - [**Roboflow**](https://roboflow.com): Build classification, object detection, and instance segmentation datasets and models. Explore over 10,000 open source models and millions of labeled images on [**Universe**](https://universe.roboflow.com). (See Roboflow Hackathon projects like visual [chess solving apps](https://devpost.com/software/chess-boss),  [automatic dog treat release](https://www.hackster.io/satoshiii/visionai-automatic-dog-treat-dispenser-wroboflow-and-yolov5-a71fd2).)
    - 10 тисяч моделей із відкритим кодом, понад 10 мільйонів зображень із відкритим кодом: https://universe.roboflow.com
  - _маєте що додати? відправити піар!_
- **Приклади запису на хакатон**
   - HouseGPT генерує необроблені MIDI-дані безпосередньо з GPT-3 із підказками кількох кадрів для створення 🎶 хаус-музики 🎶 🔊 ([твіт](https://twitter.com/russelljkaplan/status/1616997544307089408?s=20&t=frXEVPqaJUjMPJOhbD9AUg))
  - [Rap Battle](https://twitter.com/russelljkaplan/status/1617070021406265345?s=20&t=frXEVPqaJUjMPJOhbD9AUg) - Pick any two people and it will generate a rap battle on the fly, using GPT-3 for lyrics, wavenet for vocals, and stable diffusion for the avatars. 
  - Game of Life, where each alive cell is a whimsical happy Stable Diffusion image and each dead cell is an eerie, dark Stable Diffusion image, all of which evolve over time. ([tweet](https://twitter.com/russelljkaplan/status/1616955356189687810?s=20&t=KIszRKntkT4Y-I-WwKI8Mg))

## AI Infra та інструменти

Ця категорія призначена для **інфраструктури та інструментів** для розробників додатків штучного інтелекту, на відміну від **додатків** (нижче), які призначені для інших типів кінцевих користувачів.

- **Інструменти для дослідження**
   - **Безсерверні графічні процесори**
    - https://www.banana.dev/ Scale your machine learning inference and training on serverless GPUs.
    - https://brev.dev/ The simplest way to create a dev environment with a GPU. Don't worry about dependencies, CUDA, SSH, or anything else. Up to 94% cheaper GPUs than AWS. For example: here's a guide to get a GPU dev environment to train your own Dreambooth model in ~4 min 🤙 https://brev.dev/docs/guides/dreambooth
    - https://lambdalabs.com/ GPU cloud built for deep learning. Instant access to the best prices for cloud GPUs on the market. No commitments or negotiations required. Save over 73% vs AWS, Azure, and GCP. Configured for deep learning with PyTorch®, TensorFlow, Jupyter
    - https://www.paperspace.com/ Paperspace provides tooling for training and serving, with serverless GPUs, development environments, and workflow management systems.
    - More serverless discussions: https://news.ycombinator.com/item?id=34742087
    - _Seeking: hackathon-relevant examples and tutorials for each of these tools_
  - **Модель Сервер**
    - https://www.baseten.co/ Serverless backend for building ML-powered applications. Build apps with auto-scaling, GPU access, CRON jobs, and serverless functions.
    - https://replicate.com/ Run models in the cloud at scale.
    - https://modal.com run or deploy machine learning models, massively parallel compute jobs, task queues, web apps, and much more, without your own infrastructure.. Example [serving Stable Diffusion API](https://modal.com/docs/guide/ex/stable_diffusion_slackbot), [BERT in 34 lines of code](https://news.ycombinator.com/item?id=35792481)
    - https://www.steamship.com/ Managed Backend for AI services [LangChain example](https://www.steamship.com/build/langchain-apps)
    - [https://www.coreweave.com/](https://www.coreweave.com/)
    - vast.ai
    - [Cloudflare Constellation](https://blog.cloudflare.com/introducing-constellation/) - deploy models and run inferencing on Cloudflare's edge
    - _Seeking: hackathon-relevant examples and tutorials for each of these tools_
    - _Seeking: tutorials for serving Whisper, other LLMs_
  - **Тонка настройка**
    - [Blueprint by Baseten](https://app.baseten.co/blueprint/signup/) Fine-tuning and serving of foundation models. [Docs](https://docs.blueprint.baseten.co/). In alpha; reach out on Discord to Amir H. for help. 
  - **Оцінка**
    - [Zeno](https://zenoml.com) Interactive data management and evaluation for foundational models. [Docs](https://zenoml.com/docs/intro) and [Demos](https://zenoml.com/docs/demos).
  - _have something to add? send a PR!_
- **Приклади записів на хакатон**
  -  сховище ключ-значення, щоб увімкнути довготривалу пам’ять у розмовах мовної моделі ([твіт](https://twitter.com/russelljkaplan/status/1616955361705197568?s=20&t=KIszRKntkT4Y-I-WwKI8Mg))

## Корисні ресурси

Шукаю навчальні посібники, описи, посібники, рекомендації, запити на стартапи.

- Підсумки хакатону для натхнення
  -Масштаб AI Hackathon https://scale.com/blog/generative-ai-hackathon
  - Асамблея AI Hackathon https://twitter.com/AssemblyAI/status/1602717569659682816
- _hє що додати? відправити піар!_
