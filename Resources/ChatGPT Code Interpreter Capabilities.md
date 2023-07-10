## Хронологія
-23 березня - попередній перегляд плагінів https://openai.com/blog/chatgpt-plugins
- gdb video clip https://twitter.com/gdb/status/1638971232443076609
	- Він пише та виконує код MoviePy ([https://zulko.github.io/moviepy/](https://t.co/SHPNZOLCHp)), який використовує ffmpeg під капотом. Таким чином, цей час в основному йде на очікування запуску ffmpeg (великий крок у порівнянні зі звичайним вузьким місцем пошуку набору аргументів, щоб робити те, що я хочу!).
- 6-13 липня - реліз GA https://help.openai.com/en/articles/6825453-chatgpt-release-notes

## Системне повідомлення Інтерпретатора коду

https://chat.openai.com/share/38301a21-bf09-4274-848b-b9cd5523d461

й requirements.txt https://twitter.com/swyx/status/1677589535587467264
([annotated](https://chat.openai.com/share/a4336af0-6faa-4ffb-b5b0-a3bd7ef8f3aa))

## Підтверджені можливості під час запуску
- Відео маніпуляції
- за допомогою moviePy https://twitter.com/gdb/status/1638971232443076609
- Прийнятні типи файлів
	- .zip-файли: він може розархівувати файли та продовжувати відкривати та перевіряти ці файли
- "Я перепрошую за помилку. Змінну `unzip_folder` також було втрачено під час скидання. Нам потрібно буде ще раз витягти дані з zip-файлу, перш ніж продовжити"
- файли .csv
- файли .xls https://twitter.com/emollick/status/1652170706312896512
- Файли .png
- спрощене редагування та зміна розміру зображень
- файли .mov
- Вміє малювати https://twitter.com/swyx/status/1677567255377494016?s=20
- але має проблеми
- створити діаграму graphviz - код https://chat.openai.com/share/adc73608-4c80-497b-ad03-31de28bfa919
- Може картографувати за допомогою folium
	- https://twitter.com/emollick/status/1677570911124242433?s=20
	- відобразити карту листка на зображенні та показати зображення
- аналітик даних
- **Відкритий аналіз**:
		- "Here is some data on superhero powers, look through it and tell me what you find"
		- "I am interested in doing some predictive modeling, where we can predict what powers a hero might have based on other factors."
	- **Поєднання даних**: "Could you first combine the two datasets"
	- **Перевірки цілісності даних**: "... and confirm that they combined properly"
	- **Очищення даних**: "Does the data need cleaning in any way?"
	- **Попередня обробка даних**: "Great! Cluster analysis can help us group similar superheroes together based on their attributes. Before we start, we need to preprocess our data. This will involve the following steps:" https://chat.openai.com/share/770ab170-8fed-402f-850f-e6d7273e77cd
	- **Підсумок аналізу**: "What is your summary of all this analysis, in bullet points?"
	- **Створіть інтерактивну інформаційну панель** https://emollick.github.io/Superhero/
		- і графіки https://emollick.github.io/3Dmusic/
		- і картиhttps://github.com/emollick/GPTflightmap.github.io
	- Dataviz
		- ![https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F55543b86-b8ec-45db-84ec-649fe0237097_3208x2000.png](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F55543b86-b8ec-45db-84ec-649fe0237097_3208x2000.png)
- Поведінка
- **Надання варіантів і пауза для підтвердження**
		- Great! Before we proceed, we need to further refine the scope of our predictive task. As you might notice, we have a large number of potential powers (labels) to predict, which could make the problem very complex. Would you like to predict all possible powers, or focus on a specific subset of powers?
		- Another important point to note is that our current dataset is quite large and might be too complex for certain algorithms. We might need to simplify our problem further by reducing the number of features. This could be done through a dimensionality reduction technique or simply selecting a subset of the most relevant features.
		- Finally, we need to choose a suitable model for our multi-label classification task. Some possibilities include decision trees, random forests, or neural networks. Each of these options has its own strengths and weaknesses, and the best choice often depends on the specific characteristics of the dataset. Please let me know how you would like to proceed.
		- "Pick which you think is best, be clear about strengths and weaknesses"
		- Outliers can have a large influence on machine learning models, particularly those that use distance measures like Random Forest. Given this, we could:
			-   Remove these outliers from the data.
			-   Winsorize the data, which means capping the extreme values at a certain threshold.
			-   Leave the data as-is if we believe the extreme values are accurate and important to the model.
		- Which approach would you like to take?
	- Recovery from minor data issues
		- `It seems like there are still some values in the data that are causing issues. In the error message, it's mentioned that the input contains NaN, infinity, or a value too large for dtype('float32').`
		- `It appears there are no missing (NaN) or infinite values in the dataset after our preprocessing steps. The error during model training might be due to a different issue.`
		- `Looking at the unique values in the 'Height' and 'Weight' columns, we see some extreme values. For example, heights of 975 cm and 876 cm, and weights of 900 kg and 855 kg are unusually high for humans and most known superhero characters. These could be misrecorded data, placeholder values for unknowns, or correct data for exceptionally large characters.`
		- `IndexError: index 0 is out of bounds for axis 0 with size 0`-  `I apologize for the confusion. It seems like there was a misunderstanding in my previous step. I attempted to use the encoded name (a numerical value) to fetch the original name from the preprocessed data, but this approach was not correct because the numerical value does not represent an index in the original data.`
	- Запит на додаткові дані
		- https://twitter.com/emollick/status/1654729461458190338/photo/2
- Навколишнє середовище
	- Випереджальне відновлення? "I'm sorry, but it seems there was a disruption in the code execution environment causing a reset."
		- "Given the repeated resets in the code execution state, I think the most efficient way forward is to write a self-contained script that does not rely on any variables from earlier in the session."
	- Динамічно імпортує модулі
	- **Катастрофічне відновлення та повторна спроба**: "Let's start from the beginning by extracting the data from the zip file again. I'll make sure to correctly specify the locations this time." https://chat.openai.com/share/770ab170-8fed-402f-850f-e6d7273e77cd
	- can you display this .png inline?
		- from IPython.display import Image # Display the generated flowchart Image(filename='/mnt/data/flowchart_enhanced.png')
		- <IPython.core.display.Image object>
	- KeyboardInterrupt: after long execution https://chat.openai.com/share/adc73608-4c80-497b-ad03-31de28bfa919
	- Обробка зображень з PIL: "Make the background of this image black"
	- Cv2 library for computer vision, py-tesseract for OCR
	

## Застарілі можливості попереднього перегляду досліджень



## Речі, які Інтерпретатор коду робить погано

- відображення таблиць генерується виключно LLM і повільно. потрібно перейти до компонента та вивести вихідний код через компонент
- досить часто з'являються повідомлення "стан виконання коду скинуто". https://chat.openai.com/share/adc73608-4c80-497b-ad03-31de28bfa919
- відновлення середовища погане: https://twitter.com/swyx/status/1677571294416756737?s=20
- він часто галюцинує залежності, які є надзвичайно поширеними
	- `NameError: name 'df' is not defined`
	- `NameError: name 'pd' is not defined`
	- `NameError: name 'zipfile' is not defined`
	- `NameError: name 'np' is not defined`
	- `NameError: name 'combinations' is not defined` I apologize for the oversight. It seems I forgot to import the `combinations` function from the `itertools` module`
	- `NameError: name 'ImageDraw' is not defined`. I apologize for the error, it appears I forgot to import the `ImageDraw` module from the `PIL` package. L
- немає доступу до Інтернету
	- To proceed, we would need the descriptions of each package. These can typically be obtained from the package's documentation or from PyPI (the Python Package Index). However, fetching data from the internet is not permitted in the current environment.
- it doesn't "fill in the blanks" from LLM knowledge - instruction to "guess the data you don't have" fails
- thinks it doesn't have folium... but it does
- render the folium map to an image and show the image
	- Please note that due to the limitations of my current environment, I'm unable to convert the HTML file to an image directly within this notebook. However, you can do this in a local Python environment using tools like `imgkit` or `selenium`.
- Unfortunately, without more data and given the constraints of this environment, it's not possible to perform a detailed spatial analysis of the crime data. For a complete analysis, I would recommend using a GIS (Geographic Information System) software or library (like `geopandas` in Python) and obtaining more detailed spatial data.
- кластеризація та іменування
- неможливо викликати openai API для вставлення тексту, немає трансформаторів і немає UMAP
	- 
