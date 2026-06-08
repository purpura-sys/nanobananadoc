# Документация по использованию NanoBanana в Google Labs

**Ссылка:** https://labs.google/fx/tools/flow/

---

## 1. Создание проектов

Для организации рабочего пространства проще создавать раздельные проекты.

* Перейдите по ссылке: https://labs.google/fx/tools/flow/
* Нажмите **[+ New Project]** или зайдите в уже имеющийся проект
* Проекты можно переименовывать для удобства
<img width="1528" height="991" alt="1 - Создание проекта" src="https://github.com/user-attachments/assets/203f0b97-e367-4d46-8909-9a65e48adfc1" />


---

## 2. Написание промпта

Для написания промпта можно использовать несколько вариантов.

### Вариант №1 — Писать промпт самим

* Зайдите в проект
* Напишите промпт в чатбоксе
* Как правильно написать промпт, можно узнать в [google.com](https://google.com) или у любой бесплатной нейросети
* Если имеется готовый промпт – переходите к пункту **3.**

### Вариант №2 — Писать промпт с помощью Grok AI (xAI)

Это метод **двойного промптирования**, в котором участвует любая сторонняя ИИ-модель, принимающая изображение и умеющая описать его текстом. Для неё используется написание промпта для описания уже готового изображения с последующим получением готового промпта, который можно использовать для создания своего оригинального изображения.

#### Инструкция:

* Выберите подходящее изображение на https://ru.pinterest.com/search
<img width="1361" height="679" alt="0 - поиск изображений" src="https://github.com/user-attachments/assets/b2b534d1-9fc5-4471-97e9-76c4c6ee18c1" />

* Скопируйте или сохраните изображение
* Отправьте его в чатбокс Grok: https://grok.com/ с промптом для полного описания изображения


#### Примеры промптов для описания изображения:

**На английском (рекомендуется):**
```
Write a detailed prompt for generating an image in Nano Banana.
Describe in minor details: pose; hairstyle; model's outfit; camera angle; photo style; background; background details; overall mood.
```

**На русском:**
```
Напишите подробное задание по созданию изображения в Nano Banana.
Опишите в мельчайших деталях: позу; прическу; одежду модели; ракурс камеры; стиль фотографии; фон; детали фона; общее настроение.
```
<img width="1517" height="914" alt="1 3 - чатбокс в Грок" src="https://github.com/user-attachments/assets/733af530-3031-4316-ab07-62245891bc54" />



> **ВАЖНО** **точно** распиcать задание по описанию изображения для правильного разделения пунктов описания по абзацам в готовом промпте. Это задаёт промпту модульность и облегчает дальнейшие дополнения и редактирования готового варианта промпта.

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

* Написанный детальный промпт с описанием внешнего вида модели из пункта 2 поместите в чатбокс NanoBanana
<img width="1515" height="912" alt="1 4 чатбокс НаноБанана" src="https://github.com/user-attachments/assets/018280a5-4b99-4011-80b6-22b0013257cb" />

* Добавьте изображения (референсы) обуви, которая должна быть надета на модели, заранее указав в промпте, что обувь находится в прикрепленных изображениях
<img width="1552" height="930" alt="2 - Добавить референсы перетаскиванием" src="https://github.com/user-attachments/assets/16ca57bf-478d-4600-a2aa-dee1d4133448" />


* Измените настройки и запустите генерацию:
   - **Соотношение сторон:** 3:4
   - **Количество изображений:** x4
   - **Модель для генерации:** NanoBananaPro
<img width="1548" height="923" alt="3 - Изм настройки, запустить ген" src="https://github.com/user-attachments/assets/26510893-c6b3-4860-afe5-d2d6af3d302f" />


### Повторное использование промпта

После создания изображения можно переиспользовать промпт, исправить его, добавить другие изображения с обувью:

* Наведите на изображение
* Нажмите **>>> Reuse prompt**
<img width="1553" height="919" alt="1 5 - Реюз промпта" src="https://github.com/user-attachments/assets/e7b16f2a-8b12-4cc8-b507-a4a119cc2082" />


---

## 4. Скачивание готовых изображений
* ПКМ по изображению или на три точки сверху.
<img width="1551" height="965" alt="4 - Скачать" src="https://github.com/user-attachments/assets/270d9860-cf91-4bfb-a78c-3ef6e6b306d8" />


- Можно выделить несколько изображений и скачать архивом: **ПКМ → Download**
- Изображения скачаются в меньшем разрешении **1K (896×1200)** и меньшем размере файлов
<img width="1512" height="930" alt="4 5 - Выделение объектов" src="https://github.com/user-attachments/assets/5554a9d7-6099-4868-93d9-1ab8635f13ff" />


---

## 5. Дополнительная организация рабочего пространства

Чтобы не создавать беспорядок из добавленных изображений обуви, можно сохранять их в отдельные коллекции, именуя их артикулом для дальнейшего удобного поиска.

### Создание коллекции:

* **ПКМ** в свободное место вверху
* Выберите **Create Collection**

Это можно сделать при выделении нужных объектов или простым перетаскиванием объектов в коллекцию.
<img width="1523" height="934" alt="4 6 - Создание коллекции" src="https://github.com/user-attachments/assets/a9c8e96b-9fea-4970-bb14-a230d26ea311" />


### Переименование коллекции:

* **ПКМ** по созданной коллекции
* Выберите **Rename**
* Укажите нужный артикул
<img width="1520" height="941" alt="4 7 - переименование коллекции" src="https://github.com/user-attachments/assets/772fea28-fa15-4249-886b-82cd731ec7c9" />


---
Для быстрого поиска изображений можно переименовать их. Для массового преименовывания любых файлов можно использовать программу Bulk Rename Utility
<img width="1309" height="90" alt="Снимок экрана (35) — копия" src="https://github.com/user-attachments/assets/71ef18c8-48cd-41ef-bf91-e1c808ece39b" />


* Выбираем нужную папку с файлами
* Обновляем список если уже находимся в нужной папке или после скачивания в неё файлов
<img width="1309" height="1080" alt="Снимок экрана (35)" src="https://github.com/user-attachments/assets/eb6b58e5-1d8a-4c5d-8694-248291a9e41d" />


* Для изображений ставится префикс с их артикулом
* Выделяем нужные, находим Prefix и пишем артикул
* Нажать Rename для переименовывания
<img width="1309" height="1043" alt="Снимок экрана (36)" src="https://github.com/user-attachments/assets/0d7dcbf1-30ba-4549-bce9-4cde2e4bd29a" />


## 6. Ошибки соединения

Из-за нестабильности VPN-соединения генерация может не сработать.

### Решение:

- Смените сервер VPN
- Обновите страницу
- Нажмите на **овальную стрелку** — можно повторно использовать промпт или сохранить его т.к. после обновления страницы он пропадет вместе с сообщением ошибки.
- Нажмите на **круглую стрелку** — повторить генерацию с ошибкой
<img width="1515" height="917" alt="8 - Возникающие ошибки" src="https://github.com/user-attachments/assets/e89f9069-6fd6-45ad-a497-ba73b7eb2df7" />


> **Примечание:** Такое возможно и на этапе сохранения изображения. Лечится сменой сервера VPN или обновлением страницы.
<img width="1520" height="930" alt="9 - Ошибка при сохранении" src="https://github.com/user-attachments/assets/25afeeec-cdf1-4b9c-af23-c22d05969f8e" />

---

## Обновления и Дополнительные ресурсы

С обновлениями внутри Google может меняться внешний вид рабочего пространства Flow и взаимодействие с NanoBanana. За дополнительной информацией и уточнениями обращайтесь:

- [Google](https://google.com)
- [DeepSeek AI](https://chat.deepseek.com/)
- [Qwen AI](https://chat.qwen.ai/)
- [Grok AI (xAI)](https://grok.com/)
- [Help Center Google Flow](https://support.google.com/flow#topic=16908930)

---

## Заключение

Помимо [Условий использования Google и Политики конфиденциальности Google](https://policies.google.com/terms?hl=ru), важно понимать, что любые действия с нейросетями ограничиваются **только** умением пользоваться собственной фантазией, сообразительностью и логикой.
