# RuSimpleSentEval (RSSE)

## Описание задачи
Задача упрощения тестов  (text simplification) предполагает несколько постановок, из которых мы выбираем самую популярную: упрощение на уровне предложений. В такой постановке задача заключается в том, чтобы из сложного предложения получить упрощенное. 
Критерии сложности предложения включают в себя наличие сложных грамматических конструкций, в том числе, причастных и деепричастных оборотов, подчиненных предложений, наличие редких и неоднозначных слов и т.д.

Большая часть вычислительных моделей упрощения текста используют нейросетевые seq2seq модели, которые обучаются по параллельным данным, то есть, по парам сложное предложение – простое предложение. Организаторы составили набор таких параллельных предложений и предоставят их участникам соревнования для обучения моделей. Поскольку для русского языка подобного набора данных не существовало, он был создан специально для соревнования. Основой обучающего набора данных послужили переведенные с английского материалы Википедии (English Wikipedia) и упрощенной Википедии (Simple English Wikipedia), подвергнутые дополнительной фильтрации. Вторая часть набора данных, которая будет использоваться для оценки и тестирования, составлена на краудсорсинговой платформе.

В качестве метрики качества будет использована мера SARI (System output Against References and against the Input sentence). 

## Таймлайн соревнования
* **Вы находитесь здесь**
* **15.02.2021-20.02.2021** -- публикация данных 
* **15.02.2021--11.03.2021** -- [первая фаза соревнования](https://competitions.codalab.org/competitions/29037#phases) (отправка результатов для public test).
* **12.03.2021--14.03.2021**  -- [вторая фаза соревнования](https://competitions.codalab.org/competitions/29037#phases) (отправка результатов для private test).
* **15.03.2021** -- официальное завершение соревнования и подведение итогов.
* **25.03.2021** -- дедлайн по подачи статей по результатам соревнования.

## Данные

* Автоматически переведенный на русский  корпус WikiLarge [1]. Данные доступны по [ссылке](https://drive.google.com/drive/folders/1jfij3KuiRbO_XoLiquSBP2mZafzPhrsL). 
* Собранный организаторами на краудсорсинговой платформе корпус. Dev датасет (пары сложное –  простое предложение) доступен по [ссылке](https://github.com/dialogue-evaluation/RuSimpleSentEval/blob/main/dev_sents.csv). Сложные предложения из public test для первой фазы соревнования доступны по [ссылке](public_test_only.csv). 

1. Zhang, X. and Lapata, M., 2017, September. Sentence Simplification with Deep Reinforcement Learning. In Proceedings of the 2017 Conference on Empirical Methods in Natural Language Processing (pp. 584-594).


## Организаторы:
* Екатерина Артемова, ВШЭ, HUAWEI
* Валентин Малых, КФУ, HUAWEI
* Иван Смуров, ABBYY, МФТИ
* Елена Тутубалина, КФУ, ВШЭ

* [**Телеграм-чат соревнования**](https://t.me/rsse2021)
