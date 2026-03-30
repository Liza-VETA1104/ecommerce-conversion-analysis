# Маркетинговый анализ e-commerce

**Цель:** анализ влияния поведенческих метрик на конверсию (n=4.16 млн сессий)

## 📊 Данные
- **Источник:** 2019-Oct.csv (5.28 GB)
- **Подготовка:** 14 дней сессий → sessions_14days.csv
- **Метрики:** views, made_purchase, день недели, категории, время

- | Этап | Действие | Результат |
|------|----------|-----------|
| **1** | `pl.scan_csv(1.3GB)` | Lazy загрузка |
| **2** | `filter(14 дней)` | 18M → 4.16M |
| **3** | `group_by(user_session)` | Views + purchases |
| **4** | `drop_duplicates()` | -173 дубля |
| **5** | `to_pandas()` | 320 MB готово |

https://colab.research.google.com/drive/1exnIPxvRnjBP5eziwJDXq0DD3lW92D6T?authuser=1#scrollTo=jw788kZtGjUD

## 🎯 План анализа (7 гипотез)
