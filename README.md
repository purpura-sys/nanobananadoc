Документация по использованию NanoBanana в Google Labs
https://labs.google/fx/tools/ﬂow/


1.	Создание проектов.
Для организации рабочего пространства проще создавать раздельные проекты.
Заходим на >>> https://labs.google/fx/tools/ﬂow/ и нажимаем [+ New Project] или заходим в уже имеющийся проект.
Проекты можно переименовывать для удобства.

 
2.	Написание промпта.
Для написания промпта можно использовать несколько вариантов.

Вариант №1 - Писать промпт самим.
Заходим в проект и пишем промпт в чатбоксе. Как правильно написать промпт можно узнать в google.com или у любой бесплатной нейросети. Если имеется готовый промпт – перемещаемся в пункт 3.

Вариант №2 - Писать промпт с помощью Grok AI (xAI).
Это метод двойного промптирования, в котором участвует любая сторонняя ИИ-модель, принимающая изображение и умеющая описать его текстом. Для неё используется написание промпта для описания уже готового изображения с последующим получением готового промпта, который можно использовать для создания своего оригинального изображения.

Для начала выбираем подходящее изображение на https://ru.pinterest.com/search

Копируем или сохраняем изображение и кидаем в чатбокс Grok >>> https://grok.com/ с промптом для полного описания изображения с разделением на модули и написания промпта для NanoBanana (на англ восприятие лучше):

Примеры промпта для описания изображения на английском и на русском:
 
Write a detailed prompt for generating an image in Nano Banana. Describe in minor details: pose; hairstyle; model's outfit; camera angle; photo style; background; background details; overall mood.
 
Напишите подробное задание по созданию изображения в Nano Banana. Опишите в мельчайших деталях: позу; прическу; одежду модели; ракурс камеры; стиль фотографии; фон; детали фона; общее настроение.
 
 
ВАЖНО правильно расписать задание по описанию изображения для правильного разделения пунктов описания по абзацам в готовом промпте. Это задаёт промпту модульность и облегчает дальнейшие дополнения и редактирования готового варианта промпта.

После выдачи готового промпта важно найти абзацы с описанием одежды или обуви и исправить их чтобы на модели была надета нужная нам обувь с наших фотографий обуви (перевести далее на русский если пишем промпт на русском):
Important: He wears footwear from attached images.
Или для женской обуви:
Important: She wears shoes from attached images; footwear looks smaller on model to match small and elegant woman's feet.
Для женских промптов можно прописывать размер стопы и примечание чтобы обувь выглядела меньше, например "размер стопы 4.5 UK". Так же можно исправить и другие абзацы по своим предпочтениям. Например, цвет волос, одежды, положение рук\ног.

 
Пример готового модульного промпта для женской обуви, в котором абзацы можно исправить по своим предпочтениям (важные места подчёркнуты):
(Перевести на русский если требуется)

Ultra-realistic high-end fashion studio photography of a beautiful young 6 feet tall woman in her mid-20s, her hair is shoulder-length, voluminous, wavy redhead with soft curtain bangs and natural movement, gently tousled by the breeze., ﬂawless skin, wearing large black rectangular sunglasses, seated
gracefully on a white geometric block against a seamless pure white backdrop.

Model’s breasts: full, rounded DD-cup breasts with a natural, perky shape. The model has smooth, perfect legs, her foot size is 4.5 UK. Her legs are elegantly crossed with the one leg over another, one foot slightly lifted and angled toward the camera.

Outfit: She is wearing a ﬁtted, short-sleeved, rust-red/burgundy ribbed knit cardigan with a deep V-neck and three ornate gold-tone heart-shaped buttons. She wears a black-and-white gingham checkered short-skirt with a button-front detail. A dark bracelet is visible on her left wrist.

Important: She wears shoes from attached images; footwear looks smaller on model to match small and elegant woman's feet.

Camera angle: low to medium-low perspective, three-quarter view, tightly framed from mid-thigh down to the feet, making footwear the absolute focal point while showing the full pose and elegant proportions.

Lighting: bright, soft high-key studio lighting with gentle diffused shadows that beautifully highlight the leather texture, skin.

Photoshoot style: high-end commercial fashion editorial, ultra-sharp focus on every texture (leather, skin, outﬁt fabric), realistic material rendering, clean minimalist composition, vibrant colors pop against the white background, professional studio quality.

Overall mood: clean sophisticated feminine lines, conﬁdent, feminine, modern and effortlessly chic — a bold yet elegant summer fashion statement with timeless appeal.

 
3.	Работа с NanoBanana.
Написанный детальный промпт с описанием внешнего вида модели из пункта 2. помещаем в 
чатбокс NanoBanana.

Так же помещаем туда изображения обуви, которая должна быть надета на модели, заранее указав в промпте, что обувь находится в прикрепленных изображениях.

 





Изменить настройки и запустить генерацию можно ниже (выбор соотношения сторон - 3:4, количество изображений - x4, модель для генерации - NanoBananaPro).

После создания изображения можно переиспользовать наш промпт, исправить его, добавить другие изображения с обувью. Навестись на изображение и нажать >>> Reuse prompt.

  
4.	Скачивание готовых изображений.

Можно выделить несколько изображений и скачать архивом (ПКМ >>> download).
Изображения скачаются в меньшем разрешении 1К >>> 896х1200 и меньшем размере самих файлов.
 
5.	Дополнительная организация рабочего пространства.
Чтобы не плодить беспорядок из добавленных изображений обуви - можно сохранять их в отдельные коллекции именуя их артикулом для дальнейшего удобного поиска.
ПКМ в свободно место вверху >>> Create Collection

ПКМ по созданной коллекции >>> Rename и указать нужный артикул.

6.	Ошибки соединения.

Из-за нестабильности ВПН соединения генерация может не сработать. Лечится сменой сервера ВПН и\или обновлением страницы. Нажав на овальную стрелку - можно повторно использовать промпт, на круглую повторить генерацию с ошибкой. 

Так же такое возможно на этапе сохранения изображения. Лечится сменой сервера ВПН или\и обновлением страницы.

 

C обновлениями внутри google может меняться внешний вид рабочего пространства Flow и взаимодействие с NanoBanana. За дополнительной информацией и уточнениями по такому случаю обращаться c вопросами в google.com или задать вопросы иным ИИ-моделям:
https://chat.deepseek.com/
https://chat.qwen.ai/
https://grok.com/



Заключение.
Помимо Условий использования Google и Политики конфиденциальности Google важно понимать, что любые действия с нейросетями ограничиваются только умением пользоваться собственной фантазией и сообразительностью.


