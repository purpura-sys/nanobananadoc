# Документация по использованию NanoBanana в Google Labs

**Ссылка:** https://labs.google/fx/tools/flow/

---

## 1. Создание проектов

Для организации рабочего пространства проще создавать раздельные проекты.

1. Перейдите по ссылке: https://labs.google/fx/tools/flow/
2. Нажмите **[+ New Project]** или зайдите в уже имеющийся проект
3. Проекты можно переименовывать для удобства

---

## 2. Написание промпта

Для написания промпта можно использовать несколько вариантов.

### Вариант №1 — Писать промпт самим

1. Зайдите в проект
2. Напишите промпт в чатбоксе
3. Как правильно написать промпт, можно узнать в [google.com](https://google.com) или у любой бесплатной нейросети
4. Если имеется готовый промпт – переходите к пункту 3

### Вариант №2 — Писать промпт с помощью Grok AI (xAI)

Это метод **двойного промптирования**, в котором участвует любая сторонняя ИИ-модель, принимающая изображение и умеющая описать его текстом. Для неё используется написание промпта для описания уже готового изображения с последующим получением готового промпта, который можно использовать для создания своего оригинального изображения.

#### Инструкция:

1. Выберите подходящее изображение на https://ru.pinterest.com/search
2. Скопируйте или сохраните изображение
3. Отправьте его в чатбокс Grok: https://grok.com/ с промптом для полного описания изображения
   <img width="1361" height="679" alt="0 - поиск изображений" src="https://github.com/user-attachments/assets/b2b534d1-9fc5-4471-97e9-76c4c6ee18c1" />


#### Примеры промптов для описания изображения:

**На английском (рекомендуется):**
```
Write a detailed prompt for generating an image in Nano Banana. Describe in minor details: pose; hairstyle; model's outfit; camera angle; photo style; background; background details; overall mood.
```

**На русском:**
```
Напишите подробное задание по созданию изображения в Nano Banana. Опишите в мельчайших деталях: позу; прическу; одежду модели; ракурс камеры; стиль фотографии; фон; детали фона; общее настроение.
```

> **ВАЖНО:** Правильно распишите задание по описанию изображения для правильного разделения пунктов описания по абзацам в готовом промпте. Это задаёт промпту модульность и облегчает дальнейшие дополнения и редактирования готового варианта промпта.

#### Редактирование промпта

После выдачи готового промпта важно найти абзацы с описанием одежды или обуви и исправить их, чтобы на модели была надета нужная вам обувь с ваших фотографий.

**Добавьте одну из фраз:**

- Для мужской обуви:
  ```
  Important: He wears footwear from attached images.
  ```

- Для женской обуви:
  ```
  Important: She wears shoes from attached images; footwear looks smaller on model to match small and elegant woman's feet.
  ```

> **Совет:** Для женских промптов можно прописывать размер стопы и примечание, чтобы обувь выглядела меньше, например *"размер стопы 4.5 UK"*.

Также можно исправить другие абзацы по своим предпочтениям: цвет волос, одежды, положение рук/ног.

#### Пример готового модульного промпта для женской обуви:

```
Ultra-realistic high-end fashion studio photography of a beautiful young 6 feet tall woman in her mid-20s, her hair is shoulder-length, voluminous, wavy redhead with soft curtain bangs and natural movement, gently tousled by the breeze., ﬂawless skin, wearing large black rectangular sunglasses, seated
gracefully on a white geometric block against a seamless pure white backdrop.

Model’s breasts: full, rounded DD-cup breasts with a natural, perky shape. The model has smooth, perfect legs, her foot size is 4.5 UK. Her legs are elegantly crossed with the one leg over another, one foot slightly lifted and angled toward the camera.

Outfit: She is wearing a ﬁtted, short-sleeved, rust-red/burgundy ribbed knit cardigan with a deep V-neck and three ornate gold-tone heart-shaped buttons. She wears a black-and-white gingham checkered short-skirt with a button-front detail. A dark bracelet is visible on her left wrist.

Important: She wears shoes from attached images; footwear looks smaller on model to match small and elegant woman's feet.

Camera angle: low to medium-low perspective, three-quarter view, tightly framed from mid-thigh down to the feet, making footwear the absolute focal point while showing the full pose and elegant proportions.

Lighting: bright, soft high-key studio lighting with gentle diffused shadows that beautifully highlight the leather texture, skin.

Photoshoot style: high-end commercial fashion editorial, ultra-sharp focus on every texture (leather, skin, outﬁt fabric), realistic material rendering, clean minimalist composition, vibrant colors pop against the white background, professional studio quality.

Overall mood: clean sophisticated feminine lines, conﬁdent, feminine, modern and effortlessly chic — a bold yet elegant summer fashion statement with timeless appeal.
```

---

## 3. Работа с NanoBanana

1. Написанный детальный промпт с описанием внешнего вида модели из пункта 2 поместите в чатбокс NanoBanana
2. Добавьте изображения обуви, которая должна быть надета на модели, заранее указав в промпте, что обувь находится в прикрепленных изображениях
3. Измените настройки и запустите генерацию:
   - **Соотношение сторон:** 3:4
   - **Количество изображений:** x4
   - **Модель для генерации:** NanoBananaPro

### Повторное использование промпта

После создания изображения можно переиспользовать промпт, исправить его, добавить другие изображения с обувью:

1. Наведите на изображение
2. Нажмите **>>> Reuse prompt**

---

## 4. Скачивание готовых изображений

- Можно выделить несколько изображений и скачать архивом: **ПКМ → Download**
- Изображения скачаются в меньшем разрешении **1K (896×1200)** и меньшем размере файлов

---

## 5. Дополнительная организация рабочего пространства

Чтобы не создавать беспорядок из добавленных изображений обуви, можно сохранять их в отдельные коллекции, именуя их артикулом для дальнейшего удобного поиска.

### Создание коллекции:

1. **ПКМ** в свободное место вверху
2. Выберите **Create Collection**

### Переименование коллекции:

1. **ПКМ** по созданной коллекции
2. Выберите **Rename**
3. Укажите нужный артикул

---

## 6. Ошибки соединения

Из-за нестабильности VPN-соединения генерация может не сработать.

### Решение:

- Смените сервер VPN
- Обновите страницу
- Нажмите на **овальную стрелку** — можно повторно использовать промпт
- Нажмите на **круглую стрелку** — повторить генерацию с ошибкой

> **Примечание:** Такое возможно и на этапе сохранения изображения. Лечится сменой сервера VPN или обновлением страницы.

---

## Дополнительные ресурсы

С обновлениями внутри Google может меняться внешний вид рабочего пространства Flow и взаимодействие с NanoBanana. За дополнительной информацией и уточнениями обращайтесь:

- [google.com](https://google.com)
- [DeepSeek Chat](https://chat.deepseek.com/)
- [Qwen Chat](https://chat.qwen.ai/)
- [Grok](https://grok.com/)

---

## Заключение

Помимо [Условий использования Google и Политики конфиденциальности Google](https://policies.google.com/terms?hl=ru), важно понимать, что любые действия с нейросетями ограничиваются только умением пользоваться собственной фантазией и сообразительностью.
