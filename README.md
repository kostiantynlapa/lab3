# Л3 — Лапа Костянтин, ТВ-61мп, варіант 8

Рішення з ціною помилки. На історії відмов розподільчого обладнання навчаються класифікатори, дані перевіряються на пастки (витік, зміщена вибірка, зсув у часі), а для кожного об'єкта з `test.csv` ухвалюється рішення — висилати бригаду чи ні — за порогом із вартостей помилок.

Вартості варіанта 8: виїзд 2750 грн, пропущена відмова 50000 грн, поріг рішення 0.055.

## Файли

- `lab3.ipynb` — ноутбук із виконаними кроками 1–9 та виводами
- `report.md` — відповіді на питання
- `submission.csv` — рішення для об'єктів test (`object_id`, `decision`)
- `requirements.txt` — залежності

## Запуск

```
python -m venv .venv
.venv\Scripts\activate       # Windows; на Linux/macOS: source .venv/bin/activate
pip install -r requirements.txt
jupyter nbconvert --to notebook --execute --inplace lab3.ipynb
```

Дані очікуються в `variants/8/` (`registry.csv`, `train.csv`, `test.csv`). Після виконання поряд з'являється `submission.csv`.
