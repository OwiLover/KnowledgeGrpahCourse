## Лабораторные работы по "Валидация и тестирование систем ИИ"
Выполнили: <br>
Расковалова Алена, P4241 <br>
Строкова Анастасия, P4240

### Лабораторная работа 4
В рамках лабораторной работы было совершено знакомство с графовыми нейронными сетями. В GNN каждая вершина графа обновляется на основе её соседей, что позволяет модели учить представления вершин, учитывая их окружение. <br>
Выполнена следующая последовательность действий:
<li> Установка зависимостей и импорт необходимых пакетов (pykeen)
<li> Импорт выбранного датасета
<li> Получение тренировочных данных в виде троек сущность - отношение - сущность
<li> Обучение модели TransE, вывод результатов
<li> Вывод троек, получивших высший score
<br>

**Часть 1.Датасет Countries** <br>
[Код Countries](LR4_Countries.ipynbb) <br>
<img src="Countries_nlargest.PNG" width="1000" height="300"/> <br>
<br>

**Часть 2. Датасет PharmKG** <br>
[Код Pharm](LR4_PharmKG.ipynb) <br>
<img src="Pharm_nlargest.PNG" width="1000" height="300"/> <br>

В результате выполнения данной лабораторной работы мы освоили применение графовых нейронных сетей (GNNs) для анализа зависимостей в графовых структурах данных. Эмбеддинги, извлеченные с использованием GNN, позволяют представить вершины графа в векторной форме, сохраняя важную структурную информацию. <br>

Тестирование модели на новых данных и валидация для подбора гиперпараметров с использованием датасета Kinships дали возможность оценить обобщающую способность и оптимальность модели. Библиотека Pykeen значительно упростила взаимодействие с графовыми данными. <br>

Выбор модели TransE и использование датасета Countries и PharmKG позволили успешно решить задачу предсказания отношений в контексте родственных связей. Заданные эпохи обучения и валидации позволили оценить производительность модели. Результаты включают в себя метрики производительности, потери на тренировочных данных, а также выдачу модели на тестовом и валидационном наборах данных. Рассчитанные оценки для validation троек и выделение троек с наивысшим score обеспечивают полноценный анализ эффективности разработанной модели на датасете Countries и PharmKG. <br>

