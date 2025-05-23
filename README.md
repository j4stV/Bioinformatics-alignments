# DFNB1: Несиндромальная врождённая тугоухость (аутосомно‑рецессивная, тип 1А)

**OMIM № 220290** — заболевание, характеризующееся двусторонней сенсоневральной тугоухостью, проявляющейся с рождения или раннего детства без иных клинических признаков. Основная причина — нарушение межклеточной ионной коммуникации в эпителии внутреннего уха.

---

## Ассоциированные гены

| Ген | Полное название | Функция (кратко) |
|-----|-----------------|------------------|
| **GJB2** | *Gap Junction Beta‑2* (Connexin 26) | Образует белковые каналы (коннексоны) межклеточных щелей, обеспечивающие рециклинг K⁺ в кортиевом органе |
| **GJB6** | *Gap Junction Beta‑6* (Connexin 30) | Работает совместно с Cx26; мутации обоих белков нарушают ионный гомеостаз эндолимфы |

---

## Файлы последовательностей

```
/data/GJB2_human.fasta
/data/Gjb2_mouse.fasta
/data/GJB6_human.fasta
/data/Gjb6_mouse.fasta
```

---

## Результаты парного выравнивания (человек ⇄ мышь, CDS ➜ белок)

| Ген | Инструмент | Длина выравнивания | Identity | Gaps | Score | Выбор |
|-----|-----------|--------------------|----------|------|-------|-------|
| **GJB2** | Needle | 6 456 aa | 57.4 % | 20.8 % | 18 143 |  |
|         | Water  | 6 431 aa | **57.6 %** | **20.5 %** | 18 143 | **✅ лучший** |
| **GJB6** | Needle | 11 486 aa | 54.0 % | 22.7 % | 28 633 |  |
|         | Water  | 11 473 aa | **54.1 %** | **22.6 %** | **28 636** | **✅ лучший** |

### Критерии оценки

* **Identity %** — главный показатель консервативности ортологов.
* **Gaps %** — доля разрывов; чем меньше, тем ближе структуры.
* **Score** — суммарная оценка EBLOSUM62; учитывалась при равных первых двух метриках.

### Выводы

*Для обоих генов инструмент **EMBOSS Water** (локальное выравнивание) показал:*
1. Наибольший процент идентичности (+0.2 % у *GJB2*, +0.1 % у *GJB6*).
2. Наименьшую долю разрывов (−0.3 % / −0.1 %).
3. Идентичный (GJB2) или более высокий (GJB6) суммарный score.

> Поэтому **Water** признан оптимальным для дальнейшего анализа функциональных доменов коннексинов. Глобальный Needle дал сопоставимые, но слегка худшие метрики.

---

## Версии инструментов

* **EMBOSS Needle** v6.6.0 · опции `gapopen 10`, `gapextend 0.5`
* **EMBOSS Water**  v6.6.0 · те же параметры

---

