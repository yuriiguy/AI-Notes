ELI5: https://news.ycombinator.com/item?id=35977891
Стаття 2017 року
- https://ai.googleblog.com/2017/08/transformer-novel-neural-network.html?m=1
- 30-хвилинний відеоогляд https://www.youtube.com/watch?v=iDulhoQ2pro
-
Ілюстрований трансформер - [https://jalammar.github.io/illustrated-transformer/](https://jalammar.github.io/illustrated-transformer/)

![https://vinija.ai/models/assets/transformers/2.png](https://vinija.ai/models/assets/transformers/2.png)
- LSTM помер. Хай живуть трансформери! ([обговорення](https://www.youtube.com/watch?v=S27pHKBEp30))
-  еволюція методів обробки природної мови (NLP), починаючи з обмежень моделей сумки слів і ванільних рекурентних нейронних мереж (RNN), які страждають від зникаючих і зростаючих градієнтів.
- Запровадження довгострокової короткочасної пам’яті (LSTM) вирішило ці проблеми, але все ще було складним для навчання та не вистачало здібностей до навчання перенесення, що призвело до розробки моделі трансформатора.
- Модель трансформатора використовує **самоувагу** і **пряму нейронну мережу** для зчитування вхідних послідовностей і створення вихідних послідовностей, включаючи **багатосторонню увагу** для генерування кількох виходів уваги з різними наборами параметрів.
	- Ключові нововведення моделі трансформера включають **позиційне кодування** і використання функцій **активації ReLU**.
- Доповідач підкреслює переваги використання трансформаторів і моделей, таких як Roberta, для навчання моделей на великих текстових даних без контролю, що дозволяє передавати навчання та зменшувати час і ресурси для навчання.
- Незважаючи на заміну в більшості областей трансформаторами, LSTM все ще має застосування для управління в режимі реального часу.
- Доповідач також порівнює слово CNN із трансформаторами та зауважує, що трансформери можуть ефективніше пропонувати контекстні відповіді в усьому документі.
- Little Book of Deep Learning ([pdf](https://fleuret.org/public/lbdl.pdf))
- Поняття шару
- Лінійний шар
- Функції активації
- Об'єднання
- Викинути
- нормалізація шарів
- Пропуск з'єднань
- Шари уваги
- Вбудовування токенів
- Позиційне кодування
- Архітектури
- Багатошарові перцептрони
- Згорткові мережі
- До уваги моделей
– Нагадування, що мій курс глибокого навчання [@unige_en](https://twitter.com/unige_en) повністю доступний онлайн. 1000+ слайдів, ~20 годин скрінкастів. [https://fleuret.org/dlc/](https://t.co/6OVyjPdwrC)
- https://e2eml.school/transformers.html Трансформери з нуля

https://news.ycombinator.com/item?id=35712334
Ілюстрований трансформатор фантастичний, але я б запропонував тим, хто збирається його вивчати, прочитати попередні статті серії, щоб отримати основу для глибшого розуміння, а також наступні статті, які стосуються GPT і BERT, ось список:

Візуальний та інтерактивний посібник з основ нейронних мереж - [https://jalammar.github.io/visual-interactive-guide-basics-n...](https://jalammar.github.io/visual-interactive-guide-basics-neural-networks/)

A Visual And Interactive Look at Basic Neural Network Math - [https://jalammar.github.io/feedforward-neural-networks-visua...](https://jalammar.github.io/feedforward-neural-networks-visual-interactive/)- Згорткові мережі
- До уваги моделей
– Нагадування, що мій курс глибокого навчання [@unige_en](https://twitter.com/unige_en) повністю доступний онлайн. 1000+ слайдів, ~20 годин скрінкастів. [https://fleuret.org/dlc/](https://t.co/6OVyjPdwrC)
- https://e2eml.school/transformers.html Трансформери з нуля


https://news.ycombinator.com/item?id=35712334
Ілюстрований трансформатор фантастичний, але я б запропонував тим, хто збирається його вивчати, прочитати попередні статті серії, щоб отримати основу для глибшого розуміння, а також наступні статті, які стосуються GPT і BERT, ось список:

Візуальний та інтерактивний посібник з основ нейронних мереж - [https://jalammar.github.io/visual-interactive-guide-basics-n...](https://jalammar.github.io/visual-interactive-guide-basics-neural-networks/)

Візуальний та інтерактивний погляд на базову математику нейронних мереж - [https://jalammar.github.io/feedforward-neural-networks-visua...](https://jalammar.github.io/feedforward-neural-networks-visual-interactive/)

Візуалізація моделі нейронного машинного перекладу (механіка моделей Seq2seq з увагою) - [https://jalammar.github.io/visualizing-neural-machine-transl...](https://jalammar.github.io/visualizing-neural-machine-translation-mechanics-of-seq2seq-models-with-attention/)


The Illustrated BERT, ELMo та компанія (Як NLP зламав Transfer Learning) - [https://jalammar.github.io/illustrated-bert/](https://jalammar.github.io/illustrated-bert/)

Ілюстрований GPT-2 (візуалізація трансформаторних мовних моделей) - [https://jalammar.github.io/illustrated-gpt2/](https://jalammar.github.io/illustrated-gpt2/)

Як працює GPT3 – візуалізації та анімації – [https://jalammar.github.io/how-gpt3-works-visualizations-ani...](https://jalammar.github.io/how-gpt3-works-visualizations-animations/)

Ілюстрований пошуковий трансформатор - [https://jalammar.github.io/illustrated-retrieval-transformer...](https://jalammar.github.io/illustrated-retrieval-transformer/)

Ілюстрована Stable Diffusion - [https://jalammar.github.io/illustrated-stable-diffusion/](https://jalammar.github.io/illustrated-stable-diffusion/)

Якщо ви хочете навчитися їх кодувати, ця книга чудова: [https://d2l.ai/chapter_attention-mechanisms-and-transformers...](https://d2l.ai/chapter_attention-mechanisms-and-transformers/index.html)

Transformer Taxonomy (останній освітлений огляд)
https://kipp.ly/blog/transformer-taxonomy/
- Він охоплює 22 моделі, 11 архітектурних змін, 7 методик після попереднього навчання та 3 методики навчання (і 5 речей, які не є жодною з перерахованих вище).

візуалізація уваги https://catherinesyeh.github.io/attn-docs/

### Пояснювачі

-   [**The illustrated transformer**](https://jalammar.github.io/illustrated-transformer/): Більш технічний огляд архітектури трансформатора від Джея Аламмара.
-   **[The annotated transformer](http://nlp.seas.harvard.edu/annotated-transformer/)**: Глибока публікація, якщо ви хочете зрозуміти трансформери на рівні вихідного коду. Потрібні певні знання PyTorch.
-   [**Let’s build GPT: from scratch, in code, spelled out**](https://www.youtube.com/watch?v=kCc8FmEb1nY): Для інженерів Karpathy робить відеоінструкцію про те, як створити модель GPT.
-   **[The illustrated Stable Diffusion](https://jalammar.github.io/illustrated-stable-diffusion/)****:** Знайомство з моделями прихованої дифузії, найпоширенішим типом генеративної моделі ШІ для зображень.
-   **[RLHF: Reinforcement Learning from Human Feedback](https://huyenchip.com/2023/05/02/rlhf.html)**: Чіп Гюєн пояснює RLHF, який може змусити LLM поводитись більш передбачувано та зручніше для людини. Це один із найважливіших, але найменш зрозумілих аспектів таких систем, як ChatGPT.
-   [**Reinforcement learning from human feedback**](https://www.youtube.com/watch?v=hhiLw5Q_UFg): Комп’ютерний науковець і співзасновник OpenAI Джон Шульман детальніше розповідає про поточний стан, прогрес і обмеження LLM з RLHF.

### Курси

-   [**Stanford CS25**](https://www.youtube.com/watch?v=P127jhj-8-Y): Transformers United, онлайн-семінар про трансформери.
-   **[Stanford CS324](https://stanford-cs324.github.io/winter2022/)**: Великі мовні моделі з Персі Лянгом, Тацу Хашимото та Крісом Ре, що охоплюють широкий спектр технічних і нетехнічних аспектів LLM.

### Довідка та коментарі

-   **[Predictive learning, NIPS 2016](https://www.youtube.com/watch?v=Ount2Y4qxQo&t=1072s)**: У цьому ранньому виступі Янн ЛеКун наводить вагомі аргументи на користь неконтрольованого навчання як критичного елемента масштабної архітектури моделей ШІ. Перейдіть до [19:20](https://youtu.be/Ount2Y4qxQo?t=1160) для відомої аналогії з тортом, яка досі є однією з найкращих ментальних моделей для сучасного ШІ.
-   [**Штучний інтелект для повного самостійного керування автомобілем у Tesla**](https://www.youtube.com/watch?v=hx7BXih7zx8): ще одна класична доповідь Karpathy, цього разу присвячена системі збору даних Tesla. Починаючи з [8:35](https://youtu.be/hx7BXih7zx8?t=515) одна з найвидатніших вигадок зі штучним інтелектом усіх часів, яка пояснює, чому довгострокові проблеми (у цьому випадку виявлення знаку зупинки) такі складні .
- **[Гіпотеза масштабування](https://gwern.net/scaling-hypothesis)**: одним із найдивовижніших аспектів LLM є те, що масштабування — додавання більше даних і обчислень — просто підвищує точність. GPT-3 була першою моделлю, яка це чітко продемонструвала, і публікація Гверна чудово пояснює інтуїцію, що стоїть за цим.
-   [**Значення Chinchilla про дику природу**](https://www.lesswrong.com/posts/6Fpvch8RR29qLEWNH/chinchilla-s-wild-implications): цей допис номінально пояснює важливий документ про шиншиллу (див. нижче). суть великого питання масштабування LLM: чи не вичерпуються дані? Це ґрунтується на публікації вище та дає оновлений погляд на закони масштабування.
- **[Огляд великих мовних моделей](https://arxiv.org/pdf/2303.18223v4.pdf)**: повна розбивка поточних LLM, включаючи графік розробки, розмір, стратегії навчання, навчальні дані, апаратне забезпечення, і більше.
- [**Іскри загального штучного інтелекту: ранні експерименти з GPT-4**](https://arxiv.org/abs/2303.12712): ранній аналіз можливостей GPT-4, найсучаснішого на даний момент, проведеного Microsoft Research LLM, відносно людського інтелекту.
- [**Революція ШІ: як Auto-GPT відкриває нову еру автоматизації та творчості**](https://pub.towardsai.net/the-ai-revolution-how-auto-gpt-unleashes-a- new-era-of-automation-and-creativity-2008aa2ca6ae): Знайомство з Auto-GPT та агентами ШІ загалом. Ця технологія є дуже ранньою, але її важливо зрозуміти — вона використовує доступ до Інтернету та самостійно створені підзавдання для вирішення конкретних, складних проблем або цілей.
- **[Ефект Валуїджі](https://www.lesswrong.com/posts/D7PumeYTDPfBTp3i7/the-waluigi-effect-mega-post)**: номінальне пояснення «ефекту Валуїджі» (тобто, чому « alter egos» з’являються в поведінці LLM), але цікаві здебільшого своїм глибоким зануренням у теорію підказок LLM.

## спалах уваги

https://twitter.com/amanrsanger/status/1657835933503479808?s=46&t=90xQ8sGy63D2OtiaoGJuww

## hyena

- https://hazyresearch.stanford.edu/blog/2023-03-07-hyena


## інтерпретативність трансформера

openai мав статтю із маркуванням gpt

https://twitter.com/generatorman_ai/status/1664410300110766082?s=20
- Індукційні головки, модульне доповнення, схема непрямого об'єкта, OthelloGPT.


## Генеалогічне дерево трансформера

Застосування Transformers. Новий опитувальний документ, що висвітлює основні застосування Transformers для завдань глибокого навчання. Включає повний список моделей Transformer. [https://arxiv.org/abs/2306.07303](https://t.co/z0y6R4CUh6)

Ефективні методи обробки природної мови: опитування У ньому наведено ефективні методи, які використовують менше ресурсів, водночас дають результати, порівняні з ресурсомісткими системами НЛП.
[https://pbs.twimg.com/media/FhnMjm7WYAA8e18?format=jpg&name=medium]
abs: [https://arxiv.org/abs/2209.00099](https://t.co/99Gp0rPZHi) 
