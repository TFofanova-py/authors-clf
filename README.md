Тема - определение авторства текста

Исполнитель - Фофанова Татьяна

Куратор - Сергей Аксёнов

Задача классификации текстов, датасет - произведения русской, советской, российской литературы IXX - XXI веков. 

Данные. На данный момент собран датасет из 19 авторов, тексты в формате epub, каждое произведение разбито на главы. Предполагается брать отрывки текстов из глав примерно по 1500 знаков, при этом вырезать отрывки можно случайно, увеличив таким образом обучающую выборку. Данные размечаются автоматически, т.к. произведения авторов лежат в разных директориях.

На данный момент собран датасет и реализован DataLoader, который итеративно подает случайно вырезанные отрывки текста.

Что дальше:
- EDA
- предобработка текста, можно попробовать токенизацию BPE
- в качестве baseline можно использовать Word2Vec для эмбеддингов, эмбеддинг текста вычислить как взвешенную по idf сумму эмбеддингов, затем построить логистическую регрессию.
- потом можно использовать transformers

Еще хочется попробовать style transfer - генерировать текст в стиле какого-то автора.
