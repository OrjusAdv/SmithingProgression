# Документация по отрывку кода, отвечающюю за развитие игроков.

## **Секция: starting_perks**

Секция `starting_perks` определяет начальные модификаторы опыта для различных типов материалов. Значения отрицательных множителей уменьшают количество получаемого опыта.



### **Параметры:**

- **`smithing_stoneexpmultiplier_add: -0.5`**  

  - Уменьшает получаемый опыт за обработку камня (stone) на 50%.  

  - Например, если базовое количество опыта за камень равно 10, игрок получит 5.  



- **`smithing_chainexpmultiplier_add: -0.5`**  

  - Уменьшает получаемый опыт за обработку цепей (chain) на 50%.  



- **`smithing_goldexpmultiplier_add: -0.75`**  

  - Уменьшает опыт за обработку золота (gold) на 75%.  



- **`smithing_ironexpmultiplier_add: -0.75`**  

  - Уменьшает опыт за обработку железа (iron) на 75%.  



- **`smithing_diamondexpmultiplier_add: -0.90`**  

  - Уменьшает опыт за обработку алмазов (diamond) на 90%.  



- **`smithing_netheriteexpmultiplier_add: -1`**  

  - Полностью убирает получение опыта за обработку незерита (netherite).  



---



## **Секция: experience**

Секция `experience` определяет формулу опыта, максимальный уровень и модификаторы опыта, зависящие от повреждений предметов.



### **Параметры:**

- **`exp_level_curve`**  

  - Формула для расчёта необходимого опыта для достижения определённого уровня.  

  - Формат: `'(%level% + 75 * 2^(%level%/7.6)) + 300'`.  

  - Пример: на уровне 1 потребуется `(1 + 75 * 2^(1/7.6)) + 300` опыта.



- **`max_level: 100`**  

  - Устанавливает максимальный уровень навыка кузнечного дела (Smithing).



- **`durability_tools_exp_multiplier_stack: 0.01`**  

  - Увеличивает опыт за единицу урона инструменту на 1% за каждый "стек" (stack).  



- **`durability_tools_exp_multiplier_maximum: 1000`**  

  - Устанавливает максимум стеков для инструментов. Максимальное увеличение опыта: 1000%.  



- **`durability_armors_exp_multiplier_stack: 0.005`**  

  - Увеличивает опыт за единицу урона броне на 0.5% за стек.  



- **`durability_armors_exp_multiplier_maximum: 200`**  

  - Устанавливает максимум стеков для брони. Максимальное увеличение опыта: 100%.  



- **`durability_chunk_limit: 50`**  

  - Ограничивает количество стеков опыта за урон предметов в одном чанке.  

  - Если лимит превышен, игрок не получает дополнительные стеки.  



---


"""


