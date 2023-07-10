# Нотатки AI

нотатки про сучасний рівень штучного інтелекту з акцентом на генеративних і великих моделях мови. Це «сировина» для інформаційного бюлетеня https://lspace.swyx.io/.

> Це репо раніше називалося https://github.com/sw-yx/prompt-eng, але був перейменований тому що [Prompt Engineering is Overhyped](https://twitter.com/swyx/status/1596184757682941953). Це зараз [AI Engineering](https://www.latent.space/p/ai-engineer) нотатки repo.

Цей файл Readme є лише оглядом високого рівня простору; ви маєте побачити найбільше оновлень в ІНШИХ файлах розмітки в цьому репо:

- `TEXT.md` - генерація тексту, переважно за допомогою GPT-4
	- `TEXT_CHAT.md` - інформація про ChatGPT і конкурентів, а також про похідні продукти
	- `TEXT_SEARCH.md` - інформація про семантичний пошук із увімкненим GPT-4 та інша інформація
	- `TEXT_PROMPTS.md` - невеликий[swipe file](https://www.swyx.io/swipe-files-strategy) хороших підказок GPT3
- `INFRA.md` - необроблені примітки щодо інфраструктури штучного інтелекту, обладнання та масштабування
- `AUDIO.md` - відстеження транскрипції аудіо/музики/голосу + генерація
- `CODE.md` - моделі codegen, такі як Copilot
- `IMAGE_GEN.md` - найдосконаліший файл, з найбільшим наголосом на Stable Diffusion, а також на midjourney і dalle.
	- `IMAGE_PROMPTS.md` - a small [swipe file](https://www.swyx.io/swipe-files-strategy) гарних підказок зображення
- **Ресурси**: постійні очищені ресурси, на які призначено постійне посилання
- **заглушки** - дуже маленькі/легкі прото-сторінки майбутніх зон покриття
		  - `AGENTS.md` - відстеження "агентного ШІ"
-**ідеї для блогів** – потенційні ідеї для публікацій у блогах, отримані з цих нотаток

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
<details>
<summary>Зміст</summary>

- [Motivational Use Cases](#motivational-use-cases)
- [Top AI Reads](#top-ai-reads)
- [Communities](#communities)
- [People](#people)
- [Misc](#misc)
- [Quotes, Reality & Demotivation](#quotes-reality--demotivation)
- [Legal, Ethics, and Privacy](#legal-ethics-and-privacy)

</details>
<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Мотиваційні випадки використання

- зображення
  - https://mpost.io/best-100-stable-diffusion-prompts-the-most-beautiful-ai-text-to-image-prompts/it
  - [3D MRI synthetic brain images](https://twitter.com/Warvito/status/1570691960792580096?) - [позитивний прийом від статистиків нейровізуалізації](https://twitter.com/danCMDstat/status/1572312699853312000?s=20&t=x-ouUbWA5n0-PxTGZcy2iA)
  - [multiplayer stable diffusion](https://huggingface.co/spaces/huggingface-projects/stable-diffusion-multiplayer?roomid=room-0)
- відео
  - mg2img сцен із відомих фільмів ([lalaland](https://twitter.com/TomLikesRobots/status/1565678995986911236))
    - [img2img transforming actor](https://twitter.com/LighthiserScott/status/1567355079228887041?s=20&t=cBH4EGPC4r0Earm-mDbOKA) with ebsynth + koe_recast
    -як працює ebsynth https://twitter.com/TomLikesRobots/status/1612047103806545923?s=20
  - віртуальна мода ([karenxcheng](https://twitter.com/karenxcheng/status/1564626773001719813))
  - [зображення безшовної плитки](https://twitter.com/replicatehq/status/1568288903177859072?s=20&t=sRd3HRehPMcj1QfcOwDMKg)
  - еволюція сцен ([xander](https://twitter.com/xsteenbrugge/status/1558508866463219712))
  - замальовування https://twitter.com/orbamsterdam/status/1568200010747068417?s=21&t=rliacnWOIjJMiS37s8qCCw
  - webUI img2img співпраця https://twitter.com/_akhaliq/status/1563582621757898752
  - зображення у відео з поворотом https://twitter.com/TomLikesRobots/status/1571096804539912192
  - "prompt paint" https://twitter.com/1littlecoder/status/1572573152974372864
  - аудіо-відео анімація вашого обличчя https://twitter.com/siavashg/status/1597588865665363969
  - фізичні іграшки до 3d моделі + анімація https://twitter.com/sergeyglkn/status/1587430510988611584
  - музичні відео
    - [video killed the radio star](https://www.youtube.com/watch?v=WJaxFbdjm8c), [colab](https://colab.research.google.com/github/dmarx/video-killed-the-radio-star/blob/main/Video_Killed_The_Radio_Star_Defusion.ipynb) Це використовує OpenAI Whisper для перетворення мовлення в текст, що дозволяє знімати відео YouTube і створювати анімацію Stable Diffusion на основі тексту пісні у відео YouTube
    - [Stable Diffusion Videos](https://colab.research.google.com/github/nateraw/stable-diffusion-videos/blob/main/stable_diffusion_videos.ipynb) генерує відео шляхом інтерполяції між підказками та аудіо
  - проект direct text2video
    - https://twitter.com/_akhaliq/status/1575546841533497344
    - https://makeavideo.studio/ - explorer https://webvid.datasette.io/webvid/videos
    - https://phenaki.video/
    - https://github.com/THUDM/CogVideo
    - https://imagen.research.google/video/
- text-to-3d https://twitter.com/_akhaliq/status/1575541930905243652
  -  https://dreamfusion3d.github.io/
  -  open source impl: https://github.com/ashawkey/stable-dreamfusion
    - demo https://twitter.com/_akhaliq/status/1578035919403503616
-  текстові продукти
	- має список випадків використання в кінці https://huyenchip.com/2023/04/11/llm-engineering.html
  - Jasper
  - GPT for Obsidian https://reasonabledeviations.com/2023/02/05/gpt-for-second-brain/
  - gpt3 email https://github.com/sw-yx/gpt3-email
  - gpt3() in google sheet [2020](https://twitter.com/pavtalk/status/1285410751092416513?s=20&t=ppZhNO_OuQmXkjHQ7dl4wg), [2022](https://twitter.com/shubroski/status/1587136794797244417) - [sheet](https://docs.google.com/spreadsheets/d/1YzeQLG_JVqHKz5z4QE9wUsYbLoVZZxbGDnj7wCf_0QQ/edit) google sheets https://twitter.com/mehran__jalali/status/1608159307513618433
	  - https://gpt3demo.com/apps/google-sheets
	  - Charm https://twitter.com/shubroski/status/1620139262925754368?s=20
  - https://www.summari.com/ Summari helps busy people read more
- market maps/landscapes
	- sequoia market map https://twitter.com/sonyatweetybird/status/1584580362339962880
	- base10 market map https://twitter.com/letsenhance_io/status/1594826383305449491
	- matt shumer market map https://twitter.com/mattshumer_/status/1620465468229451776 https://docs.google.com/document/d/1sewTBzRF087F6hFXiyeOIsGC1N4N3O7rYzijVexCgoQ/edit
	- nfx https://www.nfx.com/post/generative-ai-tech-5-layers?ref=context-by-cohere
	- a16z https://a16z.com/2023/01/19/who-owns-the-generative-ai-platform/
		- https://a16z.com/2023/06/20/emerging-architectures-for-llm-applications/
	- madrona https://www.madrona.com/foundation-models/
- ігрові активи - 
	- emad thread https://twitter.com/EMostaque/status/1591436813750906882
	- scenario.gg https://twitter.com/emmanuel_2m/status/1593356241283125251
	- [3d game character modeling example](https://www.traffickinggame.com/ai-assisted-graphics/)
	- MarioGPT https://arxiv.org/pdf/2302.05981.pdf https://www.slashgear.com/1199870/mariogpt-uses-ai-to-generate-endless-super-mario-levels-for-free/ https://github.com/shyamsn97/mario-gpt/blob/main/mario_gpt/level.py
	- https://news.ycombinator.com/item?id=36295227

## Найкраще читання AI

Більш просунуті зчитування GPT3 були розділені на https://github.com/sw-yx/ai-notes/blob/main/TEXT.md

- https://www.gwern.net/GPT-3#prompts-as-programming
- https://learnprompting.org/

### Початківець читає

  - [Білл Гейтс про ШІ]([https://www.gatesnotes.com/The-Age-of-AI-Has-Begun](https://www.gatesnotes.com/The-Age-of-AI-Has-Begun) ([tweet](https://twitter.com/gdb/status/1638310597325365251?s=20))
	  - "Розробка ШІ є такою ж фундаментальною, як створення мікропроцесора, персонального комп’ютера, Інтернету та мобільного телефону. Це змінить те, як люди працюють, навчаються, подорожують, отримують медичне обслуговування та спілкуються один з одним."
  - [Стів Єгге про ШІ для розробників](https://about.sourcegraph.com/blog/cheating-is-all-you-need)
  - чудовий вступ до моделей основи from MSR https://youtu.be/HQI6O5DlyFc
  - підручник підказки openAIhttps://beta.openai.com/docs/quickstart/add-some-examples
  - google LAMDA intro https://aitestkitchen.withgoogle.com/how-lamda-works
  - DALLE2 книга швидкого написання http://dallery.gallery/wp-content/uploads/2022/07/The-DALL%C2%B7E-2-prompt-book-v1.02.pdf
  - https://medium.com/nerd-for-tech/prompt-engineering-the-career-of-future-2fb93f90f117
  - https://ourworldindata.org/brief-history-of-ai ai progress overview with nice charts
  - Jon Stokes' [AI Content Generation, Part 1: Machine Learning Basics](https://www.jonstokes.com/p/ai-content-generation-part-1-machine)
  - [What are transformer models and how do they work?](https://txt.cohere.ai/what-are-transformer-models/) - maybe [a bit too high level](https://news.ycombinator.com/item?id=35577138)
  - генерація тексту
	  - humanloop's [prompt engineering 101](https://website-olo3k29b2-humanloopml.vercel.app/blog/prompt-engineering-101)
	  - Пояснення Стівена Вольфрама https://writings.stephenwolfram.com/2023/02/what-is-chatgpt-doing-and-why-does-it-work/
	  - еквівалент від jon stokes jonstokes.com/p/the-chat-stack-gpt-4-and-the-near
	  - https://andymatuschak.org/prompts/
	  - LLM університету Cohere https://docs.cohere.com/docs/llmu 
	  - https://www.jonstokes.com/p/chatgpt-explained-a-guide-for-normies for normies
  - генерація зображення
	  - https://wiki.installgentoo.com/wiki/Stable_Diffusion overview
	  - https://www.reddit.com/r/StableDiffusion/comments/x41n87/how_to_get_images_that_dont_suck_a/
	  - https://mpost.io/best-100-stable-diffusion-prompts-the-most-beautiful-ai-text-to-image-prompts/
	  - https://www.kdnuggets.com/2021/03/beginners-guide-clip-model.html 
  - для нетехнічних
    - https://www.jonstokes.com/p/ai-content-generation-part-1-machine
    - https://www.protocol.com/generative-ai-startup-landscape-map
    - https://twitter.com/saranormous/status/1572791179636518913

### Проміжне читання

  - **Звіт про стан ШІ**: [2018](https://www.stateof.ai/2018), [2019](https://www.stateof.ai/2019), [2020](https://www.stateof.ai/2020), [2021](https://www.stateof.ai/2021), [2022](https://www.stateof.ai/)
  - reverse chronological major events https://bleedingedge.ai/
  - A16z AI Canon https://a16z.com/2023/05/25/ai-canon/
	  -  **[Software 2.0](https://karpathy.medium.com/software-2-0-a64152b37c35)**: Андрій Карпаті був одним із перших, хто чітко пояснив (у 2017 році!), чому нова хвиля ШІ дійсно важлива. Його аргумент полягає в тому, що штучний інтелект є новим і потужним способом програмування комп’ютерів. Оскільки магістерські програми стрімко вдосконалювалися, ця теза виявилася пророчою та дає хорошу розумову модель того, як може розвиватися ринок ШІ.
	-   **[Стан GPT](https://build.microsoft.com/en-US/sessions/db3f4859-cd30-4445-a0cd-553c3304f8e2)**: Також від Карпат, це дуже доступне пояснення того, як загалом працюють моделі ChatGPT / GPT, як ними користуватися та в яких напрямках можуть розвиватися дослідження та розробки.
	-   [**Wщо робить ChatGPT ... і чому він працює?**](https://writings.stephenwolfram.com/2023/02/what-is-chatgpt-doing-and-why-does-it-work/): Інформатик і підприємець Стівен Вольфрам дає довге, але зрозуміле пояснення, починаючи з перших принципів, того, як працюють сучасні моделі ШІ. Він стежить за хронологією від ранніх нейронних мереж до сучасних LLM і ChatGPT.
	-   **[Transformers, explained](https://daleonai.com/transformers-explained)**: Ця публікація Дейла Марковіца є коротшою та більш прямою відповіддю на запитання «що таке LLM і як це працює?» Це чудовий спосіб засвоїти тему та розвинути інтуїцію щодо технології. Це було написано про GPT-3, але все ще стосується нових моделей.
	-   **[Як Stable Diffusion працює](https://mccormickml.com/2022/12/21/how-stable-diffusion-works/)**: Це комп'ютерний зір, аналог останнього посту. Кріс МакКормік пояснює неспеціалісту, як працює Stable Diffusion, і загалом розвиває інтуїцію щодо моделей перетворення тексту в зображення. Щоб отримати ще _ніжніший_ вступ, перегляньте цей [комікс](https://www.reddit.com/r/StableDiffusion/comments/zs5dk5/i_made_an_infographic_to_explain_how_stable/) from r/StableDiffusion.
	- Explainers
		-   [**Глибоке навчання в двох словах: основні поняття**](https://developer.nvidia.com/blog/deep-learning-nutshell-core-concepts/): Ця серія з чотирьох частин від Nvidia розповідає про основи глибокого навчання, яке практикувалося в 2015 році, і є хорошим ресурсом для тих, хто тільки вивчає ШІ.
		-   **[Практичне глибоке навчання для кодерів](https://course.fast.ai/)**: Комплексний безкоштовний курс з основ штучного інтелекту, пояснений на практичних прикладах і коді.
		-   **[Word2vec пояснив](https://towardsdatascience.com/word2vec-explained-49c52b4ccb71)**: Легкий вступ до вбудовування та токенів, які є будівельними блоками LLM (і всіх мовних моделей).
		-   **[Так, ви повинні розуміти опору](https://karpathy.medium.com/yes-you-should-understand-backprop-e2f06eab496b)**: Більш глибокий допис про зворотне поширення, якщо ви хочете зрозуміти деталі. Якщо ви хочете ще більше, спробуйте [Stanford CS231n lecture](https://www.youtube.com/watch?v=i94OvYb6noo) on Youtube.
	- Курси
		-   **[Stanford CS229](https://www.youtube.com/playlist?list=PLoROMvodv4rMiGQp3WXShtMGgzqpfVfbU)**: Вступ до машинного навчання з Ендрю Нґом, який охоплює основи машинного навчання.
		-   **[Stanford CS224N](https://www.youtube.com/playlist?list=PLoROMvodv4rOSH4v6133s9LFPRHjEmbmJ)**: NLP з глибоким навчанням з Крісом Меннінгом, що охоплює основи НЛП через перше покоління LLM.
  - https://cims.nyu.edu/~sbowman/eightthings.pdf
	  1. LLMs predictably get more capable with increasing investment, even without targeted innovation. 
	  2. Many important LLM behaviors emerge unpredictably as a byproduct of increasing investment. 
	  3. LLMs often appear to learn and use representations of the outside world. 
	  4. There are no reliable techniques for steering the behavior of LLMs. 
	  5. Experts are not yet able to interpret the inner workings of LLMs. 
	  6. Human performance on a task isn’t an upper bound on LLM performance. 
	  7. LLMs need not express the values of their creators nor the values encoded in web text. 
	  8. Brief interactions with LLMs are often misleading.
	  9. simonw highlights https://fedi.simonwillison.net/@simon/110144185463887790
  - openai prompt eng cookbook https://github.com/openai/openai-cookbook/blob/main/techniques_to_improve_reliability.md
  - on prompt eng overview https://lilianweng.github.io/posts/2023-03-15-prompt-engineering/
  - Recap of 2022's major AI developments https://www.deeplearning.ai/the-batch/issue-176/
  - DALLE2 asset generation + inpainting https://twitter.com/aifunhouse/status/1576202480936886273?s=20&t=5EXa1uYDPVa2SjZM-SxhCQ
  - suhail journey https://twitter.com/Suhail/status/1541276314485018625?s=20&t=X2MVKQKhDR28iz3VZEEO8w
  - composable diffusion - "AND" instead of "and" https://twitter.com/TomLikesRobots/status/1580293860902985728
  - on BPE tokenization https://towardsdatascience.com/byte-pair-encoding-subword-based-tokenization-algorithm-77828a70bee0 see also google sentencepiece and openai tiktoken
	  - source in GPT2 source https://github.com/openai/gpt-2/blob/master/src/encoder.py
	  - note that BPEs are suboptimal https://www.lesswrong.com/posts/dFbfCLZA4pejckeKc/a-mechanistic-explanation-for-solidgoldmagikarp-like-tokens?commentId=9jNdKscwEWBB4GTCQ
		  - causes math and string character issues https://news.ycombinator.com/item?id=35363769
	  - https://platform.openai.com/tokenizer and https://github.com/openai/tiktoken (more up to date: https://tiktokenizer.vercel.app/)
	  - https://observablehq.com/@simonw/gpt-3-token-encoder-decoder
	  - karpathy wants tokenization to go away https://twitter.com/karpathy/status/1657949234535211009
	  - positional encoding not needed for decoder only https://twitter.com/a_kazemnejad/status/1664277559968927744?s=20
  - creates its own language https://twitter.com/giannis_daras/status/1531693104821985280
  - Google Cloud Generative AI Learning Path https://www.cloudskillsboost.google/paths/118
  - img2img https://andys.page/posts/how-to-draw/
  - on language modeling https://lena-voita.github.io/nlp_course/language_modeling.html and approachable but technical explanation of language generation including sampling from distributions and some mechanistic intepretability (finding neuron that tracks quote state)
  - quest for photorealism https://www.reddit.com/r/StableDiffusion/comments/x9zmjd/quest_for_ultimate_photorealism_part_2_colors/
    - https://medium.com/merzazine/prompt-design-for-dall-e-photorealism-emulating-reality-6f478df6f186
  - settings tweaking https://www.reddit.com/r/StableDiffusion/comments/x3k79h/the_feeling_of_discovery_sd_is_like_a_great_proc/
    - seed selection https://www.reddit.com/r/StableDiffusion/comments/x8szj9/tutorial_seed_selection_and_the_impact_on_your/
    - minor parameter parameter difference study (steps, clamp_max, ETA, cutn_batches, etc) https://twitter.com/KyrickYoung/status/1500196286930292742
    - Generative AI: Autocomplete for everything https://noahpinion.substack.com/p/generative-ai-autocomplete-for-everything?sd=pf
    - [How does GPT Obtain its Ability? Tracing Emergent Abilities of Language Models to their Sources](https://yaofu.notion.site/How-does-GPT-Obtain-its-Ability-Tracing-Emergent-Abilities-of-Language-Models-to-their-Sources-b9a57ac0fcf74f30a1ab9e3e36fa1dc1)  хороша стаття з історією розвитку сімейства моделей GPT і як розвивалися можливості
- https://barryz-architecture-of-agentic-llm.notion.site/Almost-Everything-I-know-about-LLMs-d117ca25d4624199be07e9b0ab356a77

### Advanced Reads

- https://github.com/Mooler0410/LLMsPracticalGuide
	- хороший підібраний список усіх документів imp
- Трансформери з нуля https://e2eml.school/transformers.html
	- transformers vs LSTM https://medium.com/analytics-vidhya/why-are-lstms-struggling-to-matchup-with-transformers-a1cc5b2557e3
	- покрокове керівництво по коду трансформатора https://twitter.com/mark_riedl/status/1555188022534176768
	- сімейство трансформерів https://lilianweng.github.io/posts/2023-01-27-the-transformer-family-v2/
		- carmack paper list https://news.ycombinator.com/item?id=34639634
		- Моделі трансформери: an introduction and catalog https://arxiv.org/abs/2302.07730
		- Deepmind - формальні алгоритми для трансформерів https://arxiv.org/pdf/2207.09238.pdf
	- Jay Alammar explainers
		- https://jalammar.github.io/illustrated-transformer/
		- https://jalammar.github.io/visualizing-neural-machine-translation-mechanics-of-seq2seq-models-with-attention/
- karpathy on transformers
	- **Конвергенція*: Поточна консолідація в AI неймовірна. Коли я починав ~десять років тому, зір, мова, природна мова, навчання з підкріпленням тощо були повністю розділені; Ви не можете читати статті в різних сферах – підходи були абсолютно різними, часто навіть не базувалися на машинному обігу. У 2010-х роках усі ці сфери почали переходити 1) до машинного навчання та, зокрема, 2) до нейронних мереж. Архітектури були різними, але принаймні статті почали читатися більш схожими, усі вони використовували великі набори даних та оптимізували нейронні мережі. Але станом на бл. за останні два роки навіть архітектури нейронних мереж у всіх сферах почали виглядати ідентично – Transformer (можна визначити в ~200 рядках PyTorch [https://github.com/karpathy/minGPT/blob/master/mingpt/model.py…](https://t.co/xQL5NyJkLE)), з дуже незначними відмінностями. Або як потужна базова лінія, або (часто) як сучасний рівень.([tweetstorm](https://twitter.com/karpathy/status/1468370605229547522?s=20))
	- **Чому Transformers перемогли**: Transformer — це чудова архітектура нейронної мережі, оскільки це диференційований комп’ютер загального призначення. Він водночас: 1) виразний (у прямому проході) 2) оптимізований (через зворотне поширення+градієнтний спуск) 3) ефективний (високий обчислювальний графік паралелізму) [tweetstorm](https://twitter.com/karpathy/status/1582807367988654081)
		- https://twitter.com/karpathy/status/1593417989830848512?s=20
	- [BabyGPT](https://twitter.com/karpathy/status/1645115622517542913) з двома токенами 0/1 і довжиною контексту 3, розглядаючи його як кінцевий ланцюг Маркова. Його навчили на послідовності «111101111011110» протягом 50 ітерацій. Параметри та архітектура Transformer змінюють ймовірності на стрілках.
	- Створіть GPT з нуля https://www.youtube.com/watch?v=kCc8FmEb1nY
	- різні GPT з нуля в 60 LOC  https://jaykmody.com/blog/gpt-from-scratch/
- [137 emergent abilities of large language models](https://www.jasonwei.net/blog/emergence)
	- Емерджетні завдання з підказками: BIG-Bench і MMLU
	- Стратегії швидкого промптингу
		- [Instruction-following](https://openreview.net/forum?id=gEZrGCozdqR)
		- [Scratchpad](https://openreview.net/forum?id=iedYJm92o0a)
		- [Using open-book knowledge for fact checking](https://arxiv.org/abs/2112.11446)
		- [Chain-of-thought prompting](https://arxiv.org/abs/2201.11903)
		- [Differentiable search index](https://arxiv.org/abs/2202.06991)
		- [Self-consistency](https://arxiv.org/abs/2203.11171)
		- [Leveraging explanations in prompting](https://arxiv.org/abs/2204.02329)
		- [Least-to-most prompting](https://arxiv.org/abs/2205.10625)
		- [Zero-shot chain-of-thought](https://arxiv.org/abs/2205.11916)
		- [Calibration via P(True)](https://arxiv.org/abs/2207.05221)
		- [Multilingual chain-of-thought](https://arxiv.org/abs/2210.03057)
		- [Ask-me-anything prompting](https://arxiv.org/abs/2210.02441)
	- якісь відштовхи - це міраж? просто не використовуйте жорсткі показники
		- https://www.jasonwei.net/blog/common-arguments-regarding-emergent-abilities
		- https://hai.stanford.edu/news/ais-ostensible-emergent-abilities-are-mirage
  - Зображення
	  - Eugene Yan explanation of the Text to Image stack https://eugeneyan.com/writing/text-to-image/
	  - VQGAN/CLIP https://minimaxir.com/2021/08/vqgan-clip/
	  - 10 years of Image generation history https://zentralwerkstatt.org/blog/ten-years-of-image-synthesis
	  - Vision Transformers (ViT) Explained https://www.pinecone.io/learn/vision-transformers/
  - negative prompting https://minimaxir.com/2022/11/stable-diffusion-negative-prompt/
  - best papers of 2022 https://www.yitay.net/blog/2022-best-nlp-papers
  - [Predictability and Surprise in Large Generative Models](https://arxiv.org/pdf/2202.07785.pdf) - good survey paper of what we know about scaling and capabilities and rise of LLMs so far
- more prompt eng papers https://github.com/dair-ai/Prompt-Engineering-Guide
- https://creator.nightcafe.studio/vqgan-clip-keyword-modifier-comparison VQGAN+CLIP Keyword Modifier Comparison
- Історія трансформерів
	-Річард Сочер про їхній внесок у механізм уваги, що привів до трансформаторів https://overcast.fm/+r1P4nKfFU/1:00:00
	- https://kipp.ly/blog/transformer-taxonomy/ Цей документ є моїм поточним оглядом літератури для людей, які намагаються наздогнати ШІ. Він охоплює 22 моделі, 11 архітектурних змін, 7 методик після попереднього навчання та 3 методики навчання (і 5 речей, які не є жодною з перерахованих вище)
	- [Understanding Large Language Models A Cross-Section of the Most Relevant Literature To Get Up to Speed](https://magazine.sebastianraschka.com/p/understanding-large-language-models)
		- Я вважаю Банданау та ін. (2014), які, як я вважаю, першими запропонували концепцію застосування функції Softmax над балами маркерів для обчислення уваги, створивши основу для оригінального трансформатора Васвані та ін. (2017) https://news.ycombinator.com/item?id=35589756
	- https://finbarrtimbers.substack.com/p/five-years-of-progress-in-gpts GPT1/2/3, Megatron, Gopher, Chinchilla, PaLM, LLaMa
	-хороший підсумковий документ (8 речей, які слід знати) https://cims.nyu.edu/~sbowman/eightthings.pdf



Ми порівняли 126 модифікаторів ключових слів із однаковою підказкою та початковим зображенням. Ось такі результати.
  - https://creator.nightcafe.studio/collection/8dMYgKm1eVXG7z9pV23W
-Google випустив PartiPrompts як еталон: https://parti.research.google/ "PartiPrompts (P2) — це багатий набір із понад 1600 підказок англійською мовою, який ми випускаємо в рамках цієї роботи. P2 можна використовувати для вимірювання можливостей моделі в різних категоріях і аспектах завдання."
- Відеоуроки
  - Pixel art https://www.youtube.com/watch?v=UvJkQPtr-8s&feature=youtu.be
- Історія cтатей:
	- 2008: Unified Architecture for NLP (Collobert-Weston) https://twitter.com/ylecun/status/1611921657802768384
	- 2015: [Semi-supervised sequence learning](https://arxiv.org/abs/1511.01432) https://twitter.com/deliprao/status/1611896130589057025?s=20
	- 2017: Transformers (Vaswani et al)
	- 2018: GPT (Radford et al)
	- 
- Різне
  - StabilityAI CIO perspective https://danieljeffries.substack.com/p/the-turning-point-for-truly-open?sd=pf
  - https://github.com/awesome-stable-diffusion/awesome-stable-diffusion
  - https://github.com/microsoft/LMOps guide to msft prompt research
  - gwern за кадром обговорює Bing, GPT4 і відносини Microsoft-OpenAI https://www.lesswrong.com/posts/jtoPawEhLNXNxvgTT/bing-chat-is-blatantly-aggressively-misaligned

### інші подібні списки

- https://gist.github.com/rain-1/eebd5e5eb2784feecf450324e3341c8d
- https://github.com/underlines/awesome-marketing-datascience/blob/master/awesome-ai.md#llama-models

## Спільноти

- StableDiffusion Discord https://discord.com/invite/stablediffusion
- LAION discord https://discord.gg/xBPBXfcFHd
- Eleuther discord: https://www.eleuther.ai/get-involved/ ([primer](https://blog.eleuther.ai/year-one/))
- https://reddit.com/r/stableDiffusion
- Akhaliq Discord: https://discord.gg/nYqfg4gnBt
- Karpathy Discord: https://discord.gg/3zy8kqD9Cp
- HuggingFace Discord: https://discuss.huggingface.co/t/join-the-hugging-face-discord/11263
- Deforum Discord https://discord.gg/upmXXsrwZc
- Lexica Discord https://discord.com/invite/bMHBjJ9wRh
- Perplexity Discord https://discord.com/invite/kWJZsxPDuX
- Chatgpt Hackers https://www.chatgpthackers.dev/
- Агенти
	- AutoGPT discord
	- BabyAGI discord
- Midjourney's discord
  - how to use Midjourney v4 https://twitter.com/fabianstelzer/status/1588856386540417024?s=20&t=PlgLuGAEEds9HwfegVRrpg
- https://stablehorde.net/
- don't forget Reddit
	- https://www.reddit.com/r/LocalLLaMA/
	- https://www.reddit.com/r/bing
	- https://www.reddit.com/r/openai


##Люди

Цей список буде застарілим, але допоможе вам почати. Мій живий список людей, яких слід підписувати, знаходиться за адресою: https://twitter.com/i/lists/1585430245762441216

- Дослідники/розробники
  - https://twitter.com/_jasonwei
  - https://twitter.com/johnowhitaker/status/1565710033463156739
  - https://twitter.com/altryne/status/1564671546341425157
  - https://twitter.com/SchmidhuberAI
  - https://twitter.com/nearcyan
  - https://twitter.com/karinanguyen_
  - https://twitter.com/abhi_venigalla
  - https://twitter.com/advadnoun
  - https://twitter.com/polynoamial
  - https://twitter.com/vovahimself
  - https://twitter.com/sarahookr
  - https://twitter.com/shaneguML
  - https://twitter.com/MaartenSap
  - https://twitter.com/ethanCaballero
  - https://twitter.com/ShayneRedford
  - https://twitter.com/seb_ruder
  - https://twitter.com/rasbt
  - https://twitter.com/wightmanr
  - https://twitter.com/GaryMarcus
  - https://twitter.com/ylecun
  - https://twitter.com/karpathy
  - https://twitter.com/pirroh
  - https://twitter.com/eerac
- Новини/Агрегатори
  - https://twitter.com/ai__pub
  - https://twitter.com/WeirdStableAI
  - https://twitter.com/multimodalart
  - https://twitter.com/LastWeekinAI
  - https://twitter.com/paperswithcode
  - https://twitter.com/DeepLearningAI_
  - https://twitter.com/dl_weekly
  - https://twitter.com/slashML
  - https://twitter.com/_akhaliq
  - https://twitter.com/aaditya_ai
  - https://twitter.com/bentossell
  - https://twitter.com/johnvmcdonnell
- Засновники/білдери/венчурні капіталісти
  - https://twitter.com/levelsio
  - https://twitter.com/goodside
  - https://twitter.com/c_valenzuelab
  - https://twitter.com/Raza_Habib496
  - https://twitter.com/sharifshameem/status/1562455690714775552
  - https://twitter.com/genekogan/status/1555184488606564353
  - https://twitter.com/levelsio/status/1566069427501764613?s=20&t=camPsWtMHdSSEHqWd0K7Ig
  - https://twitter.com/amanrsanger
  - https://twitter.com/ctjlewis
  - https://twitter.com/sarahcat21
  - https://twitter.com/jackclarkSF
  - https://twitter.com/alexandr_wang
  - https://twitter.com/rameerez
  - https://twitter.com/scottastevenson
  - https://twitter.com/denisyarats
- Stability
  - https://twitter.com/StabilityAI
  - https://twitter.com/StableDiffusion
  - https://twitter.com/hardmaru
  - https://twitter.com/JJitsev
- OpenAI
  - https://twitter.com/sama
  - https://twitter.com/ilyasut
  - https://twitter.com/miramurati
- HuggingFace
  - https://twitter.com/younesbelkada
- Художники
  - https://twitter.com/karenxcheng/status/1564626773001719813
  - https://twitter.com/TomLikesRobots
- Іншe 
  - Компанії
    - https://twitter.com/AnthropicAI
    - https://twitter.com/AssemblyAI
    - https://twitter.com/CohereAI
    - https://twitter.com/MosaicML
    - https://twitter.com/MetaAI
    - https://twitter.com/DeepMind
    - https://twitter.com/HelloPaperspace
- Боти та програми
  - https://twitter.com/dreamtweetapp
  - https://twitter.com/aiarteveryhour


##Цитати, реальність і демотивація

- Вузькі, нудні випадки використання домену https://twitter.com/WillManidis/status/1584900092615528448 і https://twitter.com/WillManidis/status/1584900100480192516
- антихайп https://twitter.com/alexandr_wang/status/1573302977418387457
- антихайп https://twitter.com/fchollet/status/1612142423425138688?s=46&t=pLCNW9pF-co4bn08QQVaUg
- підказка англ меми
- https://twitter.com/_jasonwei/status/1516844920367054848
- речі, з якими бореться stablediffusion https://opguides.info/posts/aiartpanic/
- Новий Google
   - https://twitter.com/alexandr_wang/status/1585022891594510336
— Новий Powerpoint
   - через emad
— Додавання підказок за замовчуванням в інтерфейс користувача
   - DALLE: https://twitter.com/levelsio/status/1588588688115912705?s=20&t=0ojpGmH9k6MiEDyVG2I6gg
– Попередніх зим було дві – 1974-1980 і 1987-1993 років. https://www.erichgrunewald.com/posts/the-prospect-of-an-ai-winter/
- Це просто матричне множення/стохастичні папуги
– Навіть скептик до магістра права Янн ЛеКун каже, що у магістратури є певний рівень розуміння: https://twitter.com/ylecun/status/1667947166764023808
	- 



## Право, етика та конфіденційність

- NSFW filter https://vickiboykis.com/2022/11/18/some-notes-on-the-stable-diffusion-safety-filter/
- On "AI Art Panic" https://opguides.info/posts/aiartpanic/
	- [I lost everything that made me love my job through Midjourney](https://old.reddit.com/r/blender/comments/121lhfq/i_lost_everything_that_made_me_love_my_job/)
- Yannick influencing OPENRAIL-M https://www.youtube.com/watch?v=W5M-dvzpzSQ
- art schools accepting AI art https://twitter.com/DaveRogenmoser/status/1597746558145265664
- DRM issues https://undeleted.ronsor.com/voice.ai-gpl-violations-with-a-side-of-drm/
- stealing art [https://stablediffusionlitigation.com](https://stablediffusionlitigation.com/)
	- http://www.stablediffusionfrivolous.com/
	- stable attribution https://news.ycombinator.com/item?id=34670136
	- coutner argument for disney https://twitter.com/jonst0kes/status/1616219435492163584?s=46&t=HqQqDH1yEwhWUSQxYTmF8w
	- research on stable diffusion copying https://twitter.com/officialzhvng/status/1620535905298817024?s=20&t=NC-nW7pfDa8nyRD08Lx1Nw This paper used Stable Diffusion to generate 175 million images over 350,000 prompts and only found 109 near copies of training data. Am I right that my main takeaway from this is how good Stable Diffusion is at *not* memorizing training examples?
- Ліцензування
	- [AI weights are not open "source" - Sid Sijbrandij](https://opencoreventures.com/blog/2023-06-27-ai-weights-are-not-open-source/)

## Вирівнювання, Безпека

- Anthropic - https://arxiv.org/pdf/2112.00861.pdf
	- Корисно: спробуйте зробити те, що вас просять. стисло, ефективно. просити подальші дії. перенаправляти погані запитання.
- Чесний: надайте точну інформацію, висловіть невпевненість. не імітуйте відповіді, які очікуються від експерта, якщо він не має можливостей/знань
	- Нешкідливий: не образливий/дискримінаційний. відмовитися від допомоги в небезпечних діях. розпізнавати під час надання делікатної/непрямої поради
- критика та межі як майбутній напрямок https://twitter.com/davidad/status/1628489924235206657?s=46&t=TPVwcoqO8qkc7MuaWiNcnw
- Лише весь твір Елізера
	- https://twitter.com/esyudkowsky/status/1625922986590212096
	- agi список смертельних випадків https://www.lesswrong.com/posts/uMQ3cqWDPHhjtiesc/agi-ruin-a-list-of-lethalities
	- nзауважте, що Елізер зробив суперечливі коментарі [in the past](https://twitter.com/johnnysands42/status/1641349759754485760?s=46&t=90xQ8sGy63D2OtiaoGJuww) and also in [recent times](https://twitter.com/lorakolodny/status/1641448759086415875?s=46&t=90xQ8sGy63D2OtiaoGJuww) ([TIME article](https://time.com/6266923/ai-eliezer-yudkowsky-open-letter-not-enough/))
- Коннор Ліхі може бути більш розумною/виваженою/технічно компетентною версією yud https://overcast.fm/+aYlOEqTJ0
	- це не просто фабрики скріпок
	- https://www.lesswrong.com/posts/HBxe6wdjxK239zajf/what-failure-looks-like
- лист про перерву на 6 місяців
	- https://futureoflife.org/open-letter/pause-giant-ai-experiments/
	- yann lecun vs andrew ng https://www.youtube.com/watch?v=BY9KV8uCtj4
	- https://scottaaronson.blog/?p=7174
	- [emily bender response](https://twitter.com/emilymbender/status/1640920936600997889)
	- [Geoffrey Hinton leaving Google](https://news.ycombinator.com/item?id=35771104) 
	- супроводжується публічним листом одним реченням https://www.nytimes.com/2023/05/30/technology/ai-threat-warning.html
- xrisk 
		- Чи справді уникнення вимирання від ШІ є невідкладним пріоритетом? ([link](https://link.mail.beehiiv.com/ss/c/5J8WPrGlKFK1BUsRYoWIfdCHPD-3Xbi8FugDN8_LxoMLoHhMJlEG7wG6Qm_xTk5kjhv7y5vwidMdRiSXu8XoBiq8nEOR34GaAFwHPM3qm-KgbLw6_hl3AQd9rRxt7mbTHvXRNeF6hfODzGg5z4t8D3ZdIldVTpoAGQ-KmKNEnmzBudTJIJtP1kjZLr1QqJYX/3wo/z-oFlqV_RUGtJd6OO2FogA/h13/XrV7_YgyheO615JC1X8VasmPENc7KRnJrp03iAlmoXw)) 
	-   ШІ – це не гонка озброєнь. ([link](https://link.mail.beehiiv.com/ss/c/znicDlvJFyGBhcMAVWxZFpwlt5VC0YnUsV4gzm_4ut3qiUuoiY9_n0aSS6Uv0inD2_kx5JhKOVXSRbXMrV7VwL_fuIMlfwAiTSTTCxo56Xv58IWHdUClCfyt4alUnKRf2MV5a7rIM0KG4vwVLObEua0i3t5UIvPlbHybyFluj52xGYswNiQUMZl2OrDzh1u4oLAvnCVkTUi5vCX0i6-N8A/3wo/z-oFlqV_RUGtJd6OO2FogA/h14/K2LmS7FyAGW-u4j6oHnp_bKapwqFG_Gb4MC5XPpKJsM)) 
	-   Якщо ми збираємося назвати ШІ «ризиком вимирання», нам потрібно пояснити, як це може статися. ([link](https://link.mail.beehiiv.com/ss/c/znicDlvJFyGBhcMAVWxZFsLJphRoW5fZiwv4ALj3pNMBRHKVGkJIME1sXnwK-P46O3jH_jtoC_wqyCeroi2bRUKEUKd_QQvXSoMgu3Nqbw99wsPjSDl_Lt6RSk7bni0KT4c1-gstNpWdPoUbj3air5NbOAbvtp5P9ds1xCm4qG-6dvoJELH0HHB7G9FO2ZFlXPTm37nswLD77q6opSiWnrTEHhHsCo37yO01bFol4LeaSr8F4e_WynvF0QrKLNaSKf0rDpyMSn__lxmbRl6M1A/3wo/z-oFlqV_RUGtJd6OO2FogA/h15/SYpE89X1W3Z_qSjH8YJmhLYYRRgjUHJzn2WILhBIcxw))

### регулювання

- китайське регулювання https://www.chinalawtranslate.com/en/overview-of-draft-measures-on-generative-ai/
	- https://twitter.com/mmitchell_ai/status/1647697067006111745?s=46&t=90xQ8sGy63D2OtiaoGJuww
	- Китай є єдиною великою світовою державою, яка явно [regulates](https://info.deeplearning.ai/e3t/Ctc/LX+113/cJhC404/VVt-xv1bfQFxVTDC381T3c1vVLsY3L4_gp1wN1FQ0th3q3n_V1-WJV7CgH8lW4wLFDD1Q5sD1W6QG0gj2gQKZ5W2WNS9Z5gKTB8W6jF2Dc8ltmWfW1kwRcc4LNmnNW2_F-zw6rWXtDN8M32V9_0Z1cN1gwSlkLF9WBW6yYMS68JLJYjN1wstfhr0tvgW5DCclJ4zMFhNN6tQ4vt1P5bVW5w-L-275lv9LW5zhjMk7CCjjcW20ChgZ57-8l2W50dQgR1_tfL-VqXDdY2t227nVzlNDX4m43yWW4D6GXl6Mf9JvW3qShZ085BMXqW5S2j7D4VWf5lW4c37Wn4lbf-NW4W6Hxl3CCDHRW451x4X8wNPKHW5zc90X90FjXcW97Qn_B7RdzpP3nQX1) generative AI
- Італія забороняє chatgpt
- -   а своїй щорічній зустрічі в Японії Велика сімка (G7), неформальний блок промислово розвинутих демократичних урядів, [оголосила](https://info.deeplearning.ai/e3t/Ctc/LX+113/cJhC404/VVt-xv1bfQFxVTDC381T3c1vVLsY3L4_gp1wN1FQ0s_3q3nJV1-WJV7CgFv5W51g32V2hBgR-N3j2W3szNMJlW80w4Xv5Gg2S8N4_ZHQFYd4cRW8yvm4F2zg5qpW5xfrS61fJ8H4W49Nj5Y2zWcRbW97ym606Vq3X6W2-51W529GnLcW2zlMRl3qKmBCW8jd69B7nRzmFV5K0lP4FzrchW6nxHbj1vFJPqN3sbnlvFM2WhW6PNj-t5YfVS3W6pl7681yBKGxN1R1Mbj8wWj4W22BS_g1BH_1yW7pT8c47QKBQFW64WfHc80PxjRV6dQN42mCqRMW3yJrxC3DX4_5W5yqFbL34kwc0W770qZv2fjyv03bJQ1)Хіросімський процес, міжурядова цільова група, уповноважена досліджувати ризики генеративного ШІ. Члени G7, до яких входять Канада, Франція, Німеччина, Італія, Японія, Сполучене Королівство та Сполучені Штати, пообіцяли розробити взаємосумісні закони та регулювати ШІ відповідно до демократичних цінностей. До них належать справедливість, підзвітність, прозорість, безпека, конфіденційність даних, захист від зловживань і повага до прав людини.
-   Президент США Джо Байден [issued](https://info.deeplearning.ai/e3t/Ctc/LX+113/cJhC404/VVt-xv1bfQFxVTDC381T3c1vVLsY3L4_gp1wN1FQ0s55nCT_V3Zsc37CgQX9W7wTfL38m-2KKW3mGNtx8sgMgJW10rjg65dMw5qN3jtZLMqRgQbV_3DXH2yr2HbW4vs2Tm43thGvW6fK8f72N6w37N53TdBst-8D1W6yzHrb70MHkTW1ckbRd5NfDP9W2j6yWK34KFvtW18lscs3lQ0G6W4GFgyx486-vdW5NJBQv4tvxYpW36FqGc4md2XfW2Fgj6n2fd-BSW3PyPVH9bD8W3N61PDTSyzVy1W2QSSm07tHjwWW8zG-Kl3TPwmfVMNjLb7Nnhk4W2B_zlf7n91mNW806djL3zxyMFW5RpR1Q9kcL0yW7ss_7m92D7Z-W4fWJYk3xBb3yN5bZbNkSvb14N2kgsftyLf7cN1WmZDl5Sw63W4FcWFn65g7DsVzPJZP2qtH36W3vfw782XRtSbW834rhB5jGZ7RW6K9z1d87ns4N38SY1) aстратегічний план для ШІ. Ініціатива закликає регуляторні органи США розробити загальнодоступні набори даних, контрольні показники та стандарти для навчання, вимірювання та оцінки систем штучного інтелекту.
-   Раніше цього місяця регулятор конфіденційності даних Франції [announced](https://info.deeplearning.ai/e3t/Ctc/LX+113/cJhC404/VVt-xv1bfQFxVTDC381T3c1vVLsY3L4_gp1wN1FQ0s_3q3nJV1-WJV7CgTpxW8C6yq247bfj8W4mQv0-4hl35_W8SPtZ52JXPlxW1Fkb5p54f30RW6sj0m71XsJ4yF7-b6kBx5vTW7cwGKJ6RcqpFW5325sQ2R54VbW79rbsP4wh6MyW2MwyS_6CSJfwW8VBz1y1M5_4nW2nhxPD5vZw17MCVDrTvH8ljW1JYH0t8DPm23W3BPQvW69f5TFW5ms3_413vDbJVw9GyW1yMYBfW6zpGVw12swbdV_wmsh11rtb0Vlzk0b6ZkhpZW1XWkdG7yNYpsW38p95C5jXCx7W4qrc4w1_q_sdW5RD3Jv7bdxpv2Gp1) a framework for regulating generative AI.

## Різне

- Whisper
  - https://huggingface.co/spaces/sensahin/YouWhisper YouWhisper converts Youtube videos to text using openai/whisper.
  - https://twitter.com/jeffistyping/status/1573145140205846528 youtube whipserer
  - multilingual subtitles https://twitter.com/1littlecoder/status/1573030143848722433
  - video subtitles https://twitter.com/m1guelpf/status/1574929980207034375
  - you can join whisper to stable diffusion for reasons https://twitter.com/fffiloni/status/1573733520765247488/photo/1
  - known problems https://twitter.com/lunixbochs/status/1574848899897884672 (edge case with catastrophic failures)
- textually guided audio https://twitter.com/FelixKreuk/status/1575846953333579776
- Codegen
  - CodegeeX https://twitter.com/thukeg/status/1572218413694726144
  - https://github.com/salesforce/CodeGen https://joel.tools/codegen/
- pdf to structured data - Impira used t to do it (dead link: https://www.impira.com/blog/hey-machine-whats-my-invoice-total) but if you look hard enough on twitter there are some alternatives
- text to Human Motion diffusion https://twitter.com/GuyTvt/status/1577947409551851520
  - abs: https://arxiv.org/abs/2209.14916 
  - project page: https://guytevet.github.io/mdm-page/
