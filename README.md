# Маркетинговый анализ e-commerce

**Цель:** анализ влияния поведенческих метрик на конверсию (n=4.16 млн сессий)

## 📊 Данные
- **Источник:** 2019-Oct.csv (5.28 GB)
- **Подготовка:**
  
5.3 GB сырых событий → Polars (lazy + streaming)
  
Фильтр: 14 дней + view/cart/purchase + price > 0
 
Парсинг: event_time → hour, weekday, is_weekend
 
Агрегация по user_session:

Дубли: 173 убрано (0.004%) — GA-шум

Pandas: 320 MB → sessions_14days.csv

- **Метрики:** views, made_purchase, день недели, категории, время

### 1. [Предобработка](https://colab.research.google.com/drive/1exnIPxvRnjBP5eziwJDXq0DD3lW92D6T?authuser=1#scrollTo=jw788kZtGjUD)) ✅

#### 🔧 Что сделано:






## 🎯 План анализа (7 гипотез)
