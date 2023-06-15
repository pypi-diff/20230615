# Comparing `tmp/yeref-0.1.96.tar.gz` & `tmp/yeref-0.1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.96.tar", last modified: Wed Jun 14 09:34:39 2023, max compression
+gzip compressed data, was "yeref-0.1.98.tar", last modified: Thu Jun 15 11:45:40 2023, max compression
```

## Comparing `yeref-0.1.96.tar` & `yeref-0.1.98.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-14 09:34:39.390853 yeref-0.1.96/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-14 09:34:39.391090 yeref-0.1.96/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-14 09:34:39.392052 yeref-0.1.96/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-14 09:34:35.000000 yeref-0.1.96/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-14 09:34:39.383451 yeref-0.1.96/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.96/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   551845 2023-06-14 09:17:40.000000 yeref-0.1.96/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   210936 2023-06-14 09:33:51.000000 yeref-0.1.96/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-14 09:34:39.390151 yeref-0.1.96/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-14 09:34:39.000000 yeref-0.1.96/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-14 09:34:39.000000 yeref-0.1.96/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-14 09:34:39.000000 yeref-0.1.96/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-14 09:34:39.000000 yeref-0.1.96/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-15 11:45:40.412498 yeref-0.1.98/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-15 11:45:40.412825 yeref-0.1.98/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-15 11:45:40.414042 yeref-0.1.98/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-15 11:44:55.000000 yeref-0.1.98/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-15 11:45:40.405449 yeref-0.1.98/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.98/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   556618 2023-06-15 11:44:29.000000 yeref-0.1.98/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   210936 2023-06-14 09:33:51.000000 yeref-0.1.98/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-15 11:45:40.411787 yeref-0.1.98/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-15 11:45:40.000000 yeref-0.1.98/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-15 11:45:40.000000 yeref-0.1.98/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-15 11:45:40.000000 yeref-0.1.98/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-15 11:45:40.000000 yeref-0.1.98/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.96/setup.py` & `yeref-0.1.98/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.96',
+      version='0.1.98',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -43,12 +43,12 @@
 
 # twine upload dist/*
 # freey.sitner.ya
 # cejwez-nosgin-vaVfe7
 
 # python3 -m pip install --upgrade yeref
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.96-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.97-py3-none-any.whl
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.96/yeref/l_.py` & `yeref-0.1.98/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,16 +133,24 @@
     'ru': "👩🏽‍💻 <b>Необходимо</b> оформить подписку!",
     'en': "🔔 You need to ⚙️Customize at least one post",
     'es': "🔔 Necesitas ⚙️Personalizar al menos una publicación",
     'fr': "🔔 Vous devez ⚙️Personnaliser au moins une publication",
     'zh': "🔔 你需要⚙️自定义至少一个帖子",
     'ar': "🔔 أنت بحاجة إلى تخصيص منشور واحد على الأقل",
 }
+l_subscribe_spoiler = {
+    'ru': "оформи подписку",
+    'en': "оформи подписку",
+    'es': "🔔 Necesitas ⚙️Personalizar al menos una publicación",
+    'fr': "🔔 Vous devez ⚙️Personnaliser au moins une publication",
+    'zh': "🔔 你需要⚙️自定义至少一个帖子",
+    'ar': "🔔 أنت بحاجة إلى تخصيص منشور واحد على الأقل",
+}
 l_subscribe_channel_for_post = {
-    'ru': "👩🏽‍💻 <b>Подпишись</b> на @{0}, чтобы создавать посты без ограничений",
+    'ru': "👩🏽‍💻 <b>Подпишись</b> на @{0}, чтобы снять ограничения",
     'en': "🔔 You need to ⚙️Customize at least one post",
     'es': "🔔 Necesitas ⚙️Personalizar al menos una publicación",
     'fr': "🔔 Vous devez ⚙️Personnaliser au moins une publication",
     'zh': "🔔 你需要⚙️自定义至少一个帖子",
     'ar': "🔔 أنت بحاجة إلى تخصيص منشور واحد على الأقل",
 }
 
@@ -663,15 +671,15 @@
     'en': "👩🏽‍💻 <b>Choose</b> recipient",
     'es': "👩🏽‍💻 <b>Elegir</b> destinatario",
     'fr': "👩🏽‍💻 <b>Choisissez</b> le destinataire",
     'zh': "👩🏽‍💻<b>选择</b>收件人",
     'ar': "👩🏽‍💻 <b>اختر</b> المستلم",
 }
 l_enter = {
-    'ru': "👩🏽‍💻 <b>Введи</b> Ids получателей через пробельные или разделительные символы",
+    'ru': "👩🏽‍💻 <b>Введи</b> Ids получателей через <i>пробельные или разделительные</i> символы",
     'en': "👩🏽‍💻 <b>Enter</b> recipient Ids separated by spaces or separator characters",
     'es': "👩🏽‍💻 <b>Ingrese</b> las identificaciones de los destinatarios separadas por espacios o caracteres separadores",
     'fr': "👩🏽‍💻 <b>Entrez</b> les identifiants des destinataires séparés par des espaces ou des caractères de séparation",
     'zh': "👩🏽‍💻<b>输入</b>以空格或分隔符分隔的收件人 ID",
     'ar': "👩🏽‍💻 <b>أدخل</b> معرفات المستلمين مفصولة بمسافات أو أحرف فاصلة",
 }
 l_post_time_zone = {
@@ -996,2005 +1004,1339 @@
     'fr': "postes vacants/concours",
     'zh': "职位空缺/竞争",
     'ar': "الشواغر / المسابقات",
 }
 # endregion
 
 
-# region FereyDemoBot
-l_demo_btn1 = {
-    'ru': "⛰️ Проекты",
-    'en': "⛰️ Projects",
-    'es': "⛰️ Proyectos",
-    'fr': "⛰️ Projets",
-    'zh': "⛰️ 项目",
-    'ar': "⛰️ المشاريع",
+# region FereyBotBot
+l_bot_btn1 = {
+    'ru': "⛰ Боты",
+    'en': "⛰ Bots",
+    'es': "⛰ Bots",
+    'fr': "⛰ Bots",
+    'zh': "⛰ 靴子",
+    'ar': "⛰ أحذية",
 }
-l_demo_btn2 = {
+l_bot_btn2 = {
     'ru': "🌬 Подписка",
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
-l_demo_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> проекта <b>Ferey</b>:\n\n▪️<b>информация</b> обо всех проектах\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to <i>the landing bot</i> of the <b>Ferey</b> проекта :\n\n▪️ <b>information</b> about all projects\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del проекта <b>Ferey</b> :\n\n▪️ <b>información</b> sobre todos los proyectos\n\n❗️ también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du проекта <b>Ferey</b> :\n\n▪️ <b>informations</b> sur tous les projets\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎来到<b>Ferey</b> проекта的<i>落地机器人</i>：\n\n▪️ 所有项目的<b>信息</b>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص проекта <b>Ferey</b> :\n\n▪️ <b>معلومات</b> حول جميع المشاريع\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
+l_bot_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> автоматизации <b>Telegram</b>-ботов:\n\n▪️авто-постинг и <b>авто-перевод</b>\n▪️<b>авто-ответы</b> и оповещения\n▪️нейросети: графика и текст бота\n▪️интеграции и платежи\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to the <b>Telegram</b> bot автоматизации <i>landing bot</i> :\n\n▪️auto-posting and <b>auto-translation</b>\n▪️ <b>auto-replies</b> and notifications\n▪️integrations and payments\n▪️users and administrators\n\n❗️You can also order the development of a chatbot in our ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> автоматизации de bots <b>de Telegram</b> :\n\n▪️auto-publicación y <b>auto-traducción</b>\n▪️auto <b>-respuestas</b> y notificaciones\n▪️integraciones y pagos\n▪️usuarios y administradores\n\n❗️también puedes encargar el desarrollo de un chatbot en nuestro ferey studio",
+    'fr': "🌱 {0}, bienvenue dans le <i>bot d&#x27;atterrissage</i> автоматизации du bot <b>Telegram</b> :\n\n▪️publication et <b>traduction automatiques</b>\n▪️ <b>réponses et notifications automatiques</b>\n▪️intégrations et paiements\n▪️utilisateurs et administrateurs\n\n❗️Vous pouvez également commander le développement d'un chatbot dans notre studio ferey",
+    'zh': "🌱 {0}，欢迎使用<b>Telegram</b>机器人автоматизации<i>登陆机器人</i>：\n\n▪️自动发布和<b>自动翻译</b>\n▪️<b>自动回复</b>和通知\n▪️集成和支付\n▪️用户和管理员\n\n❗️您也可以在我们的ferey工作室订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوط</i> автоматизации لروبوت <b>Telegram</b> :\n\n▪️ النشر التلقائي <b>والترجمة التلقائية</b>\n▪️ <b>الردود التلقائية</b> والإشعارات\n▪️ عمليات الدمج والمدفوعات\nالمستخدمون والمسؤولون\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو ferey الخاص بنا",
 }
-l_subscribe_demo = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
+l_subscribe_bot = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️авто-перевод\n(<i>в том числе, текста кнопок</i>)\n▪️авто-ответ\n(<i>chatgpt видит блоки бота</i>)\n▪️приоритетная поддержка\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
     'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 
-l_kind_1 = {
-    'ru': "<b>👩🏽‍💻@FereyDemoBot</b>\n\n<b>Демо</b> бот всех проектов",
-    'en': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\nDemo bot of all projects",
-    'es': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\nBot de demostración de todos los proyectos",
-    'fr': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\nDemo bot de tous les projets",
-    'zh': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\n所有项目的演示机器人",
-    'ar': "<b>👩🏽‍💻FereyDemoBot</b>\n\nروبوت تجريبي <b>@FereyDemoBot</b> المشاريع",
-}
-l_kind_2 = {
-    'ru': "<b>👩🏽‍💻@FereyBotBot</b>\n\n<b>Конструктор</b> ботов:\n▪️авто-генерация бота\n▪️авто-генерация контента (open-ai)\n▪️авто-бан/перевод/рассылка",
-    'en': "<b>👩🏽‍💻</b> <b>@FereyBotBot</b>\n\nBot Builder:\n▪️auto-generate bot\n▪️auto-generate content (open-ai)\n▪️auto-ban/auto-translate",
-    'es': "<b>👩🏽‍💻</b> <b>@FereyBotBot</b>\n\nGenerador de bots:\n▪️generación automática de bot\n▪️generación automática de contenido (open-ai)\n▪️prohibición automática/traducción automática",
-    'fr': "<b>👩🏽‍💻</b> <b>@FereyBotBot</b>\n\nBot Builder :\n▪️auto-génère le bot\n▪️auto-génère le contenu (open-ai)\n▪️auto-ban/auto-translate",
-    'zh': "<b>👩🏽‍💻</b> <b>@FereyBotBot</b>\n\nBot Builder：\n▪️自动生成机器人\n▪️自动生成内容（open-ai）\n▪️自动禁止/自动翻译",
-    'ar': "<b>👩🏽‍💻FereyBotBot</b>\n\nBot Builder:\n▪️ إنشاء روبوت تلقائيًا <b>@FereyBotBot</b> n▪️ إنشاء محتوى تلقائيًا (فتح ai)\n▪️ حظر تلقائي / ترجمة آلية",
-}
-l_kind_3 = {
-    'ru': "<b>👩🏽‍💻@FereyChannelBot</b>\n\n<b>Администрирование</b> каналов:\n▪️авто-постинг\n▪️авто-декор",
-    'en': "<b>👩🏽‍💻</b> <b>@FereyChannelBot</b>\n\nChannel admin:\n▪️auto-posting\n▪️auto-decor",
-    'es': "<b>👩🏽‍💻</b> <b>@FereyChannelBot</b>\n\nAdministrador del canal:\n▪️publicación automática\n▪️decoración automática",
-    'fr': "<b>👩🏽‍💻</b> <b>@FereyChannelBot</b>\n\nAdministrateur de la chaîne :\n▪️publication automatique\n▪️décoration automatique",
-    'zh': "<b>👩🏽‍💻</b> <b>@FereyChannelBot</b>\n\n频道管理员：\n▪️自动发布\n▪️自动装饰",
-    'ar': "<b>👩🏽‍💻FereyChannelBot</b>\n\nمسؤول القناة:\nنشر تلقائي <b>@FereyChannelBot</b> n ديكور تلقائي",
+l_add_bot_button = {
+    'ru': "➕ Добавить бота",
+    'en': "➕ Add a bot",
+    'es': "➕ Agregar un bot",
+    'fr': "➕ Ajouter un robot",
+    'zh': "➕ 添加机器人",
+    'ar': "➕ أضف بوت",
 }
-l_kind_4 = {
-    'ru': "<b>👩🏽‍💻@FereyGroupBot</b>\n\n<b>Модерация</b> групп:\n▪️авто-постинг\n▪️модерация",
-    'en': "<b>👩🏽‍💻</b> <b>@FereyGroupBot</b>\n\nGroup admin:\n▪️auto-posting\n▪️moderation",
-    'es': "<b>👩🏽‍💻</b> <b>@FereyGroupBot</b>\n\nAdministrador del grupo:\n▪️publicación automática\n▪️moderación",
-    'fr': "<b>👩🏽‍💻</b> <b>@FereyGroupBot</b>\n\nAdministrateur du groupe :\n▪️publication automatique\n▪️modération",
-    'zh': "<b>👩🏽‍💻</b> <b>@FereyGroupBot</b>\n\n群组管理员：\n▪️自动发布\n▪️审核",
-    'ar': "<b>👩🏽‍💻FereyGroupBot</b>\n\n<b>@FereyGroupBot</b> المجموعة:\nنشر تلقائي\n▪️ تعديل",
+l_add_bot_call = {
+    'ru': "➕ Оформи подписку для >1 бота или открепи активного бота, чтобы добавить нового",
+    'en': "➕ Subscribe for >1 bot or unsubscribe active bot to add a new one",
+    'es': "➕ Suscríbete a >1 bot o cancela la suscripción de un bot activo para agregar uno nuevo",
+    'fr': "➕ Abonnez-vous pour > 1 bot ou désabonnez-vous du bot actif pour en ajouter un nouveau",
+    'zh': "➕ 订阅 >1 个机器人或取消订阅活动机器人以添加新机器人",
+    'ar': "➕ اشترك في> 1 bot أو إلغاء الاشتراك في bot النشط لإضافة واحد جديد",
 }
-l_kind_5 = {
-    'ru': "<b>👩🏽‍💻@FereyUserBot</b>\n\n<b>Автоматизация</b> пользователей:\n▪️авто-постинг\n▪️авто-декор",
-    'en': "<b>👩🏽‍💻</b> <b>@FereyUserBot</b>\n\nUser Admin:\n▪️auto-posting\n▪️auto-decor",
-    'es': "<b>👩🏽‍💻</b> <b>@FereyUserBot</b>\n\nAdministrador de usuarios:\n▪️publicación automática\n▪️decoración automática",
-    'fr': "<b>👩🏽‍💻</b> <b>@FereyUserBot</b>\n\nAdministrateur utilisateur :\n▪️publication automatique\n▪️décoration automatique",
-    'zh': "<b>👩🏽‍💻</b> <b>@FereyUserBot</b>\n\n用户管理员：\n▪️自动发布\n▪️自动装饰",
-    'ar': "<b>👩🏽‍💻FereyUserBot</b>\n\nمسؤول المستخدم:\nنشر <b>@FereyUserBot</b>\nديكور تلقائي",
+l_test_bot_desc = {
+    'ru': "🫥 Описание @{0}-бота:\n\n▪️телеграф блог\n▪️авто-перевод\n▪️оповещения и utm-рефералы\n▪️интеграции",
+    'en': "🫥 @{0}-bot description:\n\n▪️telegraph blog\n▪️auto-translation\n▪️alerts and utm referrals\n▪️integrations",
+    'es': "🫥 @{0}-bot description:\n\n▪️telegraph blog\n▪️traducción automática\n▪️alertas y referencias utm\n▪️integraciones",
+    'fr': "🫥 @{0}-bot description :\n\n▪️blog télégraphique\n▪️traduction automatique\n▪️alertes et références utm\n▪️intégrations",
+    'zh': "🫥 @{0}-bot 描述：\n\n▪️电报博客\n▪️自动翻译\n▪️提醒和 utm 推荐\n▪️集成",
+    'ar': "🫥 @ {0} وصف البرنامج الآلي:\n\n▪️ مدونة telegraph\n▪️ ترجمة تلقائية\n▪️ تنبيهات وإحالات UTM\n▪️ تكامل",
 }
-l_kind_6 = {
-    'ru': "<b>👩🏽‍💻@FereyPostBot</b>\n\n<b>Приватные посты</b>:\n▪️превью\n▪️галерея",
-    'en': "<b>👩🏽‍💻</b> <b>@FereyPostBot</b>\n\nQuick post creation and publishing:\n▪️preview\n▪️gallery",
-    'es': "<b>👩🏽‍💻</b> <b>@FereyPostBot</b>\n\nCreación y publicación rápidas de publicaciones:\n▪️vista previa\n▪️galería",
-    'fr': "<b>👩🏽‍💻</b> <b>@FereyPostBot</b>\n\nCréation et publication rapides d'articles :\n▪️aperçu\n▪️galerie",
-    'zh': "<b>👩🏽‍💻</b> <b>@FereyPostBot</b>\n\n快速创建和发布帖子：\n▪️预览\n▪️图库",
-    'ar': "<b>👩🏽‍💻FereyPostBot</b>\n\nإنشاء منشور سريع <b>@FereyPostBot</b> :\nمعاينة\n▪️ معرض",
+l_clone_bot_button = {
+    'ru': "©️ Клонировать бота",
+    'en': "©️ Clone the bot",
+    'es': "©️ Clonar el bot",
+    'fr': "©️ Cloner le bot",
+    'zh': "©️ 克隆机器人",
+    'ar': "© ️ استنساخ الروبوت",
 }
-l_kind_7 = {
-    'ru': "<b>👩🏽‍💻@FereyFindBot</b>\n\n<b>Поиск</b> по каналам/группам/пользователям/ботам:\n▪️отслеживание постов\n▪️гео-поиск",
-    'en': "<b>👩🏽‍💻</b> <b>@FereyFindBot</b>\n\nSearch by channels/groups/users/bots:\n▪️post tracking\n▪️geo-search",
-    'es': "<b>👩🏽‍💻</b> <b>@FereyFindBot</b>\n\nBuscar por canales/grupos/usuarios/bots:\n▪️seguimiento de publicaciones\n▪️búsqueda geográfica",
-    'fr': "<b>👩🏽‍💻</b> <b>@FereyFindBot</b>\n\nRecherche par canaux/groupes/utilisateurs/bots :\n▪️suivi des publications\n▪️géo-recherche",
-    'zh': "<b>👩🏽‍💻</b> <b>@FereyFindBot</b>\n\n按频道/群组/用户/机器人搜索：\n▪️post tracking\n▪️geo-search",
-    'ar': "<b>👩🏽‍💻FereyFindBot</b>\n\nالبحث عن طريق القنوات / المجموعات <b>@FereyFindBot</b> المستخدمين / الروبوتات:\n▪️ تتبع المنشور\n▪️ البحث الجيو",
+l_clone_bot_call = {
+    'ru': "©️ Оформи подписку для >1 бота или открепи активного бота, чтобы склонировать бота конкурента",
+    'en': "©️ Subscribe >1 bot or unpin an active bot to clone a competitor's bot",
+    'es': "©️ Suscríbete >1 bot o desancla un bot activo para clonar el bot de un competidor",
+    'fr': "©️ Abonnez-vous >1 bot ou désépinglez un bot actif pour cloner le bot d'un concurrent",
+    'zh': "©️ 订阅 >1 个机器人或取消固定一个活跃的机器人以克隆竞争对手的机器人",
+    'ar': "© ️ اشترك> 1 بوت أو قم بإلغاء تثبيت روبوت نشط لاستنساخ روبوت منافس",
 }
-l_kind_8 = {
-    'ru': "<b>👩🏽‍💻@FereyMediaBot</b>\n\n<b>Медиа-заметки</b>:\n▪️аудио/️видео-заметки\n▪️текст/фото-стикеры",
-    'en': "<b>👩🏽‍💻</b> <b>@FereyMediaBot</b>\n\nBot with popular creatives:\n▪️audio notes\n▪️video notes",
-    'es': "<b>👩🏽‍💻</b> <b>@FereyMediaBot</b>\n\nBot con creatividades populares:\n▪️notas de audio\n▪️notas de video",
-    'fr': "<b>👩🏽‍💻</b> <b>@FereyMediaBot</b>\n\nBot avec des créations populaires :\n▪️notes audio\n▪️notes vidéo",
-    'zh': "<b>👩🏽‍💻</b> <b>@FereyMediaBot</b>\n\n具有流行创意的机器人：\n▪️音频笔记\n▪️视频笔记",
-    'ar': "<b>👩🏽‍💻FereyMediaBot</b>\n\nاستخدام التصميمات المشهورة:\n▪️ ملاحظات <b>@FereyMediaBot</b>\n▪️ ملاحظات الفيديو",
+l_clone_bot_text = {
+    'ru': "©️ <b>Вставь</b> корректную ссылку на бота, чтобы склонировать его",
+    'en': "©️ <b>Paste</b> the correct link to the bot to clone it",
+    'es': "©️ <b>Pega</b> el enlace correcto al bot para clonarlo",
+    'fr': "©️ <b>Collez</b> le bon lien vers le bot pour le cloner",
+    'zh': "©️ 将正确的链接<b>粘贴</b>到机器人以克隆它",
+    'ar': "© ️ <b>الصق</b> الرابط الصحيح إلى الروبوت لاستنساخه",
 }
-l_kind_9 = {
-    'ru': "<b>👩🏽‍💻@FereyVPNBot</b>\n\n<b>Настройка</b>VPN",
-    'en': "<b>👩🏽‍💻</b> <b>@FereyVpnBot</b>\n\nAll about VPN",
-    'es': "<b>👩🏽‍💻</b> <b>@FereyVpnBot</b>\n\nTodo sobre VPN",
-    'fr': "<b>👩🏽‍💻</b> <b>@FereyVpnBot</b>\n\nTout sur le VPN",
-    'zh': "<b>👩🏽‍💻</b> <b>@FereyVpnBot</b>\n\n关于 VPN",
-    'ar': "<b>👩🏽‍💻FereyVpnBot</b> <b>@FereyVpnBot</b> n\nكل شيء عن VPN",
+l_clone_bot_wait = {
+    'ru': "©️ <b>Клонирование</b> бота\n\n#длительность 1мин",
+    'en': "©️ Bot <b>cloning</b>\n\n#duration 1 min",
+    'es': "©️ <b>Clonación</b> de bots\n\n#duración 1 min",
+    'fr': "©️ <b>Clonage</b> de bot\n\n#durée 1 min",
+    'zh': "©️ Bot<b>克隆</b>\n\n#duration 1 分钟",
+    'ar': "© ️ <b>استنساخ</b> الروبوت\n\n# المدة 1 دقيقة",
 }
-l_kind_10 = {
-    'ru': "<b>👩🏽‍💻@FereyTargetBot</b>\n\n<b>Таргет</b> сообщений/пользователей",
-    'en': "<b>👩🏽‍💻</b> <b>@FereyTargetBot</b>\n\nTargeted email",
-    'es': "<b>👩🏽‍💻</b> <b>@FereyTargetBot</b>\n\nCorreo electrónico dirigido",
-    'fr': "<b>👩🏽‍💻</b> <b>@FereyTargetBot</b>\n\nE-mail ciblé",
-    'zh': "<b>👩🏽‍💻</b> <b>@FereyTargetBot</b>\n\n目标电子邮件",
-    'ar': "<b>👩🏽‍💻FereyTargetBot</b> \ <b>@FereyTargetBot</b>\nالبريد الإلكتروني المستهدف",
+l_addbot_handler = {
+    'ru': "➕ Пришли корректный <b>ТОКЕН</b> Telegram-бота, полученный с помощью @botFather-бота\n\n👩🏽‍💻 Например, 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
+    'en': "➕ We sent the correct Telegram bot <b>TOKEN</b> received using @botFather bot\n\n👩🏽‍💻 For example, 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
+    'es': "➕ Enviamos el <b>TOKEN</b> de bot de Telegram correcto recibido usando @botFather bot\n\n👩🏽‍💻 Por ejemplo, 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
+    'fr': "➕ Nous avons envoyé le bon <b>jeton</b> de bot Telegram reçu à l&#x27;aide du bot @botFather\n\n👩🏽‍💻 Par exemple, 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
+    'zh': "➕ 我们发送了使用@botFather bot\n\n👩🏽‍💻 收到的正确的 Telegram bot <b>TOKEN</b>例如， 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
+    'ar': "➕ أرسلنا <b>برنامج</b> Telegram bot الصحيح الذي تم استلامه باستخدام @botFather bot\n\n👩🏽‍💻 على سبيل المثال ، 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
 }
-l_kind_11 = {
-    'ru': "<b>👩🏽‍💻@FereyToolsBot</b>\n\n<b>Телеграм инструменты</b>:\n▪️конвертация файлов\n▪️шаблоны",
-    'en': "<b>👩🏽‍💻</b> <b>@FereyToolsBot</b>\n\nTool bot:\n▪️convert\n▪️download",
-    'es': "<b>👩🏽‍💻</b> <b>@FereyToolsBot</b>\n\nHerramienta bot:\n▪️convertir\n▪️descargar",
-    'fr': "<b>👩🏽‍💻</b> <b>@FereyToolsBot</b>\n\nBot outil :\n▪️convertir\n▪️télécharger",
-    'zh': "<b>👩🏽‍💻</b> <b>@FereyToolsBot</b>\n\n工具机器人：\n▪️转换\n▪️下载",
-    'ar': "<b>👩🏽‍💻FereyToolsBot</b>\n\ <b>@FereyToolsBot</b> بوت الأداة:\n▪️ تحويل\n▪️ تحميل",
+l_wait_for_translate_bot = {
+    'ru': "👩🏽‍💻 <b>Перевод</b> {0}-бота на <i>{1}</i>-язык\n\n#длительность 0мин",
+    'en': "👩🏽‍💻 <b>Translation of</b> {0}-bot into <i>{1}</i> -language\n\n#duration 0min",
+    'es': "👩🏽‍💻 <b>Traducción de</b> {0}-bot a <i>{1}</i> -idioma\n\n#duración 0min",
+    'fr': "👩🏽‍💻 <b>Traduction de</b> {0}-bot en <i>{1}</i> -langue\n\n#durée 0min",
+    'zh': "👩🏽‍💻 将 {0}-bot<b>翻译</b>成<i>{1}</i> -language\n\n#duration 0min",
+    'ar': "👩🏽‍💻 <b>ترجمة</b> {0} - الروبوت إلى <i>{1}</i> -اللغة\n\n# المدة 0 دقيقة",
 }
-l_kind_12 = {
-    'ru': "<b>👩🏽‍💻@FereyAIBot</b>\n\n<b>Нейросеть</b> генерации контента (open-ai):\n▪️chat-gpt\n▪️dalli·e",
-    'en': "<b>👩🏽‍💻</b> <b>@FereyAIBot</b>\n\nContent generation bot (open-ai):\n▪️chat-gpt\n▪️dalli e",
-    'es': "<b>👩🏽‍💻</b> <b>@FereyAIBot</b>\n\nBot de generación de contenido (open-ai):\n▪️chat-gpt\n▪️dalli e",
-    'fr': "<b>👩🏽‍💻</b> <b>@FereyAIBot</b>\n\nBot de génération de contenu (open-ai) :\n▪️chat-gpt\n▪️dalli e",
-    'zh': "<b>👩🏽‍💻</b> <b>@FereyAIBot</b>\n\n内容生成机器人（open-ai）：\n▪️chat-gpt\n▪️dalli e",
-    'ar': "<b>👩🏽‍💻FereyAIBot</b>\n\nروبوت إنشاء المحتوى (open <b>@FereyAIBot</b> ai):\n▪️chat-gpt\n▪️dalli e",
+l_template_is_ready = {
+    'ru': "👩🏽‍💻 <b>Шаблон</b> для @{0} готов!",
+    'en': "👩🏽‍💻 <b>Template</b> for @{0} is ready!",
+    'es': "👩🏽‍💻 ¡ <b>La plantilla</b> para @{0} está lista!",
+    'fr': "👩🏽‍💻 <b>Le modèle</b> pour @{0} est prêt !",
+    'zh': "👩🏽‍💻 @{0} 的<b>模板</b>已准备就绪！",
+    'ar': "👩🏽‍💻 <b>نموذج</b> @ {0} جاهز!",
 }
-l_kind_13 = {
-    'ru': "<b>👩🏽‍💻@FereyAdsBot</b>\n\n<b>Реклама</b> в:\n▪️ботах",
-    'en': "<b>👩🏽‍💻</b> <b>@FereyAdsBot</b>\n\nBot ads in:\n▪️bots\n▪️channels",
-    'es': "<b>👩🏽‍💻</b> <b>@FereyAdsBot</b>\n\nAnuncios de bot en:\n▪️bots\n▪️canales",
-    'fr': "<b>👩🏽‍💻</b> <b>@FereyAdsBot</b>\n\nAnnonces de robots dans :\n▪️bots\n▪️chaînes",
-    'zh': "<b>👩🏽‍💻</b> <b>@FereyAdsBot</b>\n\n机器人广告在：\n▪️bots\n▪️channels",
-    'ar': "<b>👩🏽‍💻FereyAdsBot</b>\n\n<b>@FereyAdsBot</b> الإعلانات في:\n▪️ الروبوتات\n▪️ القنوات",
+l_payment_successful = {
+    'ru': "👩🏽‍💻 <b>Пользователь</b> {0} 💰Внес оплату в размере {1} {2}",
+    'en': "👩🏽‍💻 <b>User</b> {0} 💰Paid payment in the amount of {1} {2}",
+    'es': "👩🏽‍💻 <b>Usuario</b> {0} 💰Pago pagado por la cantidad de {1} {2}",
+    'fr': "👩🏽‍💻 <b>Utilisateur</b> {0} 💰Paiement payé d'un montant de {1} {2}",
+    'zh': "👩🏽‍💻<b>用户</b>{0} 💰支付金额为{1} {2}",
+    'ar': "👩🏽‍💻 <b>المستخدم</b> {0} 💰 دفعة مدفوعة بمبلغ {1} {2}",
 }
-l_kind_14 = {
-    'ru': "<b>👩🏽‍💻@FereyWorkBot</b>\n\n<b>Рабочий</b> бот информации о:\n▪️вакансиях\n▪️соревнованиях",
-    'en': "<b>👩🏽‍💻</b> <b>@FereyWorkBot</b>\n\nBot of information about:\n▪️vacancies\n▪️competitions",
-    'es': "<b>👩🏽‍💻</b> <b>@FereyWorkBot</b>\n\nBot de información sobre:\n▪️vacantes\n▪️concursos",
-    'fr': "<b>👩🏽‍💻</b> <b>@FereyWorkBot</b>\n\nBot d'informations sur :\n▪️offres d'emploi\n▪️concours",
-    'zh': "<b>👩🏽‍💻</b> <b>@FereyWorkBot</b>\n\n有关以下信息的机器人：\n▪️职位空缺\n▪️比赛",
-    'ar': "<b>👩🏽‍💻FereyWorkBot</b>\n\nبعض <b>@FereyWorkBot</b> حول:\n▪️ وظائف شاغرة\n▪️ مسابقات",
+l_promocode_activated = {
+    'ru': "👩🏽‍💻 *Промокод*: `{txt}` активирован",
+    'en': "👩🏽‍💻 *Promo code*: `{txt}` activated",
+    'es': "👩🏽‍💻 *Código promocional*: `{txt}` activado",
+    'fr': "👩🏽‍💻 *Code promotionnel* : `{txt}` activé",
+    'zh': "👩🏽‍💻 *促销代码*：`{txt}` 激活",
+    'ar': "👩🏽‍💻 * الرمز الترويجي *: '{txt}` مفعل",
 }
-# endregion
-
 
-# region FereyWorkBot
-l_work_btn1 = {
-    'ru': "⛰️ Вакансии",
-    'en': "⛰️ Jobs",
-    'es': "⛰️ Empleos",
-    'fr': "⛰️ Emplois",
-    'zh': "⛰️ 工作",
-    'ar': "⛰️ وظائف",
+# region commands
+l_bot_commands_handler = {
+    'ru': "⚙️ <b>Команды</b> /cmd для <b>@{0}</b>\n\n/info   <i>информация</i>\n/stat   <i>аналитика</i>\n/status <i>статус</i>\n/on     <i>включение</i>\n/off    <i>выключение</i>\n/restart  <i>перезагрузка</i>\n\n/parse [premium|admin|utm|ban]\n/admin [id]    <i>администраторы</i>\n/promo      <i>промокод</i>\n/ban [id/@username]   <i>список</i>\n/unban     <i>разбан</i>",
+    'en': "⚙️ <b>Commands</b> /cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>promo code</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
+    'es': "⚙️ <b>Comandos</b> /cmd para <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disabled</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>administradores</i>\n/promo <i>código de promoción</i>\n/ban [id/ @username ] <i>lista</i>\n/unban <i>no baneado</i>",
+    'fr': "⚙️ <b>Commandes</b> /cmd pour <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>recharger</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>code promo</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
+    'zh': "⚙️<b>命令</b>/cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo<i>促销代码</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
+    'ar': "⚙️ <b>أوامر</b> / cmd لـ <b>@ {0}</b>\n\n/ info <i>info</i>\n/ stat <i>analytics</i>\n/ status <i>status</i>\n/ on <i>تمكين</i>\n/off <i>تعطيل</i>\n/restart <i>تحميل</i>\n\n/ parse [premium | admin | utm | ban]\n/ admin [id] <i>admins</i>\n/ <i>promo code</i>\n/ ban [id / @username ] <i>list</i>\n/ <i>unsanned</i>",
 }
-l_work_btn2 = {
-    'ru': "🌬 Подписка",
-    'en': "🌬 Subscription",
-    'es': "🌬 Suscripción",
-    'fr': "🌬 Abonnement",
-    'zh': "🌬订阅",
-    'ar': "🌬 الاشتراك",
+l_bot_status_handler = {
+    'ru': "👩🏽‍💻 <b>Статус</b> @{0}-бота: {1}",
+    'en': "👩🏽‍💻 <b>Status</b> @{0}-bot: {1}",
+    'es': "👩🏽‍💻 <b>Estado</b> @{0}-bot: {1}",
+    'fr': "👩🏽‍💻 <b>Statut</b> @{0}-bot : {1}",
+    'zh': "👩🏽‍💻<b>状态</b>@{0}-bot：{1}",
+    'ar': "👩🏽‍💻 <b>الحالة</b> @ {0} -روبوت: {1}",
 }
-l_work_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> проекта <b>Ferey</b>:\n\n▪️<b>вакансии</b> нашего стартапа\n▪️конкурсы и <b>мероприятия</b>\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to <i>the landing bot</i> of the <b>Ferey</b> проекта :\n\n▪️ <b>vacancies</b> of our startup\n▪️ contests and <b>events</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del проекта <b>Ferey</b> :\n\n▪️ <b>vacantes</b> de nuestra startup\n▪️ concursos y <b>eventos</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du проекта <b>Ferey</b> :\n\n▪️ <b>offres d&#x27;emploi</b> de notre startup\n▪️ concours et <b>événements</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎来到<b>Ferey</b> проекта的<i>登陆机器人</i>：\n\n▪️ 我们初创公司的<b>职位空缺</b>\n▪️ 竞赛和<b>活动</b>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> проекта <b>Ferey</b> :\n\n▪️ <b>الشواغر</b> في بدء التشغيل\n▪️ المسابقات <b>والأحداث</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey",
+l_bot_on_handler = {
+    'ru': "👩🏽‍💻 <b>Запуск</b> @{0}-бота..\n\n#длительность 1мин",
+    'en': "👩🏽‍💻 <b>Launch</b> @{0}-bot..\n\n#duration 1 min",
+    'es': "👩🏽‍💻 <b>Lanzar</b> @{0}-bot..\n\n#duración 1 min",
+    'fr': "👩🏽‍💻 <b>Lancer</b> @{0}-bot..\n\n#durée 1 min",
+    'zh': "👩🏽‍💻<b>启动</b>@{0}-bot..\n\n#duration 1 分钟",
+    'ar': "👩🏽‍💻 <b>Launch</b> @ {0} -bot ..\n\n# المدة 1 دقيقة",
 }
-l_subscribe_work = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
-    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
-    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
-    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
-    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
-    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+l_bot_on_handler_already = {
+    'ru': "👩🏽‍💻 <b>@{0}</b>-бот уже запущен",
+    'en': "👩🏽‍💻 <b>@{0}</b> - the bot is already running",
+    'es': "👩🏽‍💻 <b>@{0}</b> : el bot ya se está ejecutando",
+    'fr': "👩🏽‍💻 <b>@{0}</b> - le bot est déjà en cours d'exécution",
+    'zh': "👩🏽‍💻 <b>@{0}</b> - 机器人已经在运行",
+    'ar': "👩🏽‍💻 <b>@ {0}</b> - الروبوت قيد التشغيل بالفعل",
 }
-
-l_vacancy_1 = {
-    'ru': "👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company",
-    'en': "👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company",
-    'es': "👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTareas: crear máscaras ferey (video realista) para cualquier humano\nGénero: niña\nEdad: menos de 30\nPago: parte de la empresa",
-    'fr': "👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTâches : créer des masques de ferey (vidéo réaliste) pour tout humain\nSexe : fille\nÂge : moins de 30 ans\nPaiement : part de l'entreprise",
-    'zh': "👩🏽‍💻<b>文本到视频 ai-designer</b>\n\n任务：为任何人创建 ferey-mask（逼真的视频）\n性别：女孩\n年龄：30 岁以下\n薪酬：公司股份",
-    'ar': "👩🏽‍💻 <b>نص إلى فيديو مصمم ai</b>\n\nالمهام: إنشاء أقنعة ضيقة (فيديو واقعي) لأي إنسان\nالجنس: فتاة\nالعمر: أقل من 30\nالدفع: حصة الشركة",
+l_bot_off_handler = {
+    'ru': "👩🏽‍💻 <b>Остановка</b> @{0}-бота..\n\n#длительность 1мин",
+    'en': "👩🏽‍💻 @{0}-bot <b>stop</b> ..\n\n#duration 1 min",
+    'es': "👩🏽‍💻 @{0}-bot <b>parada</b> ..\n\n#duración 1 min",
+    'fr': "👩🏽‍💻 @{0}-bot <b>stop</b> ..\n\n#durée 1 min",
+    'zh': "👩🏽‍💻 @{0}-bot<b>停止</b>..\n\n#duration 1 分钟",
+    'ar': "👩🏽‍💻 @ {0} -bot <b>stop</b> ..\n\n# المدة 1 دقيقة",
 }
-l_vacancy_2 = {
-    'ru': "👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials",
-    'en': "👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials",
-    'es': "👩🏽‍💻 <b>Creador de contenido/video</b>\n\nTareas: generar creatividades para todas las redes sociales\nGénero: niña\nEdad: menos de 30\nPago: 1 TON por 1 publicación para todas las redes sociales",
-    'fr': "👩🏽‍💻 <b>Créateur de contenu/vidéo</b>\n\nTâches : générer des créations pour tous les réseaux sociaux\nSexe : fille\nÂge : moins de 30 ans\nPaiement : 1 TON pour 1 post pour tous les réseaux sociaux",
-    'zh': "👩🏽‍💻<b>内容/视频制作者</b>\n\n任务：为所有社交生成创意\n性别：女孩\n年龄：小于 30\n报酬：所有社交每 1 个帖子 1 吨",
-    'ar': "👩🏽‍💻 <b>صانع المحتوى / الفيديو</b>\n\nالمهام: إنشاء تصميمات لجميع وسائل التواصل الاجتماعي\nالجنس: فتاة\nالعمر: أقل من 30\nالدفع: 1 طن لكل مشاركة واحدة لجميع الشبكات الاجتماعية",
+l_bot_off_handler_already = {
+    'ru': "👩🏽‍💻 <b>@{0}</b>-бот уже выключен",
+    'en': "👩🏽‍💻 <b>@{0}</b> -bot is already off",
+    'es': "👩🏽‍💻 <b>@{0}</b> -bot ya está apagado",
+    'fr': "👩🏽‍💻 <b>@{0}</b> -bot est déjà désactivé",
+    'zh': "👩🏽‍💻 <b>@{0}</b> -bot 已经关闭",
+    'ar': "الروبوت 👩🏽‍💻 <b>@ {0}</b> متوقف بالفعل",
 }
-l_vacancy_3 = {
-    'ru': "👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company",
-    'en': "👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company",
-    'es': "👩🏽‍💻 <b>Desarrollador Aio/pyro-gram</b>\n\nTareas: desarrollar y apoyar todos los proyectos\nGénero: niña\nEdad: menos de 30\nPago: parte de la empresa",
-    'fr': "👩🏽‍💻 <b>Développeur Aio/pyro-gram</b>\n\nTâches : développement et support de tous les projets\nSexe : fille\nÂge : moins de 30 ans\nRémunération : part de l'entreprise",
-    'zh': "👩🏽‍💻 <b>Aio/pyro-gram 开发者</b>\n\n任务：开发和支持所有项目\n性别：女孩\n年龄：30岁以下\n薪酬：公司股份",
-    'ar': "👩🏽‍💻 <b>مطور Aio / pyro-gram</b>\n\nالمهام: تطوير ودعم جميع المشاريع\nالجنس: فتاة\nالعمر: أقل من 30\nالدفع: حصة الشركة",
+l_bot_off_handler_done = {
+    'ru': "👩🏽‍💻 <b>@{0}</b>-бот выключен",
+    'en': "👩🏽‍💻 <b>@{0}</b> -bot is off",
+    'es': "👩🏽‍💻 <b>@{0}</b> -bot está apagado",
+    'fr': "👩🏽‍💻 <b>@{0}</b> -bot est désactivé",
+    'zh': "👩🏽‍💻 <b>@{0}</b> -bot 已关闭",
+    'ar': "👩🏽‍💻 <b>@ {0}</b> -الروبوت غير مفعّل",
+}
+l_bot_restart_handler = {
+    'ru': "👩🏽‍💻 <b>Перезапуск</b> @{0}-бота..\n\n#длительность 1мин",
+    'en': "👩🏽‍💻 @{0}-bot <b>restart</b> ..\n\n#duration 1 min",
+    'es': "👩🏽‍💻 @{0}-bot <b>reinicio</b> ..\n\n#duración 1 min",
+    'fr': "👩🏽‍💻 @{0}-bot <b>restart</b> ..\n\n#durée 1 min",
+    'zh': "👩🏽‍💻@{0}-bot<b>重启</b>..\n\n#duration 1 分钟",
+    'ar': "👩🏽‍💻 @ {0} -bot <b>إعادة التشغيل</b> ..\n\n# المدة 1 دقيقة",
 }
 # endregion
 
 
-# region FereyAIBot
-l_ai_btn1 = {
-    'ru': "⛰️ Нейросети",
-    'en': "⛰️ Neural networks",
-    'es': "⛰️ Redes neuronales",
-    'fr': "⛰️ Réseaux de neurones",
-    'zh': "⛰️ 神经网络",
-    'ar': "⛰️ الشبكات العصبية",
-}
-l_ai_btn2 = {
-    'ru': "🌬 Подписка",
-    'en': "🌬 Subscription",
-    'es': "🌬 Suscripción",
-    'fr': "🌬 Abonnement",
-    'zh': "🌬订阅",
-    'ar': "🌬 الاشتراك",
-}
-l_ai_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для генерации контента:\n\n▪️<b>текст/изображение</b>\n▪️<b>анализ @telegram-канала</b>\n▪️<b>распознавание</b> речи\n▪️<b>очистка ⁰истории</b> /start\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to the content генерации <i>landing bot</i> :\n\n▪️ <b>text</b>\n▪️ <b>image</b>\n▪️ <b>analysis of the Telegram channel</b>\n\n❗️ you can also order the development of a chat bot in our studio Ferey",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> генерации de contenido :\n\n▪️ <b>texto</b>\n▪️ <b>imagen</b>\n▪️ <b>análisis del canal de Telegram</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue dans le <i>landing bot</i> генерации de contenu :\n\n▪️ <b>texte</b>\n▪️ <b>image</b>\n▪️ <b>analyse de la chaîne Telegram</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎使用内容генерации<i>登陆机器人</i>：\n\n▪️<b>文字</b>\n▪️<b>图片</b>\n▪️ <b>Telegram 频道分析</b>\n\n❗️ 您也可以在我们的工作室Ferey订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت إنشاء</i> генерации :\n\n▪️ <b>نص</b>\n▪️ <b>صورة</b>\n▪️ <b>تحليل قناة Telegram</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
-}
-l_subscribe_ai = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️отсутствие <b>режима ожидания</b>\n▪️аналитика постов канала\n(<i>+финансовый потенциал</i>)\n\n👩🏽‍💻 /balance",
-    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
-    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
-    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
-    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
-    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
-}
+# region bot
+l_bot_config = {
+    ("cctor", "👩🏽‍💻", "☑"): {
+        'ru': "Конструктор ᴺᴱᵂ",
+        'en': "Builder ᴺᴱᵂ",
+        'es': "Builder ᴺᴱᵂ",
+        'fr': "Builder ᴺᴱᵂ",
+        'zh': "Builder ᴺᴱᵂ",
+        'ar': "Builder ᴺᴱᵂ",
+    },
+    ("cban", "🕵🏽", "☑"): {
+        'ru': "Авто-бан",
+        'en': "Auto-ban",
+        'es': "Prohibición automática",
+        'fr': "Interdiction automatique",
+        'zh': "自動禁止",
+        'ar': "حظر تلقائي",
+    },
+    ("ctranslate", "文", "☐"): {
+        'ru': "Авто-перевод",
+        'en': "Auto-translate",
+        'es': "Saludo automático",
+        'fr': "Message d'accueil automatique",
+        'zh': "自動問候",
+        'ar': "الترحيب التلقائي",
+    },
+    ("canswer", "👋🏽", "☐"): {
+        'ru': "Авто-ответ",
+        'en': "Auto-answer",
+        'es': "Saludo automático",
+        'fr': "Message d'accueil automatique",
+        'zh': "自動問候",
+        'ar': "الترحيب التلقائي",
+    },
+    ("cpost", "🔔", "☐"): {
+        'ru': "Авто-постинг",
+        'en': "Auto-posting",
+        'es': "Publicación automática",
+        'fr': "Publication automatique",
+        'zh': "自動發布",
+        'ar': "النشر التلقائي",
+    },
 
-l_gen_txt = {
-    'ru': "📘 Текст{0}",
-    'en': "📘 Text{0}",
-    'es': "📘 Texto{0}",
-    'fr': "📘 Texte{0}",
-    'zh': "📘 文字{0}",
-    'ar': "📘 نص {0}",
-}
-l_gen_img = {
-    'ru': "🌌 Образ",
-    'en': "🌌 Image",
-    'es': "🌌 Imagen",
-    'fr': "🌌 Image",
-    'zh': "🌌 图片",
-    'ar': "🌌 صورة",
-}
-l_gen_tlg = {
-    'ru': "👩🏽‍💻 Анализ @telegram-канала",
-    'en': "👩🏽‍💻 Telegram channel analysis",
-    'es': "👩🏽‍💻 Análisis de canales de Telegram",
-    'fr': "👩🏽‍💻 Analyse des chaînes de télégrammes",
-    'zh': "👩🏽‍💻电报频道分析",
-    'ar': "👩🏽‍💻 تحليل قناة Telegram",
-}
-l_generate_main = {
-    'ru': "👩🏽‍💻 <b>Выбери режим</b>",
-    'en': "👩🏽‍💻 <b>Choose a mode</b>",
-    'es': "👩🏽‍💻 <b>Elige un modo</b>",
-    'fr': "👩🏽‍💻 <b>Choisissez un mode</b>",
-    'zh': "👩🏽‍💻<b>选择模式</b>",
-    'ar': "👩🏽‍💻 <b>اختر الوضع</b>",
+    ("cpayment", "💳", "☐"): {
+        'ru': "Платежи",
+        'en': "Payments",
+        'es': "Prohibición automática",
+        'fr': "Interdiction automatique",
+        'zh': "自動禁止",
+        'ar': "حظر تلقائي",
+    },
+    ("cintegration", "🗝️", "☐"): {
+        'ru': "Интеграции",
+        'en': "Integrations",
+        'es': "Publicación automática",
+        'fr': "Publication automatique",
+        'zh': "自動發布",
+        'ar': "النشر التلقائي",
+    },
+    ("cnotification", "💬", "☑"): {
+        'ru': "Оповещения",
+        'en': "Notifications",
+        'es': "Mensajes con 文/ب/y",
+        'fr': "Messagerie avec 文/ب/y",
+        'zh': "與消息 文/ب/y",
+        'ar': "文/ب/y الرسائل ذات",
+    },
+    ("cuser", "👥", "☑"): {
+        'ru': "Пользователи",
+        'en': "Users",
+        'es': "Mensajes con 文/ب/y",
+        'fr': "Messagerie avec 文/ب/y",
+        'zh': "與消息 文/ب/y",
+        'ar': "文/ب/y الرسائل ذات",
+    },
+    ("cadmin", "👮🏽", "☑"): {
+        'ru': "Администраторы",
+        'en': "Administrators",
+        'es': "Mensajes con 文/ب/y",
+        'fr': "Messagerie avec 文/ب/y",
+        'zh': "與消息 文/ب/y",
+        'ar': "文/ب/y الرسائل ذات",
+    },
 }
-l_generate_prompt = {
-    'ru': "👩🏽‍💻 <b>Введи</b> запрос для <b>{0}</b> 👇🏼..",
-    'en': "👩🏽‍💻 <b>Enter</b> a query for <b>{0}</b> 👇🏼..",
-    'es': "👩🏽‍💻 <b>Ingrese</b> una consulta para <b>{0}</b> 👇🏼..",
-    'fr': "👩🏽‍💻 <b>Entrez</b> une requête pour <b>{0}</b> 👇🏼..",
-    'zh': "👩🏽‍💻<b>输入</b>查询<b>{0}</b> 👇🏼..",
-    'ar': "👩🏽‍💻 <b>أدخل</b> استعلامًا عن <b>{0}</b> 👇🏼 ..",
+l_remove_bot = {
+    'ru': "🚫Убрать бота",
+    'en': "🚫Remove bot",
+    'es': "🚫Eliminar bot",
+    'fr': "🚫Supprimer le robot",
+    'zh': "🚫删除机器人",
+    'ar': "🚫 إزالة البوت",
 }
-l_generate_chn = {
-    'ru': "👩🏽‍💻 <b>Вставь</b> ссылку на @telegram-канал для анализа финансовых показателей",
-    'en': "👩🏽‍💻 <b>Insert</b> a link to the Telegram channel to analyze financial performance",
-    'es': "👩🏽‍💻 <b>Inserta</b> un enlace al canal de Telegram para analizar el desempeño financiero",
-    'fr': "👩🏽‍💻 <b>Insérez</b> un lien vers la chaîne Telegram pour analyser les performances financières",
-    'zh': "👩🏽‍💻<b>插入</b>到 Telegram 频道的链接以分析财务绩效",
-    'ar': "👩🏽‍💻 <b>أدخل</b> رابطًا إلى قناة Telegram لتحليل الأداء المالي",
+
+l_show_bots = {
+    'ru': "👩🏽‍💻 <b>Добавленные боты</b>\n\n[команды /cmd]",
+    'en': "👩🏽‍💻 <b>Added bots</b>\n\n[commands /cmd]",
+    'es': "👩🏽‍💻 <b>Se agregaron bots</b>\n\n[comandos /cmd]",
+    'fr': "👩🏽‍💻 <b>Ajout de bots</b>\n\n[commandes /cmd]",
+    'zh': "👩🏽‍💻<b>添加了机器人</b>\n\n[命令/cmd]",
+    'ar': "👩🏽‍💻 <b>الروبوتات المضافة</b>\n\n[أوامر / cmd]",
 }
-l_generate_wait = {
-    'ru': "👩🏽‍💻 <b>Выбери режим</b> или <b>дождись</b> окончания генерации..",
-    'en': "👩🏽‍💻 <b>Choose a mode</b> or <b>wait for</b> the generation to finish..",
-    'es': "👩🏽‍💻 <b>Elija un modo</b> o <b>espere a</b> que termine la generación..",
-    'fr': "👩🏽‍💻 <b>Choisissez un mode</b> ou <b>attendez la fin de</b> la génération..",
-    'zh': "👩🏽‍💻<b>选择一种模式</b>或<b>等待</b>生成完成..",
-    'ar': "👩🏽‍💻 <b>اختر وضعًا</b> أو <b>انتظر حتى</b> ينتهي الجيل ..",
+
+l_creturntext = {
+    'ru': "✖️ <b>Сбросить</b> настройки по умолчанию (до рекомендуемых) для бота [<b>{0}</b>]?",
+    'en': "✖️ <b>Reset</b> default settings (recommended) for bot [<b>{0}</b>]?",
+    'es': "✖️ <b>¿Restablecer</b> la configuración predeterminada (recomendado) para el bot [<b>{0}</b>]?",
+    'fr': "✖️ <b>Réinitialiser</b> les paramètres par défaut (recommandé) pour le bot [<b>{0}</b>] ?",
+    'zh': "✖️<b>重置</b>机器人 [<b>{0}</b>] 的默认设置（推荐）？",
+    'ar': "✖️ <b>إعادة تعيين</b> الإعدادات الافتراضية (موصى به) للروبوت [<b>{0}</b>]؟",
 }
-l_generate_subcribe = {
-    'ru': "👩🏽‍💻 Подожди {0}сек или оформи подписку",
-    'en': "👩🏽‍💻 Wait {0}sec or subscribe",
-    'es': "👩🏽‍💻 Espera {0}segundos o suscríbete",
-    'fr': "👩🏽‍💻 Attendez {0}sec ou abonnez-vous",
-    'zh': "👩🏽‍💻 等待 {0} 秒或订阅",
-    'ar': "👩🏽‍💻 انتظر {0} ثانية أو اشترك",
+l_creturnanswer = {
+    'ru': "✖️ Настройки бота [<b>{0}</b>] успешно сброшены!",
+    'en': "✖️ Bot settings [<b>{0}</b>] successfully reset!",
+    'es': "✖️ ¡La configuración del bot [<b>{0}</b>] se restableció correctamente!",
+    'fr': "✖️ Les paramètres du bot [<b>{0}</b>] ont été réinitialisés avec succès !",
+    'zh': "✖️ 机器人设置 [<b>{0}</b>] 成功重置！",
+    'ar': "✖️ تم إعادة تعيين إعدادات البوت [<b>{0}</b>] بنجاح!",
 }
-l_generate_subcribe_channel = {
-    'ru': "👩🏽‍💻 Оформи подписку, чтобы узнать финансовый потенциал твоего @telegram-канала",
-    'en': "👩🏽‍💻 Wait {0}sec or subscribe",
-    'es': "👩🏽‍💻 Espera {0}segundos o suscríbete",
-    'fr': "👩🏽‍💻 Attendez {0}sec ou abonnez-vous",
-    'zh': "👩🏽‍💻 等待 {0} 秒或订阅",
-    'ar': "👩🏽‍💻 انتظر {0} ثانية أو اشترك",
+l_cdeletetext = {
+    'ru': "🚫 Убрать привязку бота [<b>{0}</b>]?",
+    'en': "🚫 Remove bot binding [<b>{0}</b>]?",
+    'es': "🚫 ¿Eliminar el enlace del bot [<b>{0}</b>]?",
+    'fr': "🚫 Supprimer la liaison du bot [<b>{0}</b>] ?",
+    'zh': "🚫 删除机器人绑定 [<b>{0}</b>]？",
+    'ar': "🚫 إزالة ربط البوت [<b>{0}</b>]؟",
 }
-l_generate_error = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> генерации",
-    'en': "👩🏽‍💻 Generation <b>Error</b>",
-    'es': "👩🏽‍💻 <b>Error</b> de generación",
-    'fr': "👩🏽‍💻 <b>Erreur</b> de génération",
-    'zh': "👩🏽‍💻 生成<b>错误</b>",
-    'ar': "👩🏽‍💻 <b>خطأ</b> في التوليد",
+l_cdeleteanswer = {
+    'ru': "🚫 Бот успешно откреплен [<b>{0}</b>]",
+    'en': "🚫 Bot successfully unlocked [<b>{0}</b>]",
+    'es': "🚫 Bot desbloqueado con éxito [<b>{0}</b>]",
+    'fr': "🚫 Bot déverrouillé avec succès [<b>{0}</b>]",
+    'zh': "🚫 机器人成功解锁 [<b>{0}</b>]",
+    'ar': "🚫 تم فتح بوت بنجاح [<b>{0}</b>]",
 }
-l_generate_errchn = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> доступа к каналу (попробуй позже или сделай канал публичным)",
-    'en': "👩🏽‍💻 Channel access <b>error</b> (try later or make the channel public)",
-    'es': "👩🏽‍💻 <b>Error</b> de acceso al canal (inténtalo más tarde o haz público el canal)",
-    'fr': "👩🏽‍💻 <b>Erreur</b> d'accès à la chaîne (essayez plus tard ou rendez la chaîne publique)",
-    'zh': "👩🏽‍💻频道访问<b>错误</b>（稍后再试或公开频道）",
-    'ar': "👩🏽‍💻 <b>خطأ</b> في الوصول إلى القناة (حاول لاحقًا أو اجعل القناة عامة)",
+l_transfer_success = {
+    'ru': "👩🏽‍💻 <b>Права</b> владения на @{0}-бота успешно переданы @{1}-аккаунту!\n\n👩🏽‍💻 Теперь для передачи прав/настройки можно использовать @botfather-бота",
+    'en': "👩🏽‍💻 <b>Ownership</b> of @{0}-bot successfully transferred to @{1}-account!\n\n👩🏽‍💻 You can now use @botfather -bot to transfer ownership/configuration",
+    'es': "👩🏽‍💻 ¡ <b>La propiedad</b> de @{0}-bot se transfirió con éxito a @{1}-cuenta!\n\n👩🏽‍💻 Ahora puedes usar @botfather -bot para transferir la propiedad/configuración",
+    'fr': "👩🏽‍💻 <b>La propriété</b> de @{0}-bot a été transférée avec succès vers @{1}-compte !\n\n👩🏽‍💻 Vous pouvez maintenant utiliser @botfather -bot pour transférer la propriété/configuration",
+    'zh': "👩🏽‍💻 @{0}-bot 的<b>所有权</b>已成功转移到@{1}-帐户！\n\n👩🏽‍💻 您现在可以使用@botfather -bot 转移所有权/配置",
+    'ar': "👩🏽‍💻 تم نقل <b>ملكية</b> @ {0} -bot بنجاح إلى @ {1} -account!\n\n👩🏽‍💻 يمكنك الآن استخدام @botfather -bot لنقل الملكية / التهيئة",
 }
 # endregion
 
 
-# region FereyAdsBot
-l_ads_btn1 = {
-    'ru': "⛰️ Посты",
-    'en': "⛰️ Posts",
-    'es': "⛰️ Publicaciones",
-    'fr': "⛰️ Messages",
-    'zh': "⛰️ 帖子",
-    'ar': "⛰️ المشاركات",
+# region config
+# region ctranslate_
+l_ctranslate_text = {
+    'ru': "文 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> авто-перевод для <i>исходящих</i> сообщений бота на язык пользователя при /start-запуске бота",
+    'en': "文<b>Click</b> on ✅/☑️ to <b>enable/disable</b> auto-translate for <i>outgoing</i> bot messages into the user's language when /start-starting the bot",
+    'es': "文<b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> la traducción automática de los mensajes <i>salientes</i> del bot al idioma del usuario cuando/inicie el bot",
+    'fr': "文<b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> la traduction automatique des messages <i>sortants</i> du bot dans la langue de l'utilisateur lors du/démarrage du bot",
+    'zh': "文<b>单击</b>✅/☑️<b>启用/禁用</b>在/启动机器人时将<i>传出的</i>机器人消息自动翻译成用户的语言",
+    'ar': "文<b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> الترجمة التلقائية لرسائل الروبوت <i>الصادرة</i> إلى لغة المستخدم عند / بدء تشغيل الروبوت",
 }
-l_ads_btn2 = {
-    'ru': "🌬 Подписка",
-    'en': "🌬 Subscription",
-    'es': "🌬 Suscripción",
-    'fr': "🌬 Abonnement",
-    'zh': "🌬订阅",
-    'ar': "🌬 الاشتراك",
+l_ctranslate_in_on = {
+    'ru': "✅☑Вкл перевод входящих",
+    'en': "✅☑On translation of incoming",
+    'es': "✅☑Sobre la traducción de entrantes",
+    'fr': "✅☑Sur la traduction des entrants",
+    'zh': "✅☑关于来电翻译",
+    'ar': "✅☑على ترجمة واردة",
 }
-l_ads_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для создания креативных постов <b>Ferey</b>\n\n▪️️реклама во всех Ferey-ботах\n▪️️заказ рекламы на канале\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to <i>the landing bot</i> for creating creative постов <b>Ferey</b>\n\n▪️️advertising in all Ferey bots\n▪️️ ordering advertising on the channel\n\n❗️you can also order the development of a chat bot in our Ferey studio",
-    'es': "🌱 {0}, bienvenido <i>al bot de aterrizaje</i> para crear постов creativas <b>Ferey</b>\n\n▪️️publicidad en todos los bots de Ferey\n▪️️solicitando publicidad en el canal\n\n❗️también puedes ordenar el desarrollo de un chatbot en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue dans <i>le bot de débarquement</i> pour la création постов créatives <b>Ferey</b>\n\n▪️️publicité dans tous les bots Ferey\n▪️️commande de publicité sur la chaîne\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎来到<b>Ferey</b>创建创意постов的<i>登陆机器人</i>\n\n▪️️在所有 Ferey 机器人中投放广告\n▪️️ 在频道订购广告\n\n❗️您也可以在以下订购聊天机器人的开发我们的Ferey工作室",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> لإنشاء постов إبداعية <b>Ferey</b>\n\nالإعلان في جميع برامج Ferey\n▪️️ طلب الإعلانات على القناة\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
+l_ctranslate_in_off = {
+    'ru': "☑️☐Выкл перевод входящих",
+    'en': "☑️☐Off incoming translation",
+    'es': "☑️☐Traducción entrante desactivada",
+    'fr': "☑️☐Désactiver la traduction entrante",
+    'zh': "☑️☐关闭传入翻译",
+    'ar': "☑️☐ إيقاف الترجمة الواردة",
 }
-l_subscribe_ads = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [<b>Донат</b> на баланс]:\n▪️рассылка по всем ботам\n▪️редактирование чаевых\n(<i>чтобы указать точную сумму</i>)\n\n👩🏽‍💻 /balance",
-    'en': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [<b>Донат</b> на баланс]:\n▪️возможность сделать рассылку по всем ботам\n▪️измените значение чаевых (<i>чтобы указать точную сумму</i>)\n\n👩🏽‍💻 /balance",
-    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
-    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
-    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
-    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+l_ctranslate_out_on = {
+    'ru': "✅☑Вкл перевод исходящих",
+    'en': "✅☑On outgoing translation",
+    'es': "✅☑Sobre la traducción saliente",
+    'fr': "✅☑Sur la traduction sortante",
+    'zh': "✅☑关于传出翻译",
+    'ar': "✅☑ على الترجمة الصادرة",
 }
-
-l_post_media_ads = {
-    'ru': "✏️ 2. Прикрепи <b>медиа</b> контент: фото/гиф/видео до 5Mb\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
-    'en': "✏️ 2. Attach <b>media</b> content: photo/gif/video up to 5Mb\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
-    'es': "✏️ 2. Adjunte contenido <b>multimedia</b> : foto/gif/video de hasta 5 Mb\n\n( <i>o presione &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
-    'fr': "✏️ 2. Joignez du contenu <b>multimédia</b> : photo/gif/vidéo jusqu&#x27;à 5 Mb\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
-    'zh': "✏️ 2.附加<b>媒体</b>内容：照片/gif/视频最大5Mb\n\n（<i>或按“➡️️/Next”跳过此步骤</i>）",
-    'ar': "✏️ 2. إرفاق محتوى <b>وسائط</b> : صورة / صورة / فيديو بحجم يصل إلى 5 ميغا بايت\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
+l_ctranslate_out_off = {
+    'ru': "☑️☐Выкл перевод исходящих",
+    'en': "☑️☐Off transfer outgoing",
+    'es': "☑️☐Fuera de transferencia saliente",
+    'fr': "☑️☐Off transfert sortant",
+    'zh': "☑️☐关闭转出",
+    'ar': "☑️☐Off تحويل الصادرة",
 }
 # endregion
 
 
-# region FereyPostBot
-l_post_btn1 = {
-    'ru': "⛰️ Посты",
-    'en': "⛰️ Posts",
-    'es': "⛰️ Publicaciones",
-    'fr': "⛰️ Messages",
-    'zh': "⛰️ 帖子",
-    'ar': "⛰️ المشاركات",
-}
-l_post_btn2 = {
-    'ru': "🌬 Подписка",
-    'en': "🌬 Subscription",
-    'es': "🌬 Suscripción",
-    'fr': "🌬 Abonnement",
-    'zh': "🌬订阅",
-    'ar': "🌬 الاشتراك",
-}
-l_post_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для создания креативных постов <b>Ferey</b>\n▪️инлайн-<b>телескопы</b>\n▪️<b>уведомления</b> о нажатиях\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to <i>the landing bot</i> for creating creative постов <b>Ferey</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> para crear постов creativas <b>Ferey</b>\n\n❗️también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> pour créer постов créatifs <b>Ferey</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎使用<b>Ferey</b>创建创意постов的<i>登陆机器人</i>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> لإنشاء постов إبداعية <b>Ferey</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
-}
-l_subscribe_post = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>уведомления</b> о нажатиях\n(<i>ссылка на пользователя</i>)\n\n👩🏽‍💻 /balance",
-    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
-    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
-    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
-    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
-    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
-}
-
-l_post_bot_button_push = {
-    'ru': "👩🏽‍💻 <b>Пользователь</b>: {0} нажал на: [{1}] (пост #<u>{2}</u>)",
-    'en': "👩🏽‍💻 <b>Пользователь</b>: {name} нажал на: [{button}] (пост #<u>{post_id}</u>)",
-    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
-    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
-    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
-    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+# region canswer_
+l_canswer_text = {
+    'ru': "👋🏽 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> режим авто-ответа на текстовые сообщения с помощью нейросети",
+    'en': "👋🏽 <b>Press</b> ✅/☑️ to <b>turn on/off</b> auto-reply to text messages using neural network",
+    'es': "👋🏽 <b>Presione</b> ✅/☑️ para <b>activar/desactivar</b> la respuesta automática a los mensajes de texto usando la red neuronal",
+    'fr': "👋🏽 <b>Appuyez sur</b> ✅/☑️ pour <b>activer/désactiver</b> la réponse automatique aux messages texte à l'aide du réseau neuronal",
+    'zh': "👋🏽<b>按</b>✅/☑️ 使用神经网络<b>打开/关闭</b>自动回复短信",
+    'ar': "👋🏽 <b>اضغط</b> <b>على ✅ / ☑️ لتشغيل / إيقاف</b> الرد التلقائي على الرسائل النصية باستخدام الشبكة العصبية",
 }
 # endregion
 
 
-# region FereyVPNBot
-l_vpn_btn1 = {
-    'ru': "⛰️ VPN",
-    'en': "⛰️ VPN",
-    'es': "⛰️VPN",
-    'fr': "⛰️VPN",
-    'zh': "⛰️ VPN",
-    'ar': "⛰️ VPN",
-}
-l_vpn_btn2 = {
-    'ru': "🌬 Подписка",
-    'en': "🌬 Subscription",
-    'es': "🌬 Suscripción",
-    'fr': "🌬 Abonnement",
-    'zh': "🌬订阅",
-    'ar': "🌬 الاشتراك",
-}
-l_vpn_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> проекта Ferey:\n\n▪️<b>openvpn</b>\n▪️<b>wireguard</b>\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to <i>the landing bot</i> of the Ferey project:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del proyecto Ferey:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du projet Ferey :\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎来到 Ferey 项目的<i>落地机器人</i>：\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص بمشروع Ferey:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey",
+# region cpayment_
+l_cpayment_alert = {
+    'ru': "💳️ Нужно ⚙️Настроить хотя бы один платежный токен",
+    'en': "💳️ You need to ⚙️Set up at least one payment token",
+    'es': "💳️ Debes ⚙️Configurar al menos un token de pago",
+    'fr': "💳️ Vous devez ⚙️Configurer au moins un jeton de paiement",
+    'zh': "💳️您需要⚙️设置至少一个支付令牌",
+    'ar': "💳️ تحتاج إلى إعداد رمز دفع واحد على الأقل",
 }
-l_subscribe_vpn = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
-    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
-    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
-    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
-    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
-    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+l_cpayment_text = {
+    'ru': "💳️ <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> платежи в @{0}-боте\n\n👩🏽‍💻 <b>Текущий</b> платежный токен:\n{1}",
+    'en': "💳️ <b>Click</b> on ✅/☑️ to <b>turn on/off</b> payments in @{0}-bot\n\n👩🏽‍💻 <b>Current</b> payment token:\n{1}",
+    'es': "💳️ <b>Haz clic</b> en ✅/☑️ para <b>activar o desactivar</b> los pagos en @{0}-bot\n\n👩🏽‍💻 Token de pago <b>actual</b> :\n{1}",
+    'fr': "💳️ <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> les paiements dans @{0}-bot\n\n👩🏽‍💻 Jeton de paiement <b>actuel</b> :\n{1}",
+    'zh': "💳️<b>点击</b>✅/☑️ 在@{0}-bot 中<b>打开/关闭</b>支付\n\n👩🏽‍💻<b>当前</b>支付令牌：\n{1}",
+    'ar': "💳️ <b>انقر</b> على ✅ / ☑️ <b>لتشغيل / إيقاف</b> المدفوعات في @ {0} -bot\n\n👩🏽‍💻 رمز الدفع <b>الحالي</b> :\n{1}",
 }
-
-l_vpn_1 = {
-    'ru': "👩🏽‍💻 <b>Open VPN</b>\n\n{0}",
-    'en': "👩🏽‍💻 <b>Open VPN</b>\n\n{0}",
-    'es': "👩🏽‍💻 <b>Abrir VPN</b>\n\n{0}",
-    'fr': "👩🏽‍💻 <b>Ouvrez le VPN</b>\n\n{0}",
-    'zh': "👩🏽‍💻<b>打开 VPN</b>\n\n{0}",
-    'ar': "👩🏽‍💻 <b>افتح VPN</b>\n\n{0}",
+l_cpayment_token = {
+    'ru': "💳️ <b>Вставь</b> платежный токен, полученный из @BotFather-бота\n\n👩🏽‍💻 <b>Например</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 <b>Текущий</b> токен:\n{0}",
+    'en': "💳️ <b>Insert</b> payment token received from @BotFather -bot\n\n👩🏽‍💻 <b>For example</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 <b>Current</b> token:\n{0}",
+    'es': "💳️ <b>Inserte</b> el token de pago recibido de @BotFather -bot\n\n👩🏽‍💻 <b>Por ejemplo,</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 Token <b>actual</b> :\n{0}",
+    'fr': "💳️ <b>Insérez</b> le jeton de paiement reçu de @BotFather -bot\n\n👩🏽‍💻 <b>Par exemple</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 Jeton <b>actuel</b> :\n{0}",
+    'zh': "💳️<b>插入</b>从@BotFather -bot 收到的支付令牌\n\n👩🏽‍💻<b>例如</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻<b>当前</b>令牌：\n{0}",
+    'ar': "💳️ <b>أدخل</b> رمز الدفع المستلم من @BotFather -bot\n\n👩🏽‍💻 <b>على سبيل المثال</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 الرمز <b>المميز الحالي</b> :\n{0}",
 }
-l_vpn_2 = {
-    'ru': "👩🏽‍💻 <b>Wire Guard</b>\n\n{0}",
-    'en': "👩🏽‍💻 <b>Wire Guard</b>\n\n{0}",
-    'es': "👩🏽‍💻 <b>Protector de alambre</b>\n\n{0}",
-    'fr': "👩🏽‍💻 <b>Fil de protection</b>\n\n{0}",
-    'zh': "👩🏽‍💻<b>线卫士</b>\n\n{0}",
-    'ar': "👩🏽‍💻 <b>واقي الأسلاك</b>\n\n{0}",
+l_cpayment_done = {
+    'ru': "💳️ <b>Готово!</b>\n\n👩🏽‍💻 <b>Текущий</b> платежный токен для @{0}-бота:\n\n{1}",
+    'en': "💳️ <b>Done!</b>\n\n👩🏽‍💻 <b>Current</b> payment token for @{0}-bot:\n\n{1}",
+    'es': "💳️ <b>Listo!</b>\n\n👩🏽‍💻 Token de pago <b>actual</b> para @{0}-bot:\n\n{1}",
+    'fr': "💳️ <b>C&#x27;est fait !</b>\n\n👩🏽‍💻 Jeton de paiement <b>actuel</b> pour @{0}-bot :\n\n{1}",
+    'zh': "💳️<b>完成！</b>\n\n👩🏽‍💻 @{0}-bot 的<b>当前</b>支付令牌：\n\n{1}",
+    'ar': "💳️ <b>انتهى!</b>\n\n👩🏽‍💻 رمز الدفع <b>الحالي</b> لـ @ {0} -bot:\n\n{1}",
 }
 # endregion
 
 
-# region FereyToolsBot
-l_tools_btn1 = {
-    'ru': "⛰️ Инструменты",
-    'en': "⛰️ Tools",
-    'es': "⛰️ Herramientas",
-    'fr': "⛰️ Outils",
-    'zh': "⛰️ 工具",
-    'ar': "⛰️ أدوات",
-}
-l_tools_btn2 = {
-    'ru': "🌬 Подписка",
-    'en': "🌬 Subscription",
-    'es': "🌬 Suscripción",
-    'fr': "🌬 Abonnement",
-    'zh': "🌬订阅",
-    'ar': "🌬 الاشتراك",
-}
-l_tools_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> Telegram-инструментов:\n\n▪️<b>преобразование</b> контента\n▪️<b>получение</b> информации о сообщ\n▪️<b>удаление</b> фона\n▪️<b>конвертация</b> в телескопы\n▪️<b>сообщение</b> 0-длины\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to <i>the landing bot</i> of Telegram инструментов :\n\n▪️ content <b>conversion</b>\n▪️ <b>getting</b> information about the message\n\n❗️you can also order the development of a chat bot in our studio Ferey",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> de инструментов de Telegram:\n\n▪️ <b>conversión</b> de contenido\n▪️ <b>obtener</b> información sobre el mensaje\n\n❗️también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue dans <i>le landing bot</i> des инструментов Telegram :\n\n▪️ <b>conversion</b> de contenu\n▪️ <b>obtenir</b> des informations sur le message\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎使用 Telegram инструментов的<i>登陆机器人</i>：\n\n▪️ 内容<b>转换</b>\n▪️<b>获取</b>有关消息的信息\n\n❗️您也可以在我们的工作室Ferey订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص инструментов Telegram:\n\n▪️ <b>تحويل</b> المحتوى\n▪️ <b>الحصول على</b> معلومات حول الرسالة\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
+# region cintegration_
+l_cintegration_alert = {
+    'ru': "🗝️ Нужно ⚙️Настроить ССЫЛКУ доступа",
+    'en': "🗝️ You need to ⚙️Set up an access link",
+    'es': "🗝️ Debes ⚙️Configurar un enlace de acceso",
+    'fr': "🗝️ Vous devez ⚙️Configurer un lien d'accès",
+    'zh': "🗝️您需要⚙️设置访问链接",
+    'ar': "🗝️ تحتاج إلى إعداد ارتباط وصول",
 }
-l_subscribe_tools = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
-    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
-    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
-    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
-    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
-    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+l_cintegration_text = {
+    'ru': "🗝️ <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> интеграцию базы пользователей с <i><b>google</b>-crm/<b>airtable</b>-crm</i>\n\n👩🏽‍💻 Например, опция [<b>{0}</b>] означает возможность интеграции базы пользователей с <i>google-crm</i>",
+    'en': "🗝️ <b>Click</b> on ✅/☑️ to <b>enable/disable</b> integration of user base with <i><b>google</b> -crm/ <b>airtable</b> -crm</i>\n\n👩🏽‍💻 For example, option [<b>{0}</b>] means the ability to integrate user base with <i>google-crm</i>",
+    'es': "🗝️ <b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> la integración de la base de usuarios con <i><b>google</b> -crm/ <b>airtable</b> -crm</i>\n\n👩🏽‍💻 Por ejemplo, la opción [<b>{0}</b>] significa la capacidad de integrar la base de usuarios con <i>google-crm</i>",
+    'fr': "🗝️ <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> l&#x27;intégration de la base d&#x27;utilisateurs avec <i><b>google</b> -crm/ <b>airtable</b> -crm</i>\n\n👩🏽‍💻 Par exemple, l&#x27;option [<b>{0}</b>] signifie la possibilité d&#x27;intégrer la base d&#x27;utilisateurs avec <i>google-crm</i>",
+    'zh': "🗝️<b>点击</b>✅/☑️<b>启用/禁用</b>用户群与<i><b>google</b> -crm/ <b>airtable</b> -crm</i>\n\n👩🏽‍💻 例如，选项 [<b>{0}</b>] 表示能够将用户群与<i>google-crm</i>集成",
+    'ar': "🗝️ <b>انقر</b> على ✅ / ☑️ <b>لتمكين / تعطيل</b> تكامل قاعدة المستخدمين مع <i><b>google</b> -crm / <b>airtable</b> -crm</i>\n\n👩🏽‍💻 على سبيل المثال ، الخيار [<b>{0}</b>] يعني القدرة على تكامل قاعدة المستخدمين مع <i>google-crm</i>",
 }
 
-l_image_text = {
-    'ru': "👩🏽‍💻 <b>Выбери</b> инструменты для преобразования <i>изображения</i> в",
-    'en': "👩🏽‍💻 <b>Choose</b> tools to convert <i>your image</i> to",
-    'es': "👩🏽‍💻 <b>Elija</b> herramientas para convertir <i>su imagen</i> a",
-    'fr': "👩🏽‍💻 <b>Choisissez</b> des outils pour convertir <i>votre image</i> en",
-    'zh': "👩🏽‍💻<b>选择</b>将<i>图像</i>转换为的工具",
-    'ar': "👩🏽‍💻 <b>اختر</b> أدوات لتحويل <i>صورتك</i> إلى",
-}
-l_image_sticker = {
-    'ru': "🌌 стикер",
-    'en': "🌌 sticker",
-    'es': "🌌 pegatina",
-    'fr': "🌌 autocollant",
-    'zh': "🌌 贴纸",
-    'ar': "🌌 ملصق",
-}
-l_image_jpg = {
-    'ru': "🏞️ jpg",
-    'en': "🏞️ jpg",
-    'es': "🏞️ jpg",
-    'fr': "🏞️jpg",
-    'zh': "🏞️ jpg",
-    'ar': "🏞️ jpg",
-}
-l_image_png = {
-    'ru': "🌁 png",
-    'en': "🌁 png",
-    'es': "🌁 png",
-    'fr': "🌁 png",
-    'zh': "🌁 PNG",
-    'ar': "🌁 ينغ",
-}
-l_image_rbg = {
-    'ru': "🙌🏽 удалить фон",
-    'en': "🙌🏽 remove background",
-    'es': "🙌🏽 eliminar fondo",
-    'fr': "🙌🏽 supprimer l'arrière-plan",
-    'zh': "🙌🏽 删除背景",
-    'ar': "🙌🏽 إزالة الخلفية",
-}
-l_image_mp4 = {
-    'ru': "🎥 mp4",
-    'en': "🎥 mp4",
-    'es': "🎥 mp4",
-    'fr': "🎥 mp4",
-    'zh': "🎥 mp4",
-    'ar': "🎥 mp4",
-}
-l_image_album = {
-    'ru': "9️⃣ album⁹",
-    'en': "9️⃣ album⁹",
-    'es': "9️⃣ álbum⁹",
-    'fr': "9️⃣album⁹",
-    'zh': "9️⃣专辑⁹",
-    'ar': "9️⃣ البوم⁹",
-}
-l_image_thumb = {
-    'ru': "🖼️ thumb",
-    'en': "🖼️ thumb",
-    'es': "🖼️ pulgar",
-    'fr': "🖼️ pouce",
-    'zh': "🖼️拇指",
-    'ar': "🖼️ إبهام",
-}
-l_image_descpic = {
-    'ru': "⿴ Bot Desc Pic",
-    'en': "⿴ Bot Desc Pic",
-    'es': "⿴ Foto de descripción del bot",
-    'fr': "⿴ Image de description du robot",
-    'zh': "⿴ 机器人描述图片",
-    'ar': "⿴ بوت ديسك بيك",
-}
-l_image_sticker_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в стикер",
-    'en': "👩🏽‍💻 <b>Attach</b> a photo to convert into a sticker",
-    'es': "👩🏽‍💻 <b>Adjunta</b> una foto para convertirla en una pegatina",
-    'fr': "👩🏽‍💻 <b>Joignez</b> une photo à convertir en autocollant",
-    'zh': "👩🏽‍💻<b>附上</b>照片以转换为贴纸",
-    'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى ملصق",
-}
-l_image_jpg_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в jpg",
-    'en': "👩🏽‍💻 <b>Attach</b> a photo to convert to jpg",
-    'es': "👩🏽‍💻 <b>Adjunta</b> una foto para convertir a jpg",
-    'fr': "👩🏽‍💻 <b>Joindre</b> une photo à convertir en jpg",
-    'zh': "👩🏽‍💻<b>附上</b>照片以转换为jpg",
-    'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى jpg",
-}
-l_image_png_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в png",
-    'en': "👩🏽‍💻 <b>Attach</b> a photo to convert to png",
-    'es': "👩🏽‍💻 <b>Adjunta</b> una foto para convertir a png",
-    'fr': "👩🏽‍💻 <b>Joindre</b> une photo à convertir en png",
-    'zh': "👩🏽‍💻<b>附上</b>要转换为png的照片",
-    'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى png",
-}
-l_image_rbg_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для удаления фона",
-    'en': "👩🏽‍💻 <b>Attach</b> photo to remove background",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> foto para eliminar fondo",
-    'fr': "👩🏽‍💻 <b>Joindre</b> une photo pour supprimer l'arrière-plan",
-    'zh': "👩🏽‍💻<b>附加</b>照片以删除背景",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> صورة لإزالة الخلفية",
-}
-l_image_mp4_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в mp4 (Telegram-аватарку)",
-    'en': "👩🏽‍💻 <b>Attach</b> a photo to convert to mp4 (Telegram avatar)",
-    'es': "👩🏽‍💻 <b>Adjunta</b> una foto para convertir a mp4 (Avatar de Telegram)",
-    'fr': "👩🏽‍💻 <b>Joindre</b> une photo à convertir en mp4 (avatar Telegram)",
-    'zh': "👩🏽‍💻<b>附上</b>照片以转换为mp4（电报头像）",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> صورة لتحويلها إلى mp4 (Telegram avatar)",
+l_cintegration_google_on = {
+    'ru': "✅☑Вкл google-crm",
+    'en': "✅☑Includes google-crm",
+    'es': "✅☑Incluye google-crm",
+    'fr': "✅☑Inclut google-crm",
+    'zh': "✅☑包括谷歌客户关系管理",
+    'ar': "✅☑ يشمل google-crm",
 }
-l_image_album_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в альбом из 9 частей",
-    'en': "👩🏽‍💻 <b>Attach</b> a photo to transform into a 9-part album",
-    'es': "👩🏽‍💻 <b>Adjunta</b> una foto para transformarla en un álbum de 9 partes",
-    'fr': "👩🏽‍💻 <b>Joignez</b> une photo pour la transformer en un album en 9 parties",
-    'zh': "👩🏽‍💻<b>附上</b>照片，变身为9张相册",
-    'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى ألبوم مكون من 9 أجزاء",
+l_cintegration_google_off = {
+    'ru': "☑️☐Выкл google-crm",
+    'en': "☑️☐Выкл google-crm",
+    'es': "☑️☐Выкл google-crm",
+    'fr': "☑️☐Выкл google-crm",
+    'zh': "☑️☐Выкл 谷歌客户关系管理",
+    'ar': "☑️☐Выкл google-crm",
 }
-l_image_thumb_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в thumb-nail-иконку (160x160)",
-    'en': "👩🏽‍💻 <b>Attach</b> a photo to convert to a thumb-nail icon (160x160)",
-    'es': "👩🏽‍💻 <b>Adjunte</b> una foto para convertirla en un icono de miniatura (160x160)",
-    'fr': "👩🏽‍💻 <b>Joignez</b> une photo à convertir en icône de vignette (160x160)",
-    'zh': "👩🏽‍💻<b>附加</b>照片以转换为缩略图图标 (160x160)",
-    'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى رمز مسمار الإبهام (160 × 160)",
+l_cintegration_airtable_on = {
+    'ru': "✅☑Вкл airtable-crm",
+    'en': "✅☑Includes airtable-crm",
+    'es': "✅☑Incluye airtable-crm",
+    'fr': "✅☑Comprend airtable-crm",
+    'zh': "✅☑包括 airtable-crm",
+    'ar': "✅☑ يشمل airtable-crm",
 }
-l_image_descpic_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в формат, необходимый для установки Description Picture для бота в @BotFather (640x360)",
-    'en': "👩🏽‍💻 <b>Attach</b> a photo to convert to the format required to set the Description Picture for the bot in @BotFather (640x360)",
-    'es': "👩🏽‍💻 <b>Adjunte</b> una foto para convertir al formato requerido para configurar la imagen de descripción para el bot en @BotFather (640x360)",
-    'fr': "👩🏽‍💻 <b>Joignez</b> une photo à convertir au format requis pour définir l'image de description du bot dans @BotFather (640x360)",
-    'zh': "👩🏽‍💻<b>附上</b>照片以转换为在@BotFather中为机器人设置描述图片所需的格式（640x360）",
-    'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى التنسيق المطلوب لتعيين وصف الصورة للروبوت في @BotFather (640x360)",
+l_cintegration_airtable_off = {
+    'ru': "☑️☐Выкл airtable-crm",
+    'en': "☑️☐Выкл airtable-crm",
+    'es': "☑️☐Выкл airtable-crm",
+    'fr': "☑️☐Выкл airtable-crm",
+    'zh': "☑️☐Выкл airtable-crm",
+    'ar': "☑️☐Выкл airtable-crm",
 }
 
-l_gif_text = {
-    'ru': "👩🏽‍💻 <b>Выбери</b> инструменты для преобразования <i>гиф</i> в",
-    'en': "👩🏽‍💻 <b>Choose</b> tools to convert <i>GIF</i> to",
-    'es': "👩🏽‍💻 <b>Elija</b> herramientas para convertir <i>GIF</i> a",
-    'fr': "👩🏽‍💻 <b>Choisissez</b> des outils pour convertir <i>GIF</i> en",
-    'zh': "👩🏽‍💻<b>选择将</b><i>GIF</i>转换为的工具",
-    'ar': "👩🏽‍💻 <b>اختر</b> أدوات لتحويل <i>GIF</i> إلى",
-}
-l_gif_mp4 = {
-    'ru': "🎥 mp4",
-    'en': "🎥 mp4",
-    'es': "🎥 mp4",
-    'fr': "🎥 mp4",
-    'zh': "🎥 mp4",
-    'ar': "🎥 mp4",
-}
-l_gif_thumb = {
-    'ru': "🖼️ thumb-nail",
-    'en': "🖼️ thumb-nail",
-    'es': "🖼️ miniatura",
-    'fr': "🖼️ ongle du pouce",
-    'zh': "🖼️ 缩略图",
-    'ar': "🖼️ الإبهام",
-}
-l_gif_descgif = {
-    'ru': "⿴ Bot Desc Gif",
-    'en': "⿴ Bottom Desc Gif",
-    'es': "⿴ Gif de descripción inferior",
-    'fr': "⿴ Bas Desc Gif",
-    'zh': "⿴ 底部描述 Gif",
-    'ar': "⿴ أسفل Desc Gif",
-}
-l_gif_mp4_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> гиф для преобразования в mp4",
-    'en': "👩🏽‍💻 <b>Attach</b> GIF to convert to mp4",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> GIF para convertir a mp4",
-    'fr': "👩🏽‍💻 <b>Joindre</b> GIF pour convertir en mp4",
-    'zh': "👩🏽‍💻<b>附加</b>GIF 以转换为 mp4",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> GIF للتحويل إلى mp4",
+l_cintegration_google = {
+    'ru': "🗝️ <b>Вставь ссылку</b> на пустую google-таблицу (<i>с открытым доступом для редактирования</i>) для интеграции с базой пользователей @{0}-бота\n\n👩🏽‍💻 <b>Например</b>, https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 <b>Текущая</b> ссылка:\n{1}",
+    'en': "🗝️ <b>Insert a link</b> to an empty google spreadsheet ( <i>with open access for editing</i> ) to integrate with the @{0}-bot user base\n\n👩🏽‍💻 <b>For example</b> , https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 <b>Current</b> URL:\n{1}",
+    'es': "🗝️ <b>Inserta un enlace</b> a una hoja de cálculo de Google vacía ( <i>con acceso abierto para editar</i> ) para integrarla con la base de usuarios de @{0}-bot\n\n👩🏽‍💻 <b>Por ejemplo</b> , https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 URL <b>actual</b> :\n{1}",
+    'fr': "🗝️ <b>Insérez un lien</b> vers une feuille de calcul Google vide ( <i>avec accès ouvert pour modification</i> ) à intégrer à la base d&#x27;utilisateurs @{0}-bot\n\n👩🏽‍💻 <b>Par exemple</b> , https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 URL <b>actuelle</b> :\n{1}",
+    'zh': "🗝️<b>插入指向空谷歌电子表格的链接</b>（<i>开放编辑权限</i>）以与@{0}-bot 用户群集成\n\n👩🏽‍💻<b>例如</b>，https: https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻<b>当前</b>网址：\n{1}",
+    'ar': "🗝️ <b>أدخل رابطًا</b> إلى جدول بيانات google فارغ ( <i>مع وصول مفتوح للتعديل</i> ) للتكامل مع @ {0} -bot user base\n\n👩🏽‍💻 <b>على سبيل المثال</b> ، https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 عنوان URL <b>الحالي</b> :\n{1}",
 }
-l_gif_thumb_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> гиф для преобразования в thumb-nail-иконку (160x160)",
-    'en': "👩🏽‍💻 <b>Attach</b> GIF to convert to thumb-nail icon (160x160)",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> GIF para convertir en icono de miniatura (160x160)",
-    'fr': "👩🏽‍💻 <b>Attachez</b> GIF pour convertir en icône de vignette (160x160)",
-    'zh': "👩🏽‍💻<b>附加</b>GIF 以转换为缩略图图标 (160x160)",
-    'ar': "👩🏽‍💻 <b>أرفق</b> ملف GIF للتحويل إلى أيقونة مسمار الإبهام (160 × 160)",
+l_cintegration_airtable = {
+    'ru': "🗝️ <b>Вставь ссылку</b> на пустую airtable-таблицу (<i>с открытым доступом для редактирования и любого e-mail</i>) для интеграции с базой пользователей @{0}-бота\n\n👩🏽‍💻 <b>Например</b>, https://airtable.com/invite/l?inviteId=inv4VGM&inviteToken=f1d31f9aba6b&utm_medium=email\n\n👩🏽‍💻 <b>Текущая</b> ссылка:\n{1}",
+    'en': "🗝️ <b>Insert a link</b> to an empty airtable-table ( <i>with open access for editing and any e-mail</i> ) for integration with the @{0}-bot user base\n\n👩🏽‍💻 <b>For example</b> , https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email\n\n👩🏽‍💻 <b>Current</b> URL:\n{1}",
+    'es': "🗝️ <b>Inserte un enlace</b> a una mesa de aire vacía ( <i>con acceso abierto para editar y cualquier correo electrónico</i> ) para la integración con la base de usuarios de @{0}-bot\n\n👩🏽‍💻 <b>Por ejemplo</b> , https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email\n\n👩🏽‍💻 URL <b>actual</b> :\n{1}",
+    'fr': "🗝️ <b>Insérez un lien</b> vers une table airtable vide ( <i>avec un accès ouvert pour l&#x27;édition et tout e-mail</i> ) pour l&#x27;intégration avec la base d&#x27;utilisateurs @{0}-bot\n\n👩🏽‍💻 <b>Par exemple</b> , https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email\n\n👩🏽‍💻 URL <b>actuelle</b> :\n{1}",
+    'zh': "🗝️<b>插入一个指向空的 airtable-table 的链接</b>（<i>具有编辑和任何电子邮件的开放访问权限</i>）以与 @{0}-bot 用户群集成\n\n👩🏽‍💻<b>例如</b>， https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email\n\n👩🏽‍💻<b>当前</b>网址：\n{1}",
+    'ar': "🗝️ <b>أدخل ارتباطًا</b> إلى جدول airtable فارغ ( <i>مع وصول مفتوح للتحرير وأي بريد إلكتروني</i> ) للتكامل مع @ {0} -bot user base\n\n👩🏽‍💻 <b>على سبيل المثال</b> ، https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email <b>؟</b>",
 }
-l_gif_descgif_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> гиф для преобразования в формат, необходимый для установки Description Gif для бота в @BotFather (640x360). После формирования GIF нажимаем на нее через <u>мобильное</u> приложение (ожидая загрузки), далее Поделиться - приложение Telegram - @BotFather",
-    'en': "👩🏽‍💻 <b>Attach</b> a gif to convert to the format needed to set the Description Gif for the bot to @BotFather (640x360). After generating a GIF, click on it through <u>the mobile</u> application (waiting for download), then Share - Telegram application - @BotFather",
-    'es': "👩🏽‍💻 <b>Adjunte</b> un gif para convertir al formato necesario para configurar el GIF de descripción para el bot en @BotFather (640x360). Después de generar un GIF, haga clic en él a través de <u>la aplicación móvil</u> (en espera de descarga), luego Compartir - Aplicación Telegram - @BotFather",
-    'fr': "👩🏽‍💻 <b>Joignez</b> un gif à convertir au format nécessaire pour définir le gif de description du bot sur @BotFather (640x360). Après avoir généré un GIF, cliquez dessus via <u>l&#x27;application mobile</u> (en attente de téléchargement), puis Partager - Application Telegram - @BotFather",
-    'zh': "👩🏽‍💻<b>附加</b>一个 gif 以转换为将机器人的描述 Gif 设置为@BotFather (640x360) 所需的格式。生成GIF后，通过<u>手机</u>应用点击（等待下载），然后Share - Telegram application - @BotFather",
-    'ar': "👩🏽‍💻 <b>أرفق</b> صورة gif للتحويل إلى التنسيق المطلوب لتعيين Description Gif للبوت إلى @BotFather (640x360). بعد إنشاء ملف GIF ، اضغط عليه من خلال تطبيق <u>الهاتف المحمول</u> (في انتظار التنزيل) ، ثم شارك - تطبيق Telegram @BotFather",
+l_cintegration_done = {
+    'ru': "🗝️ <b>Готово!</b>\n\n👩🏽‍💻 <b>Текущая</b> ссылка:\n{0}",
+    'en': "🗝️ <b>Done!</b>\n\n👩🏽‍💻 <b>Current</b> URL:\n{0}",
+    'es': "🗝️ <b>Listo!</b>\n\n👩🏽‍💻 URL <b>actual</b> :\n{0}",
+    'fr': "🗝️ <b>C&#x27;est fait !</b>\n\n👩🏽‍💻 URL <b>actuelle</b> :\n{0}",
+    'zh': "🗝️<b>完成！</b>\n\n👩🏽‍💻<b>当前</b>网址：\n{0}",
+    'ar': "🗝️ <b>انتهى!</b>\n\n👩🏽‍💻 عنوان URL <b>الحالي</b> :\n{0}",
 }
+# endregion
 
-l_video_text = {
-    'ru': "👩🏽‍💻 <b>Выбери</b> инструменты для преобразования <i>видео</i> в",
-    'en': "👩🏽‍💻 <b>Choose</b> tools to convert <i>video</i> to",
-    'es': "👩🏽‍💻 <b>Elija</b> herramientas para convertir <i>videos</i> a",
-    'fr': "👩🏽‍💻 <b>Choisissez</b> des outils pour convertir <i>la vidéo</i> en",
-    'zh': "👩🏽‍💻<b>选择将</b><i>视频</i>转换为的工具",
-    'ar': "👩🏽‍💻 <b>اختر</b> أدوات لتحويل <i>الفيديو</i> إلى",
-}
-l_video_videonote = {
-    'ru': "⚫️ телескоп",
-    'en': "⚫️ telescope",
-    'es': "⚫️ telescopio",
-    'fr': "⚫️ télescope",
-    'zh': "⚫️望远镜",
-    'ar': "⚫️ تلسكوب",
-}
-l_video_mp3 = {
-    'ru': "▶️ mp3",
-    'en': "▶️ mp3",
-    'es': "▶️ mp3",
-    'fr': "▶️ mp3",
-    'zh': "▶️ mp3",
-    'ar': "▶️ mp3",
-}
-l_video_mp4 = {
-    'ru': "🎥 mp4",
-    'en': "🎥 mp4",
-    'es': "🎥 mp4",
-    'fr': "🎥 mp4",
-    'zh': "🎥 mp4",
-    'ar': "🎥 mp4",
-}
-l_video_album = {
-    'ru': "9️⃣ album⁹",
-    'en': "9️⃣ album⁹",
-    'es': "9️⃣ álbum⁹",
-    'fr': "9️⃣album⁹",
-    'zh': "9️⃣专辑⁹",
-    'ar': "9️⃣ البوم⁹",
-}
-l_video_thumb = {
-    'ru': "🖼️ thumb-nail",
-    'en': "🖼️ thumb-nail",
-    'es': "🖼️ miniatura",
-    'fr': "🖼️ ongle du pouce",
-    'zh': "🖼️ 缩略图",
-    'ar': "🖼️ الإبهام",
-}
-l_video_gif = {
-    'ru': "📽️ gif",
-    'en': "📽️ gif",
-    'es': "📽️ gif",
-    'fr': "📽️ gif",
-    'zh': "📽️动图",
-    'ar': "📽️ gif",
-}
-l_video_transcribe = {
-    'ru': "🗣️ транскрибация",
-    'en': "🗣️ transcription",
-    'es': "🗣️ transcripción",
-    'fr': "🗣️ retranscription",
-    'zh': "🗣️ 转录",
-    'ar': "🗣️ النسخ",
-}
-l_video_videonote_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> видео для преобразования в телескоп (круглую видео-заметку)",
-    'en': "👩🏽‍💻 <b>Attach</b> a video to transform into a telescope (round video note)",
-    'es': "👩🏽‍💻 <b>Adjunta</b> un video para transformarte en telescopio (nota de video redonda)",
-    'fr': "👩🏽‍💻 <b>Joindre</b> une vidéo pour se transformer en télescope (note vidéo ronde)",
-    'zh': "👩🏽‍💻<b>附上</b>变身望远镜的视频（圆形视频笔记）",
-    'ar': "<b>أرفق</b> مقطع فيديو لتحويله إلى تلسكوب (ملاحظة فيديو مستديرة)",
-}
-l_video_mp3_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> видео для преобразования в mp3-аудио",
-    'en': "👩🏽‍💻 <b>Attach</b> video to convert to mp3 audio",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> video para convertir a audio mp3",
-    'fr': "👩🏽‍💻 <b>Joindre</b> une vidéo pour la convertir en audio mp3",
-    'zh': "👩🏽‍💻<b>附加</b>视频以转换为 mp3 音频",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> الفيديو لتحويله إلى صوت mp3",
-}
-l_video_mp4_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> видео для преобразования в mp4",
-    'en': "👩🏽‍💻 <b>Attach</b> video to convert to mp4",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> video para convertir a mp4",
-    'fr': "👩🏽‍💻 <b>Joindre</b> une vidéo à convertir en mp4",
-    'zh': "👩🏽‍💻<b>附上</b>视频以转换为mp4",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> الفيديو لتحويله إلى mp4",
-}
-l_video_album_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> видео для преобразования в альбом из 9 частей",
-    'en': "👩🏽‍💻 <b>Attach</b> video to convert into 9 part album",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> video para convertir en álbum de 9 partes",
-    'fr': "👩🏽‍💻 <b>Joindre</b> une vidéo à convertir en album en 9 parties",
-    'zh': "👩🏽‍💻<b>附上</b>视频以转换成 9 部分专辑",
-    'ar': "👩🏽‍💻 <b>أرفق مقطع</b> فيديو لتحويله إلى ألبوم مكون من 9 أجزاء",
-}
-l_video_thumb_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> видео для преобразования в thumb-nail-иконку (160x160)",
-    'en': "👩🏽‍💻 <b>Attach</b> video to convert to thumbnail (160x160)",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> video para convertirlo en miniatura (160x160)",
-    'fr': "👩🏽‍💻 <b>Joindre</b> une vidéo à convertir en vignette (160x160)",
-    'zh': "👩🏽‍💻<b>附加</b>视频以转换为缩略图 (160x160)",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> فيديو للتحويل إلى صورة مصغرة (160 × 160)",
-}
-l_video_gif_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> видео для преобразования в гиф",
-    'en': "👩🏽‍💻 <b>Attach</b> video to convert to GIF",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> video para convertir a GIF",
-    'fr': "👩🏽‍💻 <b>Joindre</b> une vidéo à convertir en GIF",
-    'zh': "👩🏽‍💻<b>附加</b>视频以转换为 GIF",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> الفيديو لتحويله إلى GIF",
-}
-l_video_transcribe_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> круглую видео для преобразования в текст",
-    'en': "👩🏽‍💻 <b>Attach</b> round video to convert to text",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> video redondo para convertir a texto",
-    'fr': "👩🏽‍💻 <b>Attachez</b> une vidéo ronde pour la convertir en texte",
-    'zh': "👩🏽‍💻<b>附上</b>圆形视频以转换为文本",
-    'ar': "👩🏽‍💻 <b>أرفق</b> مقطع فيديو مستديرًا للتحويل إلى نص",
-}
 
-l_audio_text = {
-    'ru': "👩🏽‍💻 <b>Выбери</b> инструменты для преобразования <i>audio</i> в",
-    'en': "👩🏽‍💻 <b>Choose</b> tools to convert <i>audio</i> to",
-    'es': "👩🏽‍💻 <b>Elija</b> herramientas para convertir <i>audio</i> a",
-    'fr': "👩🏽‍💻 <b>Choisissez</b> des outils pour convertir <i>l&#x27;audio</i> en",
-    'zh': "👩🏽‍💻<b>选择</b>将<i>音频</i>转换为的工具",
-    'ar': "👩🏽‍💻 <b>اختر</b> أدوات لتحويل <i>الصوت</i> إلى",
-}
-l_audio_mp3 = {
-    'ru': "▶️ mp3-аудио",
-    'en': "▶️ mp3-audio",
-    'es': "▶️ audio mp3",
-    'fr': "▶️ audio mp3",
-    'zh': "▶️ mp3音频",
-    'ar': "▶ ️ mp3 الصوت",
-}
-l_audio_ogg = {
-    'ru': "🎤 ogg-голосовое",
-    'en': "🎤 ogg-voice",
-    'es': "🎤 voz ogg",
-    'fr': "🎤 ogg-voix",
-    'zh': "🎤 ogg 声音",
-    'ar': "🎤 ogg-voice",
-}
-l_audio_transcribe = {
-    'ru': "🗣️ транскрибация",
-    'en': "🗣️ transcription",
-    'es': "🗣️ transcripción",
-    'fr': "🗣️ retranscription",
-    'zh': "🗣️ 转录",
-    'ar': "🗣️ النسخ",
+# region cnotification_
+l_cnotification_text = {
+    'ru': "💬 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> оповещения о <i><b>/start-stop</b> запуске/блокировке бота пользователем и попадании пользователя в <b>/ban</b>-список/<b>нажатии</b> на кнопки пользователем/<b>диалоге</b> с администраторами/<b>всех</b> действиях пользователя</i>\n\n👩🏽‍💻 Например, опция [<b>{0}</b>] означает показ сообщений от пользователя администраторам бота (/admin) с возможностью реплай-ответа на сообщения",
+    'en': "💬 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> notifications about <i><b>/start-stop</b> launching/blocking the bot by the user and getting the user into the <b>/ban</b> -list/ <b>pressing</b> buttons by the user/ <b>dialog</b> with administrators/ <b>all</b> user actions</i>\n\n👩🏽‍💻 For example, the option [<b>{0}</b>] means показ messages from the user to bot administrators (/admin) with the ability to replay response to messages",
+    'es': "💬 <b>Haga clic</b> en ✅/☑️ para <b>activar/desactivar</b> las notificaciones sobre <i><b>/iniciar y detener</b> el lanzamiento/bloqueo del bot por parte del usuario y colocar al usuario en la <b>/lista de prohibición</b> / <b>pulsar</b> botones por parte del usuario/ <b>diálogo</b> con los administradores/ <b>todas</b> las acciones del usuario \</i> n\n👩🏽‍💻 Por ejemplo, la opción [<b>{0}</b>] significa показ los mensajes del usuario a los administradores del bot (/admin) con la capacidad de reproducir la respuesta a los mensajes.",
+    'fr': "💬 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> les notifications sur <i><b>/start-stop</b> lancer/bloquer le bot par l&#x27;utilisateur et faire entrer l&#x27;utilisateur dans la <b>/banni</b> -liste/ <b>appuyer sur</b> les boutons par l&#x27;utilisateur/ <b>dialogue</b> avec les administrateurs/ <b>toutes</b> les actions de l&#x27;utilisateur \</i> n\n👩🏽‍💻 Par exemple, l&#x27;option [<b>{0}</b>] signifie показ les messages de l'utilisateur aux administrateurs du bot (/admin) avec la possibilité de rejouer la réponse aux messages",
+    'zh': "💬<b>单击</b>✅/☑️ 以<b>打开/关闭</b><i>关于<b>/start-stop</b>启动/阻止用户的机器人并让用户进入<b>/ban</b>列表/用户<b>按下</b>按钮/与管理员<b>对话</b>/<b>所有</b>用户操作的通知 \</i> n\n👩🏽‍💻 例如，选项 [<b>{0}</b>] 表示将用户的消息показ给机器人管理员 (/admin)，并能够重播对消息的响应",
+    'ar': "💬 <b>انقر</b> فوق ✅ / ☑️ <b>لتشغيل / إيقاف تشغيل</b> <i>الإشعارات حول <b>/ بدء - إيقاف</b> تشغيل / حظر الروبوت من قبل المستخدم وإدخال المستخدم في أزرار <b>/ قائمة الحظر</b> / <b>الضغط</b> بواسطة المستخدم / <b>الحوار</b> مع المسؤولين / <b>جميع</b> إجراءات المستخدم \</i> n\n👩🏽‍💻 على سبيل المثال ، الخيار [<b>{0}</b>] يعني показ الرسائل من المستخدم إلى المشرفين (/ admin) مع إمكانية إعادة الرد على الرسائل",
 }
-l_audio_mp3_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> голосовое для преобразования в mp3",
-    'en': "👩🏽‍💻 <b>Attach</b> voice to convert to mp3",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> voz para convertir a mp3",
-    'fr': "👩🏽‍💻 <b>Joindre</b> la voix pour convertir en mp3",
-    'zh': "👩🏽‍💻<b>附上</b>语音转换成mp3",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> الصوت للتحويل إلى mp3",
+l_cnotification_start_on = {
+    'ru': "✅☑Вкл /start-stop-/ban",
+    'en': "✅☑On /start-stop-/ban",
+    'es': "✅☑Activar/iniciar-detener-/prohibir",
+    'fr': "✅☑On /start-stop-/interdiction",
+    'zh': "✅☑开/启-停-/禁",
+    'ar': "✅☑ On / start-stop- / ban",
 }
-l_audio_ogg_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> audio для преобразования в голосовое",
-    'en': "👩🏽‍💻 <b>Attach</b> audio to convert to voice",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> audio para convertir a voz",
-    'fr': "👩🏽‍💻 <b>Attachez</b> l'audio pour convertir en voix",
-    'zh': "👩🏽‍💻<b>附加</b>音频以转换为语音",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> الصوت لتحويله إلى صوت",
+l_cnotification_start_off = {
+    'ru': "☑️☐Выкл /start-stop-/ban",
+    'en': "☑️☐Выкл /start-stop-/ban",
+    'es': "☑️☐Выкл /start-stop-/ban",
+    'fr': "☑️☐Выкл /start-stop-/ban",
+    'zh': "☑️☐Выкл /开始-停止-/禁止",
+    'ar': "☑️☐Выкл / start-stop- / الحظر",
 }
-l_audio_transcribe_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> голосовое для преобразования в текст",
-    'en': "👩🏽‍💻 <b>Attach</b> voice to convert to text",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> voz para convertir a texto",
-    'fr': "👩🏽‍💻 <b>Attachez</b> la voix pour convertir en texte",
-    'zh': "👩🏽‍💻<b>附加</b>语音以转换为文本",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> صوت لتحويله إلى نص",
+l_cnotification_push_on = {
+    'ru': "✅☑Вкл нажатие на кнопки",
+    'en': "✅☑On pressing buttons",
+    'es': "✅☑Al presionar botones",
+    'fr': "✅☑En appuyant sur les boutons",
+    'zh': "✅☑按下按钮",
+    'ar': "✅☑ عند الضغط على الأزرار",
 }
-l_audio_recognize = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> распознавания речи",
-    'en': "👩🏽‍💻 Speech Recognition <b>Error</b>",
-    'es': "👩🏽‍💻 <b>Error</b> de reconocimiento de voz",
-    'fr': "👩🏽‍💻 <b>Erreur</b> de reconnaissance vocale",
-    'zh': "👩🏽‍💻语音识别<b>错误</b>",
-    'ar': "👩🏽‍💻 <b>خطأ</b> في التعرف على الكلام",
+l_cnotification_push_off = {
+    'ru': "☑️☐Выкл нажатие на кнопки",
+    'en': "☑️☐Off pressing the buttons",
+    'es': "☑️☐Apagado presionando los botones",
+    'fr': "☑️☐Off en appuyant sur les boutons",
+    'zh': "☑️☐关闭按钮",
+    'ar': "☑️☐ إيقاف الضغط على الأزرار",
 }
 
-l_text_text = {
-    'ru': "👩🏽‍💻 <b>Выбери</b> инструменты для преобразования <i>текста</i> в",
-    'en': "👩🏽‍💻 <b>Choose</b> tools to convert <i>text</i> to",
-    'es': "👩🏽‍💻 <b>Elija</b> herramientas para convertir <i>texto</i> a",
-    'fr': "👩🏽‍💻 <b>Choisissez</b> des outils pour convertir du <i>texte</i> en",
-    'zh': "👩🏽‍💻<b>选择</b>将<i>文本</i>转换为的工具",
-    'ar': "👩🏽‍💻 <b>اختر</b> أدوات لتحويل <i>النص</i> إلى",
-}
-l_text_bin = {
-    'ru': "🔢 bin",
-    'en': "🔢 bin",
-    'es': "🔢 papelera",
-    'fr': "🔢 bin",
-    'zh': "🔢 垃圾桶",
-    'ar': "🔢 بن",
-}
-l_text_hex = {
-    'ru': "🔠 hex",
-    'en': "🔠 hex",
-    'es': "🔠 maleficio",
-    'fr': "🔠 hexagone",
-    'zh': "🔠十六进制",
-    'ar': "🔠 عرافة",
-}
-l_text_null = {
-    'ru': "0️⃣ null",
-    'en': "0️⃣ null",
-    'es': "0️⃣ nulo",
-    'fr': "0️⃣ nul",
-    'zh': "0️⃣ 无",
-    'ar': "0️⃣ لاغية",
-}
-l_text_mp3 = {
-    'ru': "▶️ mp3-аудио",
-    'en': "▶️ mp3-audio",
-    'es': "▶️ audio mp3",
-    'fr': "▶️ audio mp3",
-    'zh': "▶️ mp3音频",
-    'ar': "▶ ️ mp3 الصوت",
-}
-l_text_url = {
-    'ru': "️🧾 url-encode",
-    'en': "️🧾 url-encode",
-    'es': "️🧾 codificación de URL",
-    'fr': "️🧾 url-encoder",
-    'zh': "️🧾 网址编码",
-    'ar': "️🧾 عنوان url ترميز",
-}
-l_text_bin_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> текст для преобразования в бинарный вид",
-    'en': "👩🏽‍💻 <b>Attach</b> text to convert to binary",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> texto para convertir a binario",
-    'fr': "👩🏽‍💻 <b>Joindre</b> du texte à convertir en binaire",
-    'zh': "👩🏽‍💻<b>附加</b>文本以转换为二进制",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> نص لتحويله إلى ثنائي",
-}
-l_text_hex_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> текст для преобразования в hex-символы",
-    'en': "👩🏽‍💻 <b>Attach</b> text to convert to hex characters",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> texto para convertir a caracteres hexadecimales",
-    'fr': "👩🏽‍💻 <b>Joindre</b> du texte à convertir en caractères hexadécimaux",
-    'zh': "👩🏽‍💻<b>附加</b>文本以转换为十六进制字符",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> نص لتحويله إلى أحرف سداسية عشرية",
-}
-l_text_mp3_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> текст для преобразования в голосовое",
-    'en': "👩🏽‍💻 <b>Attach</b> text to convert to voice",
-    'es': "👩🏽‍💻 <b>Adjuntar</b> texto para convertir a voz",
-    'fr': "👩🏽‍💻 <b>Joindre</b> du texte à convertir en voix",
-    'zh': "👩🏽‍💻<b>附加</b>文本以转换为语音",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> نص لتحويله إلى صوت",
+l_cnotification_dialog_on = {
+    'ru': "✅☑Вкл диалог",
+    'en': "✅☑Dialogue included",
+    'es': "✅☑Diálogo incluido",
+    'fr': "✅☑Dialogue inclus",
+    'zh': "✅☑包括对话",
+    'ar': "✅☑ متضمن الحوار",
 }
-l_text_url_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> текст для url-encode-преобразования",
-    'en': "👩🏽‍💻 <b>Attach</b> text for url-encode conversion",
-    'es': "👩🏽‍💻 <b>Adjunte</b> texto para la conversión de codificación URL",
-    'fr': "👩🏽‍💻 <b>Joindre</b> du texte pour la conversion en url-encode",
-    'zh': "👩🏽‍💻<b>附加</b>文本进行 url-encode 转换",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> نص لتحويل ترميز url",
+l_cnotification_dialog_off = {
+    'ru': "☑️☐Выкл диалог",
+    'en': "☑️☐Disable dialogue",
+    'es': "☑️☐Desactivar diálogo",
+    'fr': "☑️☐Désactiver les dialogues",
+    'zh': "☑️☐禁用对话",
+    'ar': "☑️☐ تعطيل الحوار",
 }
-l_text_text1024 = {
-    'ru': "💭 Текст 1024 символа",
-    'en': "💭 Text 1024 characters",
-    'es': "💭 Texto 1024 caracteres",
-    'fr': "💭 Texte 1024 caractères",
-    'zh': "💭 文本 1024 个字符",
-    'ar': "💭 نص 1024 حرفًا",
+l_cnotification_all_on = {
+    'ru': "✅☑Вкл все действия",
+    'en': "✅☑Including all actions",
+    'es': "✅☑Incluyendo todas las acciones",
+    'fr': "✅☑Incluant toutes les actions",
+    'zh': "✅☑包括所有动作",
+    'ar': "✅☑ بما في ذلك جميع الإجراءات",
 }
-l_text_text4096 = {
-    'ru': "🗯️ Текст 4096 символа",
-    'en': "🗯️ Text 4096 characters",
-    'es': "🗯️ Texto 4096 caracteres",
-    'fr': "🗯️ Texte 4096 caractères",
-    'zh': "🗯️ 文本 4096 个字符",
-    'ar': "🗯️ نص 4096 حرفًا",
+l_cnotification_all_off = {
+    'ru': "☑️☐Выкл все действия",
+    'en': "☑️☐Off all actions",
+    'es': "☑️☐Desactivar todas las acciones",
+    'fr': "☑️☐Désactiver toutes les actions",
+    'zh': "☑️☐关闭所有操作",
+    'ar': "☑️☐ إيقاف جميع الإجراءات",
 }
 
-l_convert_error = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> преобразования контента (попробуй позже и загрузи другой файл)",
-    'en': "👩🏽‍💻 Content conversion <b>error</b> (try later and upload another file)",
-    'es': "👩🏽‍💻 <b>Error</b> de conversión de contenido (intente más tarde y cargue otro archivo)",
-    'fr': "👩🏽‍💻 <b>Erreur</b> de conversion de contenu (essayez plus tard et téléchargez un autre fichier)",
-    'zh': "👩🏽‍💻内容转换<b>错误</b>（稍后再试并上传另一个文件）",
-    'ar': "👩🏽‍💻 <b>خطأ</b> في تحويل المحتوى (حاول لاحقًا وقم بتحميل ملف آخر)",
-}
-l_telegraph_text = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> .jpg/.png/.gif/.mp4 - контент, чтобы создать ссылку",
-    'en': "👩🏽‍💻 <b>Attach</b> .jpg/.png/.gif/.mp4 content to create a link",
-    'es': "👩🏽‍💻 <b>Adjunte</b> contenido .jpg/.png/.gif/.mp4 para crear un enlace",
-    'fr': "👩🏽‍💻 <b>Joignez</b> du contenu .jpg/.png/.gif/.mp4 pour créer un lien",
-    'zh': "👩🏽‍💻<b>附加</b>.jpg/.png/.gif/.mp4 内容以创建链接",
-    'ar': "👩🏽‍💻 <b>أرفق</b> محتوى .jpg / .png / .gif / .mp4 لإنشاء ارتباط",
-}
-l_telegraph_error = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> получения ссылки (попробуй позже или загрузи другой файл)",
-    'en': "👩🏽‍💻 <b>Failed</b> to get link (try later and upload another file)",
-    'es': "👩🏽‍💻 <b>No se pudo</b> obtener el enlace (intente más tarde y cargue otro archivo)",
-    'fr': "👩🏽‍💻 <b>Échec</b> de l'obtention du lien (essayez plus tard et téléchargez un autre fichier)",
-    'zh': "👩🏽‍💻 获取链接<b>失败</b>（稍后再试并上传另一个文件）",
-    'ar': "👩🏽‍💻 <b>فشل</b> الحصول على الرابط (حاول لاحقًا وقم بتحميل ملف آخر)",
-}
-l_json_text = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> любое сообщение или сделай пересылку",
-    'en': "👩🏽‍💻 <b>Attach</b> any message or forward",
-    'es': "👩🏽‍💻 <b>Adjunte</b> cualquier mensaje o reenvíe",
-    'fr': "👩🏽‍💻 <b>Joindre</b> n'importe quel message ou transférer",
-    'zh': "👩🏽‍💻<b>附上</b>任何讯息或转发",
-    'ar': "👩🏽‍💻 <b>إرفاق</b> أي رسالة أو إعادة توجيهها",
+l_cnotification_dialog = {
+    'ru': "💬 <b>Пользователь</b>: {0} [<b>id</b>={1}] написал в @{2}-боте:",
+    'en': "💬 <b>User</b> : {0} [<b>id</b> = {1}] wrote in @{2}-bot:",
+    'es': "💬 <b>Usuario</b> : {0} [<b>id</b> = {1}] escribió en @{2}-bot:",
+    'fr': "💬 <b>Utilisateur</b> : {0} [<b>id</b> = {1}] a écrit dans @{2}-bot :",
+    'zh': "💬<b>用户</b>：{0} [<b>id</b> = {1}] 在@{2}-bot 中写道：",
+    'ar': "💬 <b>المستخدم</b> : {0} [<b>id</b> = {1}] كتب في @ {2} -bot:",
 }
 # endregion
 
 
-# region FereyMediaBot
-l_media_btn1 = {
-    'ru': "⛰️ Медиа",
-    'en': "⛰️ Media",
-    'es': "⛰️ Medios",
-    'fr': "⛰️ Médias",
-    'zh': "⛰️ 媒体",
-    'ar': "⛰️ ميديا",
-}
-l_media_btn2 = {
-    'ru': "🌬 Подписка",
-    'en': "🌬 Subscription",
-    'es': "🌬 Suscripción",
-    'fr': "🌬 Abonnement",
-    'zh': "🌬订阅",
-    'ar': "🌬 الاشتراك",
+# region cuser_
+l_cuser_text2 = {
+    'ru': "👥 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> <i>замену голосовых/телескопов на <b>audio/video</b> (*рекомендуется, если premium-пользователи установили такой запрет)/сервисные <b>статусы</b> бота (печатает..записывает видео..)/ведение списка <b>/utm-рефералов</b></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse - вывести всех пользователей\n/utm - вывести utm-рефералов\n/link - создать реферальную /utm ссылку",
+    'en': "👥 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> <i>the replacement of voice/telescopes with <b>audio/video</b> (*recommended if</i> premium <i>users have set such a ban)/bot service <b>statuses</b> (prints..records video..)/maintaining a list of <b>/utm referrals</b></i>\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/parse - display all users\n/utm - display utm referrals\n/link - create a referral /utm link",
+    'es': "👥 <b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> <i>el reemplazo de voz/telescopios con <b>audio/video</b> (*recomendado si</i> los usuarios premium <i>han establecido dicha prohibición)/ <b>estados</b> de servicio de bot (imprime... graba video...)/mantiene una lista de <b>/utm referencias</b></i>\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/parse - mostrar todos los usuarios\n/utm - mostrar referencias utm\n/link - crear un enlace de referencia /utm",
+    'fr': "👥 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>le remplacement de la voix/des télescopes par <b>l&#x27;audio/la vidéo</b> (*recommandé si</i> les utilisateurs premium <i>ont défini une telle interdiction)/ <b>les statuts</b> du service de bot (imprime..enregistre la vidéo..)/maintient une liste de <b>/références utm</b></i>\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/parse - afficher tous les utilisateurs\n/utm - afficher les références utm\n/lien - créer une référence /lien utm",
+    'zh': "👥<b>点击</b>✅/☑️<b>启用/禁用</b><i>用音频<b>/视频</b>替换语音/望远镜（*如果</i>premium<i>用户设置了此类禁令，则推荐）/机器人服务<b>状态</b>（打印..记录视频..）/维护列表<b>/utm referrals</b></i>\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/parse - 显示所有用户\n/utm - 显示 utm referrals\n/link - 创建一个推荐 /utm 链接",
+    'ar': "👥 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <i>استبدال الصوت / التلسكوبات بالصوت <b>/ الفيديو</b> (* يوصى به إذا</i> قام المستخدمون premium <i>بتعيين مثل هذا الحظر) / <b>حالات</b> خدمة الروبوت (طباعة .. تسجيلات فيديو ..) / الاحتفاظ بقائمة من <b>إحالات / utm</b></i>\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - كافة الأوامر\n/ parse - عرض كافة المستخدمين\n/ utm - عرض إحالات utm\n/ link - إنشاء ارتباط إحالة / utm",
 }
-l_media_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> медиа-заметок:\n\n▪️<b>стикеры</b> из текста и фото\n▪️<b>аудио-тренды</b>\n▪️<b>видео-заметки</b>\n▪️инлайн-<b>телескопы</b>\n▪️<b>кнопочные</b> премиум-заметки\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to <i>the landing bot of</i> медиа notes:\n\n▪️ <b>stickers</b> from text and photos\n▪️ <b>audio sounds</b>\n▪️ <b>video notes</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
-    'es': "🌱 {0}, bienvenido <i>al bot de aterrizaje de</i> notas медиа :\n\n▪️ <b>pegatinas</b> de texto y fotos\n▪️ <b>sonidos de audio</b>\n▪️ <b>notas de video</b>\n\n❗️ también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue dans <i>le bot de débarquement des</i> notes медиа :\n\n▪️ <b>autocollants</b> à partir de textes et de photos\n▪️ <b>sons audio</b>\n▪️ <b>notes vidéo</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎来到медиа笔记<i>的登陆机器人</i>：\n\n▪️文字和照片的<b>贴纸</b>\n▪️<b>音频声音</b>\n▪️<b>视频笔记</b>\n\n❗️您也可以在我们的Ferey工作室",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الأساسي</i> لملاحظات медиа :\n\n▪️ <b>ملصقات</b> من النصوص والصور\n▪️ <b>الأصوات الصوتية</b>\n▪️ <b>ملاحظات الفيديو</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت الدردشة في استوديو Ferey الخاص بنا",
+l_cuser_restricted_on = {
+    'ru': "✅☑Вкл audio/video замена",
+    'en': "✅☑Includes audio/video replacement",
+    'es': "✅☑Incluye reemplazo de audio/video",
+    'fr': "✅☑Comprend le remplacement audio/vidéo",
+    'zh': "✅☑包括音频/视频替换",
+    'ar': "✅☑ يشمل استبدال الصوت / الفيديو",
 }
-l_subscribe_media = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>кнопочные</b> премиум-заметки\n\n👩🏽‍💻 /balance",
-    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
-    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
-    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
-    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
-    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+l_cuser_restricted_off = {
+    'ru': "☑️☐Выкл audio/video замена",
+    'en': "☑️☐Off audio/video replacement",
+    'es': "☑️☐Reemplazo de audio/video apagado",
+    'fr': "☑️☐Off remplacement audio/vidéo",
+    'zh': "☑️☐关闭音频/视频替换",
+    'ar': "☑️☐ إيقاف استبدال الصوت / الفيديو",
 }
-
-l_media_text = {
-    'ru': "👩🏽‍💻 <b>Здесь</b> можно выбрать тип выпадающих media-заметок (/add | /del)",
-    'en': "👩🏽‍💻 <b>Here</b> you can select the type of drop-down media notes (/add | /del)",
-    'es': "👩🏽‍💻 <b>Aquí</b> puede seleccionar el tipo de notas multimedia desplegables (/add | /del)",
-    'fr': "👩🏽‍💻 <b>Ici,</b> vous pouvez sélectionner le type de notes multimédia déroulantes (/add | /del)",
-    'zh': "👩🏽‍💻<b>在这里</b>可以选择下拉媒体备注的类型（/add | /del）",
-    'ar': "👩🏽‍💻 <b>هنا</b> يمكنك تحديد نوع ملاحظات الوسائط المنسدلة (/ إضافة | / ديل)",
+l_cuser_status_on = {
+    'ru': "✅☑Вкл сервисные статусы",
+    'en': "✅☑On service statuses",
+    'es': "✅☑Sobre estados de servicio",
+    'fr': "✅☑Sur les états de service",
+    'zh': "✅☑关于服务状态",
+    'ar': "✅☑على حالات الخدمة",
 }
-l_media_del = {
-    'ru': "👩🏽‍💻 <b>Выбери</b> media-заметку для удаления",
-    'en': "👩🏽‍💻 <b>Select</b> media note to delete",
-    'es': "👩🏽‍💻 <b>Seleccione</b> la nota multimedia para eliminar",
-    'fr': "👩🏽‍💻 <b>Sélectionnez</b> la note multimédia à supprimer",
-    'zh': "👩🏽‍💻<b>选择</b>要删除的媒体备注",
-    'ar': "<b>حدد</b> ملاحظة وسائط لحذفها",
+l_cuser_status_off = {
+    'ru': "☑️☐Выкл сервисные статусы",
+    'en': "☑️☐Off service statuses",
+    'es': "☑️☐Estados de servicio desactivados",
+    'fr': "☑️☐Hors statuts de service",
+    'zh': "☑️☐关闭服务状态",
+    'ar': "☑️☐ إيقاف حالات الخدمة",
 }
-l_media_show = {
-    'ru': "👩🏽‍💻 <b>Введи</b> текст для поиска по media-заметкам",
-    'en': "👩🏽‍💻 <b>Enter</b> text to search media notes",
-    'es': "👩🏽‍💻 <b>Ingrese</b> texto para buscar notas multimedia",
-    'fr': "👩🏽‍💻 <b>Entrez</b> du texte pour rechercher des notes multimédias",
-    'zh': "👩🏽‍💻<b>输入</b>文字搜索媒体笔记",
-    'ar': "👩🏽‍💻 <b>أدخل</b> نصًا للبحث في ملاحظات الوسائط",
+l_cuser_utm_on = {
+    'ru': "✅☑Вкл utm-рефералы",
+    'en': "✅☑On utm referrals",
+    'es': "✅☑Sobre referencias utm",
+    'fr': "✅☑Sur les références utm",
+    'zh': "✅☑关于 utm 推荐",
+    'ar': "✅☑On الإحالات UTM",
 }
-l_media_random = {
-    'ru': "🎲 <b>Случайный</b> выбор",
-    'en': "🎲 <b>Random</b> selection",
-    'es': "🎲 Selección <b>aleatoria</b>",
-    'fr': "🎲 Sélection <b>aléatoire</b>",
-    'zh': "🎲<b>随机</b>选择",
-    'ar': "🎲 اختيار <b>عشوائي</b>",
+l_cuser_utm_off = {
+    'ru': "☑️☐Выкл utm-рефералы",
+    'en': "☑️☐Off utm referrals",
+    'es': "☑️☐Off referencias utm",
+    'fr': "☑️☐Hors références utm",
+    'zh': "☑️☐关闭utm推荐",
+    'ar': "☑️☐ Off إحالات UTM",
 }
-l_media_none = {
-    'ru': "👩🏽‍💻 <b>Media</b>-заметок не найдено",
-    'en': "👩🏽‍💻 <b>Media</b> - no notes found",
-    'es': "👩🏽‍💻 <b>Medios</b> : no se encontraron notas",
-    'fr': "👩🏽‍💻 <b>Médias</b> - aucune note trouvée",
-    'zh': "👩🏽‍💻<b>媒体</b>- 未找到笔记",
-    'ar': "👩🏽‍💻 <b>وسائط</b> - لم يتم العثور على ملاحظات",
+l_bot_is_off = {
+    'ru': "👩🏽‍💻 <b>@{0}-бот</b> выключен\n\n/on - включить бот",
+    'en': "👩🏽‍💻 <b>@{0}-bot</b> off\n\n/on - enable bot",
+    'es': "👩🏽‍💻 <b>@{0}-bot</b> apagado\n\n/encendido - habilitar bot",
+    'fr': "👩🏽‍💻 <b>@{0}-bot</b> off\n\n/on - activer le bot",
+    'zh': "👩🏽‍💻 <b>@{0}-bot</b> off\n\n/on - 启用机器人",
+    'ar': "👩🏽‍💻 <b>@ {0} -bot</b> off\n\n/ on - قم بتمكين الروبوت",
 }
-l_media_file = {
-    'ru': "👩🏽‍💻 1/2. <b>Прикрепи</b> audio/video, text/photo контент для создания media-заметки",
-    'en': "👩🏽‍💻 1/2. <b>Attach</b> audio/video, text/photo content to create a media note",
-    'es': "👩🏽‍💻 1/2. <b>Adjunte</b> contenido de audio/video, texto/foto para crear una nota multimedia",
-    'fr': "👩🏽‍💻 1/2. <b>Joignez</b> du contenu audio/vidéo, texte/photo pour créer une note multimédia",
-    'zh': "👩🏽‍💻 1/2。<b>附加</b>音频/视频、文本/照片内容以创建媒体说明",
-    'ar': "👩🏽‍💻 1/2. <b>قم بإرفاق</b> محتوى صوت / فيديو ونص / صورة لإنشاء ملاحظة وسائط",
+l_cuser_utm = {
+    'ru': "👥 <b>Готово!</b> <b>/utm-список</b> реферальных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Вывести</b> рефералов конкретного пользователя можно командой:\n/utm id или /utm @username\n\n👩🏽‍💻 <b>Текущее</b> число utm-рефералов: <u>{1}</u>",
+    'en': "👥 <b>Done!</b> <b>/utm-list</b> of referral users of @{0}-bot\n\n👩🏽‍💻 You can <b>display</b> referrals of a specific user with the command:\n/utm id or /utm @username\n\n👩🏽‍💻 <b>Current</b> number of utm-referrals : <u>{1}</u>",
+    'es': "👥 <b>Listo!</b> <b>/utm-lista</b> de usuarios de referencia de @{0}-bot\n\n👩🏽‍💻 Puede <b>mostrar</b> referencias de un usuario específico con el comando:\n/utm id o /utm @username\n\n👩🏽 ‍💻 Número <b>actual</b> de referencias utm: <u>{1}</u>",
+    'fr': "👥 <b>C&#x27;est fait !</b> <b>/utm-list</b> des utilisateurs référents de @{0}-bot\n\n👩🏽‍💻 Vous pouvez <b>afficher</b> les références d&#x27;un utilisateur spécifique avec la commande :\n/utm id ou /utm @username\n\n👩🏽 ‍💻 Nombre <b>actuel</b> de références utm : <u>{1}</u>",
+    'zh': "👥<b>完成！</b> <b>/utm-@{0}-bot 的推荐用户列表</b>\n\n👩🏽‍💻 您可以使用以下命令<b>显示</b>特定用户的推荐：\n/utm id或/utm @username\n\n👩🏽 ‍💻<b>当前</b>的 utm-referrals 数量： <u>{1}</u>",
+    'ar': "👥 <b>انتهى!</b> <b>/ utm-list</b> لمستخدمي الإحالة لـ @ {0} -bot\n\n👩🏽‍💻 يمكنك <b>عرض</b> إحالات مستخدم معين بالأمر:\n/utm id أو /utm @username\n\n👩🏽 ‍💻 العدد <b>الحالي</b> لإحالات UTM: <u>{1}</u>",
 }
-l_media_title1 = {
-    'ru': "👩🏽‍💻 2/2. <b>Введи</b> ключевые_слова для твоей media-заметки\n[изменить ключевые_слова нельзя]",
-    'en': "👩🏽‍💻 2/2. <b>Enter</b> ключевые_слова for your media note\n[ключевые_слова cannot be changed]",
-    'es': "👩🏽‍💻 2/2. <b>Ingrese</b> ключевые_слова para su nota de prensa\n[ключевые_слова no se pueden cambiar]",
-    'fr': "👩🏽‍💻 2/2. <b>Saisissez</b> ключевые_слова pour votre note média\n[ключевые_слова ne peuvent pas être modifiés]",
-    'zh': "👩🏽‍💻 2/2。为您的媒体说明<b>输入</b>ключевые_слова\n[无法更改ключевые_слова]",
-    'ar': "👩🏽‍💻 2/2. <b>أدخل</b> ключевые_слова لملاحظتك الإعلامية\n[لا يمكن تغيير ключевые_слова]",
+l_cuser_link_done = {
+    'ru': "👥 <b>Готово!</b> Реферальная /utm ссылка на @{0}-бота (размести ее на любой площадке, чтобы понимать, что пользователи перешли в бота с этой площадки):\n\n{1}",
+    'en': "👥 <b>Done!</b> Referral /utm link to the @{0}-bot (place it on any site to understand that users have switched to the bot from this site):\n\n{1}",
+    'es': "👥 <b>Listo!</b> Enlace de referencia /utm al @{0}-bot (colóquelo en cualquier sitio para comprender que los usuarios han cambiado al bot desde este sitio):\n\n{1}",
+    'fr': "👥 <b>C&#x27;est fait !</b> Lien de parrainage /utm vers le @{0}-bot (placez-le sur n&#x27;importe quel site pour comprendre que les utilisateurs sont passés au bot depuis ce site) :\n\n{1}",
+    'zh': "👥<b>完成！</b> @{0}-bot 的引荐 /utm 链接（将其放在任何站点上以了解用户已从该站点切换到该 bot）：\n\n{1}",
+    'ar': "👥 <b>انتهى!</b> رابط الإحالة / utm إلى @ {0} -bot (ضعه على أي موقع لفهم أن المستخدمين قد تحولوا إلى الروبوت من هذا الموقع):\n\n{1}",
 }
-l_media_title2 = {
-    'ru': "👩🏽‍💻 2/2. <b>Текущие</b> ключевые_слова для твоей media-заметки\n\n{0}\n\n[пришли новые или нажми {1}]",
-    'en': "👩🏽‍💻 2/2. <b>Current</b> ключевые_слова for your media note\n\n{0}\n\n[new ones come in or press {1}]",
-    'es': "👩🏽‍💻 2/2. ключевые_слова <b>actuales</b> para su nota de prensa\n\n{0}\n\n[nuevas ingrese o presione {1}]",
-    'fr': "👩🏽‍💻 2/2. ключевые_слова <b>actuels</b> pour votre note multimédia\n\n{0}\n\n[les nouveaux arrivent ou appuyez sur {1}]",
-    'zh': "👩🏽‍💻 2/2。您的媒体说明的<b>当前</b>ключевые_слова\n\n{0}\n\n[请输入新关键字或按 {1}]",
-    'ar': "👩🏽‍💻 2/2. ключевые_слова <b>الحالية</b> لملاحظة الوسائط الخاصة بك\n\n{0}\n\n[يتم إدخال كلمات رئيسية جديدة أو الضغط على {1}]",
+l_cuser_link_start = {
+    'ru': "👥 <b>Придумай</b> название для /utm ссылки (*после ?start= может быть <u>любое</u> имя источника из цифр и/или латинских букв)\n\n👩🏽‍💻 <b>Например</b>, ссылки /utm-рефералов для отслеживания:\nhttps://t.me/{0}?start={1} - <i>реферальных пользователей</i> {1}-<i>пользователя</i>\nhttps://t.me/{0}?start=instagram - <i>пользователей из instagram</i>",
+    'en': "👥 <b>Think of</b> a name for the /utm link (*after ?start= there can be <u>any</u> source name from numbers and/or Latin letters)\n\n👩🏽‍💻 <b>For example</b> , /utm referral links for tracking:\nhttps://t .me/{0}?start={1} - <i>referral users</i> {1} - <i>user</i>\nhttps://t.me/{0}?start=instagram - <i>users from instagram</i>",
+    'es': "👥 <b>Piense en</b> un nombre para el enlace /utm (*después de ?start= puede haber <u>cualquier</u> nombre de fuente de números y/o letras latinas)\n\n👩🏽‍💻 <b>Por ejemplo</b> , enlaces de referencia /utm para el seguimiento:\nhttps ://t .me/{0}?start={1} - <i>usuarios de referencia</i> {1} - <i>usuario</i>\nhttps://t.me/{0}?start=instagram - <i>usuarios de instagram</i>",
+    'fr': "👥 <b>Pensez à</b> un nom pour le lien /utm (*après ?start= il peut y avoir <u>n&#x27;importe quel</u> nom de source à partir de chiffres et/ou de lettres latines)\n\n👩🏽‍💻 <b>Par exemple</b> , les liens de référence /utm pour le suivi :\nhttps ://t .me/{0}?start={1} - <i>utilisateurs de référence</i> {1} - <i>utilisateur</i>\nhttps://t.me/{0}?start=instagram - <i>utilisateurs d&#x27;instagram</i>",
+    'zh': "👥<b>为 /utm 链接想</b>一个名字（*在?start=之后可以有<u>任何</u>来自数字和/或拉丁字母的源名称）\n\n👩🏽‍💻<b>例如</b>，用于跟踪的 /utm 推荐链接：\nhttps ://t .me/{0}?start={1} -<i>推荐用户</i>{1} -<i>用户</i>\nhttps://t.me/{0}?start=instagram -<i>来自 instagram 的用户</i>",
+    'ar': "👥 <b>فكر في</b> اسم ارتباط / utm (* after ?start= يمكن أن يكون هناك <u>أي</u> اسم مصدر من الأرقام و / أو الأحرف اللاتينية)\n\n👩🏽‍💻 <b>على سبيل المثال</b> ، روابط الإحالة / utm للتتبع:\nhttps : // t .me / {0}؟ start = {1} - <i>المستخدمون المحالون</i> {1} - <i>المستخدم</i>\nhttps: //t.me/ {0}؟ start = instagram - <i>المستخدمون من instagram</i>",
 }
-l_media_confirm = {
-    'ru': "🏁 Завершить",
-    'en': "🏁 Complete",
-    'es': "🏁 Completa",
-    'fr': "🏁 Complet",
-    'zh': "🏁 完成",
-    'ar': "🏁 مكتمل",
+l_promo_done = {
+    'ru': "👩🏽‍💻 <b>Готово!</b>\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n{0}\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n/promo 0",
+    'en': "👩🏽‍💻 <b>Done!</b>\n\n👩🏽‍💻 <i>Current /promo code</i> :\n{0}\n👩🏽‍💻 <i>Delete /promo code</i> :\n/promo 0",
+    'es': "👩🏽‍💻 <b>Listo!</b>\n\n👩🏽‍💻 <i>Código /promocional actual</i> :\n{0}\n👩🏽‍💻 <i>Eliminar código /promocional</i> :\n/promo 0",
+    'fr': "👩🏽‍💻 <b>C&#x27;est fait !</b>\n\n👩🏽‍💻 <i>Code /promo actuel</i> :\n{0}\n👩🏽‍💻 <i>Supprimer le code /promo</i> :\n/promo 0",
+    'zh': "👩🏽‍💻<b>完成！</b>\n\n👩🏽‍💻<i>当前/促销代码</i>：\n{0}\n👩🏽‍💻<i>删除/促销代码</i>：\n/promo 0",
+    'ar': "👩🏽‍💻 <b>انتهى!</b>\n\n👩🏽‍💻 <i>الرمز الحالي / الترويجي</i> :\n{0}\n👩🏽‍💻 <i>حذف / الرمز الترويجي</i> :\n/promo 0",
 }
-l_media_error = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> (попробуй позже или загрузи другое media)",
-    'en': "👩🏽‍💻 <b>Error</b> (try later or upload another media)",
-    'es': "👩🏽‍💻 <b>Error</b> (intenta más tarde o sube otro medio)",
-    'fr': "👩🏽‍💻 <b>Erreur</b> (essayez plus tard ou téléchargez un autre média)",
-    'zh': "👩🏽‍💻<b>错误</b>（稍后再试或上传其他媒体）",
-    'ar': "👩🏽‍💻 <b>خطأ</b> (حاول لاحقًا أو قم بتحميل وسائط أخرى)",
+l_promo_start = {
+    'ru': "👩🏽‍💻 <b>Введи</b> /promo-код для @{0}-бота:\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n{1}\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n/promo 0",
+    'en': "👩🏽‍💻 <b>Enter</b> /promo code for @{0}-bot:\n\n👩🏽‍💻 <i>Current /promo code</i> :\n{1}\n👩🏽‍💻 <i>Delete /promo code</i> :\n/promo 0",
+    'es': "👩🏽‍💻 <b>Ingresa el</b> /código de promoción para @{0}-bot:\n\n👩🏽‍💻 <i>Actual /código de promoción</i> :\n{1}\n👩🏽‍💻 <i>Eliminar /código de promoción</i> :\n/promo 0",
+    'fr': "👩🏽‍💻 <b>Entrez</b> /code promo pour @{0}-bot :\n\n👩🏽‍💻 <i>Code /code promo actuel</i> :\n{1}\n👩🏽‍💻 <i>Supprimer /code promo</i> :\n/promo 0",
+    'zh': "👩🏽‍💻<b>输入</b>@{0}-bot 的 /promo 代码：\n\n👩🏽‍💻<i>当前 /promo 代码</i>：\n{1}\n👩🏽‍💻<i>删除 /promo 代码</i>：\n/promo 0",
+    'ar': "👩🏽‍💻 <b>أدخل</b> / الرمز الترويجي لـ @ {0} -bot:\n\n👩🏽‍💻 <i>الرمز الحالي / الترويجي</i> :\n{1}\n👩🏽‍💻 <i>حذف / الرمز الترويجي</i> :\n/promo 0",
 }
-l_media_finish = {
-    'ru': "👩🏽‍💻 <b>Media</b>-заметка успешно создана",
-    'en': "👩🏽‍💻 <b>Media</b> - note created successfully",
-    'es': "👩🏽‍💻 <b>Medios</b> : nota creada con éxito",
-    'fr': "👩🏽‍💻 <b>Média</b> - note créée avec succès",
-    'zh': "👩🏽‍💻<b>媒体</b>- 笔记创建成功",
-    'ar': "👩🏽‍💻 <b>الوسائط</b> - تم إنشاء الملاحظة بنجاح",
+# endregion
+
+
+# region cadmin_
+l_cadmin_text2 = {
+    'ru': "👮🏽 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> <i>доступ добавленных администраторов к функционалу <b>[💬 Оповещения]</b></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей",
+    'en': "👮🏽 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> <i>access of added administrators to functionality <b>[💬 Notifications]</b></i>\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/admin - add/remove administrator\n/parse - display all users",
+    'es': "👮🏽 <b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> <i>el acceso de los administradores agregados a la funcionalidad <b>[💬 Notificaciones]</b></i>\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/admin - agregar/eliminar administrador\n/ analizar - mostrar todos los usuarios",
+    'fr': "👮🏽 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>l&#x27;accès des administrateurs ajoutés à la fonctionnalité <b>[💬 Notifications]</b></i>\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/admin - ajouter/supprimer un administrateur\n/ parse - affiche tous les utilisateurs",
+    'zh': "👮🏽<b>单击</b>✅/☑️<b>启用/禁用</b><i>添加的管理员对功能的访问<b>[💬 通知]</b></i>\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/admin - 添加/删除管理员\n/ parse - 显示所有用户",
+    'ar': "👮🏽 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <i>وصول المسؤولين المضافين إلى الوظائف <b>[💬 إعلامات]</b></i>\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - كافة الأوامر\n/ admin - إضافة / إزالة المسؤول\n/ تحليل - عرض جميع المستخدمين",
 }
-l_media_publish = {
-    'ru': "🔗 Список",
-    'en': "🔗 List",
-    'es': "🔗 Lista",
-    'fr': "🔗 Liste",
-    'zh': "🔗 清单",
-    'ar': "🔗 قائمة",
+l_cadmin_done = {
+    'ru': "👮🏽 <b>Готово!</b>/admin-список @{0}-бота:\n\n{1}\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{2}/10</u>",
+    'en': "👮🏽 <b>Done!</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/admin - add/remove administrator\n/parse - display all users\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{2}/10</u>",
+    'es': "👮🏽 <b>Listo!</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/admin - agregar/eliminar administrador\n/parse - mostrar todos los usuarios\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{2}/10</u>",
+    'fr': "👮🏽 <b>C&#x27;est fait !</b> /admin-list @{0}-bot :\n\n{1}\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/admin - ajouter/supprimer un administrateur\n/parse - afficher tous les utilisateurs\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{2}/10</u>",
+    'zh': "👮🏽<b>完成！</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/admin - 添加/删除管理员\n/parse - 显示所有用户\n\n👩🏽‍💻<b>当前</b>管理员人数： <u>{2}/10</u>",
+    'ar': "👮🏽 <b>انتهى!</b> / admin-list @ {0} -bot:\n\n{1}\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - جميع الأوامر\n/ admin - إضافة / إزالة المسؤول\n/ parse - عرض جميع المستخدمين\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{2} / 10</u>",
 }
-l_media_check = {
-    'ru': "🔗 Проверка",
-    'en': "🔗 Check",
-    'es': "🔗 Comprobar",
-    'fr': "🔗 Vérifier",
-    'zh': "🔗 检查",
-    'ar': "🔗 تحقق",
+l_cadmin_add = {
+    'ru': "👮🏽 <b>Введи</b> до 10 id-пользователей через <i>пробельные или разделительные</i> символы, чтобы добавить их в /admin-список\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{0}</u>",
+    'en': "👮🏽 <b>Enter</b> user id separated by spaces or separators to add them to /admin-list\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{0}</u>",
+    'es': "👮🏽 <b>Ingrese</b> id de usuario separados por espacios o separadores para agregarlos a /admin-list\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{0}</u>",
+    'fr': "👮🏽 <b>Entrez</b> id des utilisateurs séparés par des espaces ou des séparateurs pour les ajouter à /admin-list\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{0}</u>",
+    'zh': "👮🏽<b>输入</b>以空格或分隔符分隔的用户id ，以将其添加到 /admin-list\n\n👩🏽‍💻<b>当前</b>管理员人数： <u>{0}</u>",
+    'ar': "👮🏽 <b>أدخل</b> id المستخدمين مفصولة بمسافات أو فواصل لإضافتها إلى / قائمة المشرف\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{0}</u>",
 }
-l_media_hasdeleted = {
-    'ru': "👩🏽‍💻 <b>Media</b>-заметка удалена",
-    'en': "👩🏽‍💻 <b>Media</b> - note deleted",
-    'es': "👩🏽‍💻 <b>Medios</b> - nota eliminada",
-    'fr': "👩🏽‍💻 <b>Médias</b> - note supprimée",
-    'zh': "👩🏽‍💻<b>媒体</b>- 注释已删除",
-    'ar': "👩🏽‍💻 <b>الوسائط</b> - تم حذف الملاحظة",
+l_cadmin_remove = {
+    'ru': "👮🏽 <b>Введи</b> id пользователей через <i>пробельные или разделительные</i> символы, чтобы удалить их из /admin-список\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{0}</u>",
+    'en': "👮🏽 <b>Enter</b> user id separated by spaces or separators to remove them from /admin-list\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{0}</u>",
+    'es': "👮🏽 <b>Ingrese</b> id de usuario separados por espacios o separadores para eliminarlos de /admin-list\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{0}</u>",
+    'fr': "👮🏽 <b>Entrez</b> id d&#x27;utilisateur séparés par des espaces ou des séparateurs pour les supprimer de /admin-list\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{0}</u>",
+    'zh': "👮🏽<b>输入</b>以空格或分隔符分隔的用户id ，以将其从 /admin-list 中删除\n\n👩🏽‍💻<b>当前</b>管理员数量： <u>{0}</u>",
+    'ar': "👮🏽 <b>أدخل</b> id المستخدمين مفصولة بمسافات أو فواصل لإزالتها من / قائمة المشرف\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{0}</u>",
 }
-l_media_delprepare = {
-    'ru': "🔗 Выбрать",
-    'en': "🔗 Choose",
-    'es': "🔗 Elige",
-    'fr': "🔗 Choisissez",
-    'zh': "🔗选择",
-    'ar': "🔗 اختر",
+l_parse_text = {
+    'ru': "👩🏽‍💻 <b>Готово!</b> Парсинг пользователей (<u>{0}</u>) @{1}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse - вывести всех пользователей\n/parse premium - вывести premium-пользователей\n/parse admin - вывести admin-пользователей\n/parse utm - вывести utm-рефералов\n",
+    'en': "👩🏽‍💻 <b>Done!</b> Parsing users ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/parse - print all users\n/parse premium - print premium users\n/parse admin - display admin users\n/parse utm - display utm referrals\n",
+    'es': "👩🏽‍💻 <b>Listo!</b> Analizando usuarios ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/parse - imprimir todos los usuarios\n/parse premium - imprimir usuarios premium\n/parse admin - mostrar usuarios administradores\n/parse utm - mostrar referencias utm\n",
+    'fr': "👩🏽‍💻 <b>C&#x27;est fait !</b> Analyse des utilisateurs ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/parse - imprimer tous les utilisateurs\n/parse premium - imprimer les utilisateurs premium\n/parse admin - affiche les utilisateurs administrateurs\n/parse utm - affiche les références utm\n",
+    'zh': "👩🏽‍💻<b>完成！</b>解析用户（ <u>{0}</u> ）@{1}-bot\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/parse - 打印所有用户\n/parse premium - 打印高级用户\n/parse admin - 显示管理员用户\n/parse utm - 显示 utm 引用\n",
+    'ar': "👩🏽‍💻 <b>انتهى!</b> تحليل المستخدمين ( <u>{0}</u> ) @ {1} -bot\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - جميع الأوامر\n/ تحليل - طباعة جميع المستخدمين\n/parse premium - طباعة المستخدمين المتميزين\n/parse admin - عرض المستخدمين المسؤولين\n/parse utm - عرض إحالات UTM\n",
 }
 # endregion
+# endregion
 
 
-# region FereyFindBot
-l_find_btn1 = {
-    'ru': "⛰️ Поиск",
-    'en': "⛰️ Search",
-    'es': "⛰️ Buscar",
-    'fr': "⛰️ Rechercher",
-    'zh': "⛰️ 搜索",
-    'ar': "⛰️ بحث",
-}
-l_find_btn2 = {
-    'ru': "📍 Geo поиск",
-    'en': "📍 Geo search",
-    'es': "📍 Búsqueda geográfica",
-    'fr': "📍 Recherche géographique",
-    'zh': "📍地理搜索",
-    'ar': "📍 البحث الجغرافي",
-}
-l_find_btn3 = {
-    'ru': "🔔 Уведомления",
-    'en': "🔔 Notifications",
-    'es': "🔔 Notificaciones",
-    'fr': "🔔 Notifications",
-    'zh': "🔔 通知",
-    'ar': "🔔 الإخطارات",
+# region client
+l_idea = {
+    'ru': "💡 Идея!",
+    'en': "💡 Idea!",
+    'es': "💡 Idea!",
+    'fr': "💡 Idée !",
+    'zh': "💡 想法！",
+    'ar': "💡 فكرة!",
 }
-l_find_btn4 = {
-    'ru': "🌬 Подписка",
-    'en': "🌬 Subscription",
-    'es': "🌬 Suscripción",
-    'fr': "🌬 Abonnement",
-    'zh': "🌬订阅",
-    'ar': "🌬 الاشتراك",
+l_have_read = {
+    'ru': "👩🏽‍💻 {0} прочитал сообщение",
+    'en': "👩🏽‍💻 {0} read the message",
+    'es': "👩🏽‍💻 {0} lee el mensaje",
+    'fr': "👩🏽‍💻 {0} lire le message",
+    'zh': "👩🏽‍💻 {0}阅读消息",
+    'ar': "👩🏽‍💻 {0} اقرأ الرسالة",
 }
-l_find_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> поиска в <b>Telegram</b>:\n\n▪️<b>top</b> каналы/группы\n▪️<b>vip</b> пользователи/боты\n▪️<b>гео</b> парсинг\n▪️<b>пассивный</b> маркетинг\n\n❗️также можно заказать разработку Telegram-продвижения в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
-    'en': "🌱 {0}, welcome to <b>Telegram</b> поиска <i>landing bot</i> :\n\n▪️ <b>top</b> channels/groups\n▪️ <b>vip</b> users/bots\n▪️ <b>geo</b> parsing\n▪️ <b>passive</b> marketing\n\n❗️ you can also order development Telegram promotions in our Ferey studio",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> поиска <b>de Telegram</b> :\n\n▪️ canales/grupos <b>principales</b>\n▪️ usuarios <b>vip</b> /bots\n▪️ análisis <b>geográfico</b>\n▪️ marketing <b>pasivo</b>\n\n❗️ también puedes solicitar promociones de desarrollo de Telegram en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue sur <b>Telegram</b> поиска <i>landing bot</i> :\n\n▪️ <b>meilleurs</b> canaux/groupes\n▪️ utilisateurs/bots <b>vip</b>\n▪️ analyse <b>géographique</b>\n▪️ marketing <b>passif</b>\n\n❗️ vous pouvez également commander des promotions de développement Telegram dans notre atelier de Ferey",
-    'zh': "🌱 {0}，欢迎使用<b>Telegram</b> поиска<i>登陆机器人</i>：\n\n▪️<b>热门</b>频道/群组\n▪️ <b>vip</b>用户/机器人\n▪️<b>地理</b>解析\n▪️<b>被动</b>营销\n\n❗️ 您也可以订购开发 Telegram 促销在我们的Ferey工作室",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوطي</i> поиска <b>Telegram</b> :\n\n▪️ <b>أفضل</b> القنوات / المجموعات\n▪️ مستخدمين / برامج تتبع <b>لكبار</b> الشخصيات\n▪️ تحليل <b>جغرافي</b>\n▪️ تسويق <b>سلبي</b>\n\n❗️ يمكنك أيضًا طلب ترويجات Telegram للتطوير في استوديو Ferey الخاص بنا",
+l_telegraph_title = {
+    'ru': "📰 Telegraph блог",
+    'en': "📰 Telegraph Blog",
+    'es': "📰Blog de telégrafo",
+    'fr': "📰 Blog télégraphique",
+    'zh': "📰 电报博客",
+    'ar': "📰 مدونة التلغراف",
 }
-l_subscribe_find = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>уведомления</b> об услуге\n(<i>ссылка на сообщение</i>)\n▪️<b>приоритетная</b> выдача при поиске\n\n👩🏽‍💻 /balance",
-    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
-    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
-    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
-    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
-    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+l_telegraph_blog = {
+    'ru': "<figure><img src='{0}'/><figcaption>Фото профиля: @{1}</figcaption></figure><blockquote>Лэндинг-блог для продвижения в <i>Telegram</i></blockquote>👩🏽‍💻 <b>бот:</b> {2}<br>[<b>id</b>={3}]<br><b>Био:</b> {4}<br><aside>Описание</aside>{5}",
+    'en': "Profile photo: @{1}Landing blog for promotion in <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = {3}] <b>Bio:</b> {4}Description{5}",
+    'es': "Foto de perfil: @{1}Blog de aterrizaje para promoción en <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = {3}] <b>Bio:</b> {4}Descripción{5}",
+    'fr': "Photo de profil : @{1}Blog d'atterrissage pour la promotion dans <i>Telegram</i> 👩🏽‍💻 <b>bot :</b> {2}[<b>id</b> = {3}] <b>Bio :</b> {4}Description{5}",
+    'zh': "个人资料照片：@{1}登陆博客以在<i>Telegram</i> 👩🏽‍💻<b>机器人中进行推广：</b> {2}[<b>id</b> = {3}]<b>简介：</b> {4}说明{5}",
+    'ar': "صورة الملف الشخصي: @ {1} مدونة الهبوط للترويج في <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2} [<b>id</b> = {3}] <b>السيرة الذاتية:</b> {4} الوصف {5}",
 }
+# endregion
 
-l_geo_minus = {
-    'ru': "-",
-    'en': "-",
-    'es': "-",
-    'fr': "-",
-    'zh': "-",
-    'ar': "-",
-}
-l_geo_current = {
-    'ru': "📍R: {0}m",
-    'en': "📍R: {0}m",
-    'es': "📍R: {0}m",
-    'fr': "📍R : {0}mois",
-    'zh': "📍R：{0}米",
-    'ar': "📍R: {0} م",
+
+# region extra bot
+l_show_admin_panel_md = {
+    'ru': "*👩🏽‍💻 Создание и редактирование блога*\n\n👩🏽‍💻 Вы зашли как *Администратор* и можете создавать и редактировать блоги, но не удалять их\n\n¹ Авторизация по ссылке в браузере:\n`{0}`\n\n² Перейди (в течение 10сек) по нужной ссылке для редактирования публикации (жми, чтобы скопировать):\n\n",
+    'en': "*👩🏽‍💻 Creating and editing a blog*\n\n👩🏽‍💻 You are logged in as *Administrator* and can create and edit blogs, but not delete them\n\n¹ Authorization via link in browser:\n`{0 }`\n\n² Go (within 10 seconds) to the desired link to edit the post (click to copy):\n\n",
+    'es': "*👩🏽‍💻 Crear y editar un blog*\n\n👩🏽‍💻 Ha iniciado sesión como *Administrador* y puede crear y editar blogs, pero no eliminarlos\n\n¹ Autorización a través de un enlace en el navegador:\n`{0 }`\n\n² Vaya (dentro de 10 segundos) al enlace deseado para editar la publicación (haga clic para copiar):\n\n",
+    'fr': "*👩🏽‍💻 Créer et modifier un blog*\n\n👩🏽‍💻 Vous êtes connecté en tant qu'*administrateur* et vous pouvez créer et modifier des blogs, mais pas les supprimer\n\n¹ Autorisation via un lien dans le navigateur :\n`{0 }`\n\n² Accédez (dans les 10 secondes) au lien souhaité pour modifier le message (cliquez pour copier) :\n\n",
+    'zh': "*👩🏽‍💻 创建和编辑博客*\n\n👩🏽‍💻 您以*管理员*身份登录，可以创建和编辑博客，但不能删除它们\n\n¹ 通过浏览器中的链接授权：\n`{0 }`\n\n²（在 10 秒内）转到所需的链接以编辑帖子（单击以复制）：\n\n",
+    'ar': "* 👩🏽‍💻 إنشاء مدونة وتحريرها *\n\n👩🏽‍💻 تم تسجيل دخولك بصفتك * المسؤول * ويمكنك إنشاء المدونات وتحريرها ، ولكن لا يمكنك حذفها\n\n¹ التفويض عبر الارتباط في المستعرض:\n'{0}`\n\n² انتقل (في غضون 10 ثوانٍ) إلى الرابط المطلوب لتعديل المشاركة (انقر للنسخ):\n\n",
 }
-l_geo_plus = {
-    'ru': "+",
-    'en': "+",
-    'es': "+",
-    'fr': "+",
-    'zh': "+",
-    'ar': "+",
+l_show_admin_panel_html = {
+    'ru': "<b>👩🏽‍💻 Создание и редактирование блога</b>\n\n👩🏽‍💻 Вы зашли как <b>Администратор</b> и можете создавать и редактировать блоги, но не удалять их\n\n1. Авторизация по ссылке в браузере:\n{0}\n\n2. Перейди (в течение 10сек) по нужной ссылке для редактирования публикации (жми, чтобы скопировать):\n\n",
+    'en': "<b>👩🏽‍💻 Creating and editing a blog</b>\n\n👩🏽‍💻 You are logged in as <b>Administrator</b> and can create and edit blogs, but not delete them\n\n1. Authorization by link in browser:\n{0}\n\n2. Go (within 10 seconds) to the desired link to edit the publication (click to copy):\n\n",
+    'es': "<b>👩🏽‍💻 Crear y editar un blog</b>\n\n👩🏽‍💻 Ha iniciado sesión como <b>Administrador</b> y puede crear y editar blogs, pero no borrarlos\n\n1. Autorización por enlace en el navegador:\n{0}\n\n2. Vaya (dentro de 10 segundos) al enlace deseado para editar la publicación (haga clic para copiar):\n\n",
+    'fr': "<b>👩🏽‍💻 Créer et modifier un blog</b>\n\n👩🏽‍💻 Vous êtes connecté en tant <b>qu&#x27;administrateur</b> et pouvez créer et modifier des blogs, mais pas les supprimer\n\n1. Autorisation par lien dans le navigateur :\n{0}\n\n2. Accédez (dans les 10 secondes) au lien souhaité pour modifier la publication (cliquez pour copier) :\n\n",
+    'zh': "<b>👩🏽‍💻 创建和编辑博客</b>\n\n👩🏽‍💻 您以<b>管理员</b>身份登录，可以创建和编辑博客，但不能删除它们\n\n1.通过浏览器中的链接授权：\n{0}\n\n2.转到（在 10 秒内）所需的链接以编辑发布（单击以复制）：\n\n",
+    'ar': "<b>👩🏽‍💻 إنشاء مدونة وتحريرها</b>\n\n👩🏽‍💻 قمت بتسجيل الدخول <b>كمسؤول</b> ويمكنك إنشاء المدونات وتحريرها ، ولكن لا يمكنك حذفها\n\n1. التفويض بالارتباط في المتصفح:\n{0}\n\n2. انتقل (في غضون 10 ثوانٍ) إلى الارتباط المطلوب لتحرير المنشور (انقر للنسخ):\n\n",
 }
-l_geo_text1 = {
-    'ru': "📍 <b>Geo-поиск</b> пользователей по координатам\n\n👩🏽‍💻 <b>Жми</b> на -/+, чтобы настроить 📍Radius",
-    'en': "📍 <b>Geo-search</b> users by coordinates\n\n👩🏽‍💻 <b>Click</b> on -/+ to adjust 📍Radius",
-    'es': "📍 Usuarios <b>de búsqueda geográfica</b> por coordenadas\n\n👩🏽‍💻 <b>Haz clic</b> en -/+ para ajustar el 📍Radio",
-    'fr': "📍 <b>Géo-recherche</b> des utilisateurs par coordonnées\n\n👩🏽‍💻 <b>Cliquez</b> sur -/+ pour ajuster 📍Rayon",
-    'zh': "📍 按坐标<b>地理搜索</b>用户\n\n👩🏽‍💻<b>点击</b>-/+ 调整📍半径",
-    'ar': "📍 <b>البحث الجغرافي</b> للمستخدمين عن طريق الإحداثيات\n\n👩🏽‍💻 <b>انقر</b> فوق - / + لضبط 📍Radius",
+l_show_admin_panel_create = {
+    'ru': "🆕 Создать",
+    'en': "🆕 Create",
+    'es': "🆕 Crear",
+    'fr': "🆕 Créer",
+    'zh': "🆕 创建",
+    'ar': "🆕 خلق",
 }
-l_geo_text2 = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> геопозицию через 📎-меню вложений или на<b>Жми</b> на кнопку ниже\n[📍Отправить Geo] 👇🏽",
-    'en': "👩🏽‍💻 <b>Attach</b> a location via the 📎 attachment menu or <b>click</b> on the button below\n[📍Send Geo] 👇🏽",
-    'es': "👩🏽‍💻 <b>Adjunte</b> una ubicación a través del 📎 menú de archivos adjuntos o <b>haga clic</b> en el botón a continuación\n[📍Send Geo] 👇🏽",
-    'fr': "👩🏽‍💻 <b>Joignez</b> un lieu via le 📎 menu de pièces jointes ou <b>cliquez</b> sur le bouton ci-dessous\n[📍Envoyer Géo] 👇🏽",
-    'zh': "👩🏽‍💻通过📎附件菜单<b>附加</b>位置或<b>单击</b>下面的按钮\n[📍发送地理信息]👇🏽",
-    'ar': "👩🏽‍💻 <b>قم بإرفاق</b> موقع عبر قائمة 📎 المرفقات أو <b>انقر</b> فوق الزر أدناه\n[Send Geo] 👇🏽",
+l_show_admin_panel_auth = {
+    'ru': "👩🏽‍💻 Авторизация",
+    'en': "👩🏽‍💻 Authorization",
+    'es': "👩🏽‍💻 Autorización",
+    'fr': "👩🏽‍💻 Autorisation",
+    'zh': "👩🏽‍💻授权",
+    'ar': "👩🏽‍💻 إذن",
 }
-l_geo_send = {
-    'ru': "📍Отправить Geo",
-    'en': "📍Send Geo",
-    'es': "📍Enviar Geo",
-    'fr': "📍Envoyer Géo",
-    'zh': "📍发送地理位置",
-    'ar': "📍إرسال جيو",
+# endregion
+
+
+# region html
+l_burger_save = {
+    'ru': "Сохранить",
+    'en': "Save",
+    'es': "Ahorrar",
+    'fr': "Sauvegarder",
+    'zh': "节省",
+    'ar': "يحفظ",
 }
-l_geo_start = {
-    'ru': "🔎 Начинаем поиск..",
-    'en': "🔎 Let's start the search..",
-    'es': "🔎 Comencemos la búsqueda..",
-    'fr': "🔎 Commençons la recherche..",
-    'zh': "🔎 让我们开始搜索..",
-    'ar': "🔎 لنبدأ البحث ..",
+l_burger_gen = {
+    'ru': "Сгенерировать бота",
+    'en': "Generate bot",
+    'es': "Generar bot",
+    'fr': "Générer un robot",
+    'zh': "生成机器人",
+    'ar': "توليد بوت",
 }
-l_geo_no = {
-    'ru': "📍 Пользователей (@username) в данной геопозиции не найдено",
-    'en': "📍 No users ( @username ) found in this location",
-    'es': "📍 No se encontraron usuarios ( @username ) en esta ubicación",
-    'fr': "📍 Aucun utilisateur ( @username ) trouvé à cet emplacement",
-    'zh': "📍 在此位置找不到用户 ( @username )",
-    'ar': "📍 لم يتم العثور على مستخدمين ( @username ) في هذا الموقع",
+l_burger_import = {
+    'ru': "Импортировать .bot",
+    'en': "Import .bot",
+    'es': "Importar .bot",
+    'fr': "Importer .bot",
+    'zh': "导入.bot",
+    'ar': "استيراد .bot",
 }
-l_geo_finish = {
-    'ru': "🔥 <b>Готово!</b> Найдено пользователей: <u>{0}</u>",
-    'en': "🔥 <b>Done!</b> Found users: <u>{0}</u>",
-    'es': "🔥 <b>Listo!</b> Usuarios encontrados: <u>{0}</u>",
-    'fr': "🔥 <b>C&#x27;est fait !</b> Utilisateurs trouvés : <u>{0}</u>",
-    'zh': "🔥<b>完成！</b>找到的用户： <u>{0}</u>",
-    'ar': "🔥 <b>انتهى!</b> المستخدمون الموجودون: <u>{0}</u>",
+l_burger_export = {
+    'ru': "Экспортировать как >",
+    'en': "Export as >",
+    'es': "Exportar como >",
+    'fr': "Exporter sous >",
+    'zh': "导出为 >",
+    'ar': "تصدير باسم>",
 }
-
-l_find_add_cmd = {
-    'ru': "👩🏽‍💻 <b>Пришли</b> ссылку на канал/группу/пользователя/бота",
-    'en': "👩🏽‍💻 <b>Send</b> a link to a channel/group/user/bot",
-    'es': "👩🏽‍💻 <b>Enviar</b> un enlace a un canal/grupo/usuario/bot",
-    'fr': "👩🏽‍💻 <b>Envoyer</b> un lien vers un canal/groupe/utilisateur/bot",
-    'zh': "👩🏽‍💻<b>发送</b>指向频道/组/用户/机器人的链接",
-    'ar': "👩🏽‍💻 <b>أرسل</b> رابطًا إلى قناة / مجموعة / مستخدم / روبوت",
+l_burger_clear = {
+    'ru': "Очистить",
+    'en': "Cleaning",
+    'es': "Limpieza",
+    'fr': "Nettoyage",
+    'zh': "打扫",
+    'ar': "تنظيف",
 }
-l_find_err_cmd = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> (вставь корректную ссылку или повтори позже)",
-    'en': "👩🏽‍💻 <b>Error</b> (insert correct link or try again later)",
-    'es': "👩🏽‍💻 <b>Error</b> (inserta el enlace correcto o vuelve a intentarlo más tarde)",
-    'fr': "👩🏽‍💻 <b>Erreur</b> (insérez le lien correct ou réessayez plus tard)",
-    'zh': "👩🏽‍💻<b>错误</b>（插入正确的链接或稍后重试）",
-    'ar': "👩🏽‍💻 <b>خطأ</b> (أدخل الرابط الصحيح أو حاول مرة أخرى لاحقًا)",
+l_burger_gen_alert = {
+    'ru': "Создать нового бота?",
+    'en': "Create a new bot?",
+    'es': "¿Crear un nuevo bot?",
+    'fr': "Créer un nouveau bot ?",
+    'zh': "创建一个新的机器人？",
+    'ar': "إنشاء روبوت جديد؟",
 }
-l_find_ok_cmd = {
-    'ru': "👩🏽‍💻 <b>Ссылка</b> успешно добавлена!",
-    'en': "👩🏽‍💻 <b>Link</b> added successfully!",
-    'es': "👩🏽‍💻 ¡ <b>Enlace</b> agregado exitosamente!",
-    'fr': "👩🏽‍💻 <b>Lien</b> ajouté avec succès !",
-    'zh': "👩🏽‍💻<b>链接</b>添加成功！",
-    'ar': "👩🏽‍💻 تمت إضافة <b>الرابط</b> بنجاح!",
+l_burger_import_alert = {
+    'ru': "Загрузка..",
+    'en': "Loading..",
+    'es': "Cargando..",
+    'fr': "Chargement..",
+    'zh': "加载中..",
+    'ar': "تحميل..",
 }
-l_find_check = {
-    'ru': "🔗 Проверка",
-    'en': "🔗 Check",
-    'es': "🔗 Comprobar",
-    'fr': "🔗 Vérifier",
-    'zh': "🔗 检查",
-    'ar': "🔗 تحقق",
+l_burger_clear_alert = {
+    'ru': "Очистить сцену?",
+    'en': "Clear the scene?",
+    'es': "Limpiar la escena?",
+    'fr': "Vider la scène ?",
+    'zh': "清理现场？",
+    'ar': "مسح المشهد؟",
 }
 
-l_find_menu = {
-    'ru': "↩ Menu",
-    'en': "↩ Menu",
-    'es': "↩ Menú",
-    'fr': "↩Menu",
-    'zh': "↩ 菜单",
-    'ar': "↩ القائمة",
-}
-l_find_text = {
-    'ru': "<b>🔎 Сбор целевой аудитории (ЦА)</b>\n\n▪️выгрузка тематических каналов\n▪️выгрузка лидов/чатов с ЦА\n▪️выгрузка конкурентов по нише\n▪️каталог ботов\n\n<b>Итог:</b> <i>получение <u>горячей</u> ЦА, анализ ЦА конкурентов</i>",
-    'en': "<b>🔎 Gathering the target audience (CA)</b>\n\n▪️uploading thematic channels\n▪️uploading leads/chats from the target audience\n▪️uploading competitors by niche\n▪️bot directory\n\n<b>Result:</b> <i>getting <u>a hot target</u> audience, analyzing the target audience of competitors</i>",
-    'es': "<b>🔎 Reunir el público objetivo (CA)</b>\n\n▪️cargar canales temáticos\n▪️cargar clientes potenciales/chats del público objetivo\n▪️cargar competidores por nicho\n▪️directorio de bots\n\n<b>Resultado:</b> <i>obtener <u>un público objetivo atractivo</u> , analizando el público objetivo de los competidores</i>",
-    'fr': "<b>🔎 Rassembler le public cible (CA)</b>\n\n▪️télécharger des chaînes thématiques\n▪️télécharger des prospects/chats du public cible\n▪️télécharger des concurrents par niche\n▪️répertoire de robots\n\n<b>Résultat :</b> <i>obtenir <u>un public cible chaud</u> , analysant le public cible des concurrents</i>",
-    'zh': "<b>🔎 收集目标受众 (CA)</b>\n\n▪️上传主题频道\n▪️从目标受众上传线索/聊天\n▪️按利基上传竞争对手\n▪️bot 目录\n\n<b>结果：</b><i>获得<u>热门目标</u>受众, 分析竞争对手的目标受众</i>",
-    'ar': "<b>🔎 تجميع الجمهور المستهدف (CA)</b>\n\n▪️ تحميل القنوات الموضوعية\n▪️ تحميل العملاء المتوقعين / الدردشات من الجمهور المستهدف\n▪️ تحميل المنافسين حسب المجال المناسب\n▪️ الدليل الآلي\n\n<b>النتيجة:</b> <i>الحصول على جمهور <u>مستهدف نشط</u> ، وتحليل الجمهور المستهدف من المنافسين</i>",
-}
-l_find_category_typing = {
-    'ru': "✅ #ввести свои параметры",
-    'en': "✅ #ввести your parameters",
-    'es': "✅ #ввести sus parámetros",
-    'fr': "✅ #ввести vos paramètres",
-    'zh': "✅ # #ввести你的参数",
-    'ar': "✅ # #ввести المعلمات الخاصة بك",
+l_ent_close = {
+    'ru': "Закрыть",
+    'en': "Close",
+    'es': "Cerca",
+    'fr': "Fermer",
+    'zh': "关闭",
+    'ar': "يغلق",
 }
-l_find_desc = {
-    'ru': "<b>Описание:</b> {0}",
-    'en': "<b>Description:</b> {0}",
-    'es': "<b>Descripción:</b> {0}",
-    'fr': "<b>Descriptif :</b> {0}",
-    'zh': "<b>说明：</b> {0}",
-    'ar': "<b>الوصف:</b> {0}",
+l_ent_save = {
+    'ru': "Сохранить",
+    'en': "Save",
+    'es': "Ahorrar",
+    'fr': "Sauvegarder",
+    'zh': "节省",
+    'ar': "يحفظ",
 }
-l_find_reacts = {
-    'ru': "<b>Реакции:</b> {0}",
-    'en': "<b>Reactions:</b> {0}",
-    'es': "<b>Reacciones:</b> {0}",
-    'fr': "<b>Réactions :</b> {0}",
-    'zh': "<b>反应：</b> {0}",
-    'ar': "<b>التفاعلات:</b> {0}",
+l_ent_delete = {
+    'ru': "Удалить",
+    'en': "Delete",
+    'es': "Borrar",
+    'fr': "Supprimer",
+    'zh': "删除",
+    'ar': "يمسح",
 }
-l_find_send = {
-    'ru': "<b>Сообщ/медиа/инлайн/инвайт:</b> {0}/{1}/{2}/{3}",
-    'en': "<b>Message/Media/Inline/Invite:</b> {0}/{1}/{2}/{3}",
-    'es': "<b>Mensaje/Medios/En línea/Invitación:</b> {0}/{1}/{2}/{3}",
-    'fr': "<b>Message/Média/Inline/Invitation :</b> {0}/{1}/{2}/{3}",
-    'zh': "<b>消息/媒体/内联/邀请：</b> {0}/{1}/{2}/{3}",
-    'ar': "<b>رسالة / وسائط / مضمنة / دعوة:</b> {0} / {1} / {2} / {3}",
+l_copied = {
+    'ru': "Скопировано",
+    'en': "Copied",
+    'es': "Copiado",
+    'fr': "Copié",
+    'zh': "已复制",
+    'ar': "نسخ",
 }
-l_find_bio = {
-    'ru': "<b>Био:</b> {0}",
-    'en': "<b>Bio:</b> {0}",
-    'es': "<b>Biografía:</b> {0}",
-    'fr': "<b>Biographie :</b> {0}",
-    'zh': "<b>简历：</b> {0}",
-    'ar': "<b>السيرة الذاتية:</b> {0}",
+l_web_gen_img = {
+    'ru': "Сгенерировать Образ",
+    'en': "Generate Image",
+    'es': "Generar imagen",
+    'fr': "Générer une image",
+    'zh': "生成图像",
+    'ar': "توليد الصورة",
 }
-l_find_about = {
-    'ru': "<b>Описание:</b> {0}",
-    'en': "<b>Description:</b> {0}",
-    'es': "<b>Descripción:</b> {0}",
-    'fr': "<b>Descriptif :</b> {0}",
-    'zh': "<b>说明：</b> {0}",
-    'ar': "<b>الوصف:</b> {0}",
+l_web_gen_txt = {
+    'ru': "Сгенерировать Текст",
+    'en': "Generate Text",
+    'es': "Generar Texto",
+    'fr': "Générer du texte",
+    'zh': "生成文本",
+    'ar': "توليد نص",
 }
-l_find_description = {
-    'ru': "<b>Подробнее:</b> {0}",
-    'en': "<b>Read more:</b> {0}",
-    'es': "<b>Leer más:</b> {0}",
-    'fr': "<b>En savoir plus :</b> {0}",
-    'zh': "<b>阅读更多：</b> {0}",
-    'ar': "<b>اقرأ المزيد:</b> {0}",
+l_all_trg = {
+    'ru': ": все триггеры",
+    'en': ": all triggers",
+    'es': ": todos los disparadores",
+    'fr': ": tous les déclencheurs",
+    'zh': ": 所有触发器",
+    'ar': ": جميع المشغلات",
 }
-l_find_commands = {
-    'ru': "<b>Команды:</b> {0}",
-    'en': "<b>Commands:</b> {0}",
-    'es': "<b>Comandos:</b> {0}",
-    'fr': "<b>Commandes :</b> {0}",
-    'zh': "<b>命令：</b> {0}",
-    'ar': "<b>الأوامر:</b> {0}",
+l_one_trg = {
+    'ru': ": 1 триггер",
+    'en': ": 1 trigger",
+    'es': ": 1 gatillo",
+    'fr': ": 1 gâchette",
+    'zh': "：1个触发器",
+    'ar': ": 1 الزناد",
 }
-
-l_find_chn = {
-    'ru': "📰 Каналы",
-    'en': "📰 Channels",
-    'es': "📰 Canales",
-    'fr': "📰 Chaînes",
-    'zh': "📰频道",
-    'ar': "📰 القنوات",
+l_actions = {
+    'ru': ": действия",
+    'en': ": actions",
+    'es': ": acciones",
+    'fr': ": Actions",
+    'zh': "：行动",
+    'ar': ": أجراءات",
 }
-l_find_grp = {
-    'ru': "📁 Группы",
-    'en': "📁 Groups",
-    'es': "📁 Grupos",
-    'fr': "📁 Groupes",
-    'zh': "📁 团体",
-    'ar': "📁 المجموعات",
+l_trigger = {
+    'ru': "Триггер",
+    'en': "Trigger",
+    'es': "Desencadenar",
+    'fr': "Déclencher",
+    'zh': "扳机",
+    'ar': "مشغل",
 }
-l_find_usr = {
-    'ru': "🕵️ Конкуренты",
-    'en': "🕵️ Competitors",
-    'es': "🕵️ Competidores",
-    'fr': "🕵️ Concurrents",
-    'zh': "🕵️ 参赛者",
-    'ar': "🕵️ المنافسون",
+l_action = {
+    'ru': "Действие",
+    'en': "Action",
+    'es': "Acción",
+    'fr': "Action",
+    'zh': "行动",
+    'ar': "فعل",
 }
-l_find_bot = {
-    'ru': "🫥 Боты",
-    'en': "🫥 Tg bots",
-    'es': "🫥Tg bots",
-    'fr': "🫥 Robots Tg",
-    'zh': "🫥 Tg 机器人",
-    'ar': "🫥 Tg bots",
+l_message = {
+    'ru': "Сообщение",
+    'en': "Message",
+    'es': "Mensaje",
+    'fr': "Message",
+    'zh': "信息",
+    'ar': "رسالة",
 }
 
-l_find_chn_choose = {
-    'ru': "📰 <b>Выбери категорию</b> для выгрузки каналов",
-    'en': "📰 <b>Choose a category</b> for uploading channels",
-    'es': "📰 <b>Elige una categoría</b> para subir canales",
-    'fr': "📰 <b>Choisissez une catégorie</b> pour télécharger des chaînes",
-    'zh': "📰<b>选择上传频道的类别</b>",
-    'ar': "📰 <b>اختر فئة</b> لتحميل القنوات",
-}
-l_find_grp_choose = {
-    'ru': "📁 <b>Выбери категорию</b> для выгрузки групп",
-    'en': "📁 <b>Choose a category</b> for uploading groups",
-    'es': "📁 <b>Elige una categoría</b> para subir grupos",
-    'fr': "📁 <b>Choisissez une catégorie</b> pour télécharger des groupes",
-    'zh': "📁<b>选择上传群组的类别</b>",
-    'ar': "📁 <b>اختر فئة</b> لتحميل المجموعات",
-}
-l_find_usr_choose = {
-    'ru': "🕵️ <b>Выбери категорию</b> для выгрузки пользователей",
-    'en': "🕵️ <b>Choose a category</b> to upload users",
-    'es': "🕵️ <b>Elige una categoría</b> para subir usuarios",
-    'fr': "🕵️ <b>Choisissez une catégorie</b> pour télécharger des utilisateurs",
-    'zh': "🕵️<b>选择一个类别</b>上传用户",
-    'ar': "🕵️ <b>اختر فئة</b> لتحميل المستخدمين",
+l_trg_add = {
+    'ru': "+ Добавить Триггер",
+    'en': "+ Add Trigger",
+    'es': "+ Agregar disparador",
+    'fr': "+ Ajouter un déclencheur",
+    'zh': "+ 添加触发器",
+    'ar': "+ إضافة مشغل",
 }
-l_find_bot_choose = {
-    'ru': "🥾 <b>Выбери категорию</b> для выгрузки ботов",
-    'en': "🥾 <b>Choose a category</b> for uploading bots",
-    'es': "🥾 <b>Elija una categoría</b> para cargar bots",
-    'fr': "🥾 <b>Choisissez une catégorie</b> pour télécharger des bots",
-    'zh': "🥾<b>选择上传机器人的类别</b>",
-    'ar': "🥾 <b>اختر فئة</b> لتحميل الروبوتات",
+l_trg_cmd = {
+    'ru': "+ команда",
+    'en': "+ command",
+    'es': "+ comando",
+    'fr': "+ commande",
+    'zh': "+ 命令",
+    'ar': "+ الأمر",
 }
-
-l_find_chn_find = {
-    'ru': "🔎 Поиск по каналам",
-    'en': "🔎 Channel search",
-    'es': "🔎 Búsqueda de canales",
-    'fr': "🔎 Recherche de chaînes",
-    'zh': "🔎 频道搜索",
-    'ar': "🔎 قناة البحث",
+l_trg_txt = {
+    'ru': "+ текст",
+    'en': "+ text",
+    'es': "+ texto",
+    'fr': "+ texte",
+    'zh': "+ 文字",
+    'ar': "+ نص",
 }
-l_find_grp_find = {
-    'ru': "🔎 Поиск по группам",
-    'en': "🔎 Group search",
-    'es': "🔎 Búsqueda de grupos",
-    'fr': "🔎 Recherche de groupe",
-    'zh': "🔎 群组搜索",
-    'ar': "🔎 بحث المجموعة",
+l_trg_btn = {
+    'ru': "+ кнопка",
+    'en': "+ button",
+    'es': "+ botón",
+    'fr': "+ bouton",
+    'zh': "+ 按钮",
+    'ar': "+ زر",
 }
-l_find_usr_find = {
-    'ru': "🔎 Поиск по конкурентам",
-    'en': "🔎 Search by competitors",
-    'es': "🔎 Búsqueda por competidores",
-    'fr': "🔎 Recherche par concurrents",
-    'zh': "🔎 按竞争对手搜索",
-    'ar': "🔎 البحث عن طريق المنافسين",
+l_trg_var = {
+    'ru': "+ переменная",
+    'en': "+ variable",
+    'es': "+ variables",
+    'fr': "+ variable",
+    'zh': "+ 变量",
+    'ar': "+ متغير",
 }
-l_find_bot_find = {
-    'ru': "🔎 Поиск по ботам",
-    'en': "🔎 Search by bots",
-    'es': "🔎 Búsqueda por bots",
-    'fr': "🔎 Recherche par bots",
-    'zh': "🔎 机器人搜索",
-    'ar': "🔎 البحث عن طريق الروبوتات",
+l_trg_lst = {
+    'ru': "+ список",
+    'en': "+ list",
+    'es': "+ lista",
+    'fr': "+ liste",
+    'zh': "+ 列表",
+    'ar': "+ قائمة",
 }
 
-l_find_chn_link = {
-    'ru': "🔗 Перейти к каналу",
-    'en': "🔗 Go to channel",
-    'es': "🔗 Ir al canal",
-    'fr': "🔗 Aller à la chaîne",
-    'zh': "🔗 前往频道",
-    'ar': "🔗 اذهب إلى القناة",
+l_act_add = {
+    'ru': "+ Добавить Действие",
+    'en': "+ Add Action",
+    'es': "+ Agregar acción",
+    'fr': "+ Ajouter une action",
+    'zh': "+ 添加动作",
+    'ar': "+ إضافة عمل",
 }
-l_find_grp_link = {
-    'ru': "🔗 Перейти к группе",
-    'en': "🔗 Go to group",
-    'es': "🔗 Ir al grupo",
-    'fr': "🔗 Aller au groupe",
-    'zh': "🔗 进群",
-    'ar': "🔗 اذهب إلى المجموعة",
+l_act_dly = {
+    'ru': "+ задержка",
+    'en': "+ delay",
+    'es': "+ retraso",
+    'fr': "+ délai",
+    'zh': "+延迟",
+    'ar': "+ تأخير",
 }
-l_find_usr_link = {
-    'ru': "🔗 Перейти к пользователю",
-    'en': "🔗 Go to user",
-    'es': "🔗 Ir a usuario",
-    'fr': "🔗 Aller à l'utilisateur",
-    'zh': "🔗 转到用户",
-    'ar': "🔗 اذهب إلى المستخدم",
+l_act_wait = {
+    'ru': "+ ожидание",
+    'en': "+ waiting",
+    'es': "+ esperando",
+    'fr': "+ attente",
+    'zh': "+ 等待",
+    'ar': "+ الانتظار",
 }
-l_find_bot_link = {
-    'ru': "🔗 Перейти к боту",
-    'en': "🔗 Go to bot",
-    'es': "🔗 Ir al bot",
-    'fr': "🔗 Aller au robot",
-    'zh': "🔗 转到机器人",
-    'ar': "🔗 اذهب إلى bot",
+l_act_req = {
+    'ru': "+ запрос",
+    'en': "+ request",
+    'es': "+ solicitud",
+    'fr': "+ demande",
+    'zh': "+ 要求",
+    'ar': "+ طلب",
 }
 
-l_find_category_blog = {
-    'ru': "#блогер",
-    'en': "#blogger",
-    'es': "#bloguero",
-    'fr': "#blogueur",
-    'zh': "#博主",
-    'ar': "#مدَّوِن",
-}
-l_find_category_digit = {
-    'ru': "#оцифровка",
-    'en': "#digitizer",
-    'es': "#digitalizador",
-    'fr': "#numériseur",
-    'zh': "#数字转换器",
-    'ar': "#جهاز التحويل الرقمي",
-}
-l_find_category_smm = {
-    'ru': "#смм",
-    'en': "#smm",
-    'es': "#mmm",
-    'fr': "#nm",
-    'zh': "#嗯",
-    'ar': "#سم",
-}
-l_find_category_recruit = {
-    'ru': "#рекрут",
-    'en': "#recruit",
-    'es': "#recluta",
-    'fr': "#recruter",
-    'zh': "#招募",
-    'ar': "#تجنيد",
-}
-l_find_category_design = {
-    'ru': "#дизайн",
-    'en': "#design",
-    'es': "#diseño",
-    'fr': "#conception",
-    'zh': "#设计",
-    'ar': "#تصميم",
+l_msg_text = {
+    'ru': ": text",
+    'en': ": text",
+    'es': ": texto",
+    'fr': ": texte",
+    'zh': "： 文本",
+    'ar': ": نص",
 }
-l_find_category_coach = {
-    'ru': "#коуч",
-    'en': "#coach",
-    'es': "#entrenador",
-    'fr': "#entraîneur",
-    'zh': "#教练",
-    'ar': "#مدرب",
+l_msg_photo = {
+    'ru': ": фото",
+    'en': ": photo",
+    'es': ": foto",
+    'fr': ": photo",
+    'zh': "： 照片",
+    'ar': ": صورة",
 }
-l_find_category_it = {
-    'ru': "#ИТ",
-    'en': "#DOG",
-    'es': "#PERRO",
-    'fr': "#CHIEN",
-    'zh': "#狗",
-    'ar': "#كلب",
+l_msg_gif = {
+    'ru': ": гиф",
+    'en': ": gif",
+    'es': ": gif",
+    'fr': ": gif",
+    'zh': ": 动图",
+    'ar': ": gif",
 }
-l_find_category_course = {
-    'ru': "#курсы",
-    'en': "#courses",
-    'es': "#cursos",
-    'fr': "#cours",
-    'zh': "#培训班",
-    'ar': "#الدورات",
+l_msg_video = {
+    'ru': ": видео",
+    'en': ": video",
+    'es': ": video",
+    'fr': ": vidéo",
+    'zh': "： 视频",
+    'ar': ": فيديو",
 }
-l_find_category_business = {
-    'ru': "#бизнес",
-    'en': "#business",
-    'es': "#negocio",
-    'fr': "#entreprise",
-    'zh': "#商业",
-    'ar': "#عمل",
+l_msg_video_note = {
+    'ru': ": телескоп",
+    'en': ": telescope",
+    'es': ": telescopio",
+    'fr': ": télescope",
+    'zh': ": 望远镜",
+    'ar': ": تلسكوب",
 }
-l_find_category_goods = {
-    'ru': "#товарка",
-    'en': "#cargo",
-    'es': "#carga",
-    'fr': "#cargaison",
-    'zh': "#货物",
-    'ar': "#البضائع",
+l_msg_audio = {
+    'ru': ": аудио",
+    'en': ": audio",
+    'es': ": sonido",
+    'fr': ": l'audio",
+    'zh': "： 声音的",
+    'ar': ": صوتي",
 }
-l_find_category_offline = {
-    'ru': "#оффлайн",
-    'en': "#offline",
-    'es': "#desconectado",
-    'fr': "#hors ligne",
-    'zh': "#离线",
-    'ar': "#غير متصل على الانترنت",
+l_msg_voice = {
+    'ru': ": голосовое",
+    'en': ": voice",
+    'es': ": voz",
+    'fr': ": voix",
+    'zh': "： 嗓音",
+    'ar': ": صوت",
 }
-l_find_category_lawyer = {
-    'ru': "#юрист",
-    'en': "#lawyer",
-    'es': "#abogado",
-    'fr': "#avocat",
-    'zh': "#律师",
-    'ar': "#محامي",
+l_msg_document = {
+    'ru': ": документ",
+    'en': ": document",
+    'es': ": documento",
+    'fr': ": document",
+    'zh': "： 文档",
+    'ar': ": وثيقة",
 }
-l_find_category_verified = {
-    'ru': "#верифиц",
-    'en': "#verification",
-    'es': "#verificación",
-    'fr': "#vérification",
-    'zh': "#确认",
-    'ar': "#تَحَقّق",
+l_msg_sticker = {
+    'ru': ": стикер",
+    'en': ": sticker",
+    'es': ": pegatina",
+    'fr': ": autocollant",
+    'zh': "： 贴纸",
+    'ar': ": ملصق",
 }
-l_find_category_premium = {
-    'ru': "#премиум",
-    'en': "#premium",
-    'es': "#de primera calidad",
-    'fr': "#prime",
-    'zh': "#优质的",
-    'ar': "#غالي",
+l_msg_quiz = {
+    'ru': ": опрос",
+    'en': ": survey",
+    'es': ": encuesta",
+    'fr': ": enquête",
+    'zh': "： 民意调查",
+    'ar': ": استطلاع",
 }
-l_find_category_health = {
-    'ru': "#здоровье",
-    'en': "#health",
-    'es': "#salud",
-    'fr': "#santé",
-    'zh': "#健康",
-    'ar': "#صحة",
+l_msg_dice = {
+    'ru': ": игра",
+    'en': ": game",
+    'es': ": juego",
+    'fr': ": jeu",
+    'zh': "： 游戏",
+    'ar': ": لعبة",
 }
 
-l_find_category_getting = {
-    'ru': "🔎 Выгружаем <b>категорию</b> {0}..\n\n#длительность 0мин",
-    'en': "🔎 Upload <b>category</b> {0}..\n\n#duration 0min",
-    'es': "🔎 Subir <b>categoría</b> {0}..\n\n#duración 0min",
-    'fr': "🔎 <b>Catégorie</b> de téléchargement {0}..\n\n#durée 0min",
-    'zh': "🔎 上传<b>类别</b>{0}..\n\n#duration 0min",
-    'ar': "🔎 <b>فئة</b> التحميل {0} ..\n\n# المدة 0 دقيقة",
+l_btn_button_in = {
+    'ru': "✅ Кнопка ↑",
+    'en': "✅ Button ↑",
+    'es': "✅ Botón ↑",
+    'fr': "✅ Bouton ↑",
+    'zh': "✅按钮↑",
+    'ar': "✅ زر ↑",
 }
-l_find_keyword_getting = {
-    'ru': "🔎 Выгружаем базу по ключевым словам <i>{0}</i>..\n\n#длительность 1мин",
-    'en': "🔎 Unload the database by keywords <i>{0}</i> ..\n\n#duration 1 min",
-    'es': "🔎 Descarga la base de datos por palabras clave <i>{0}</i> ..\n\n#duración 1 min",
-    'fr': "🔎 Décharger la base de données par mots clés <i>{0}</i> ..\n\n#durée 1 min",
-    'zh': "🔎 通过关键字<i>{0}</i>卸载数据库 ..\n\n#duration 1 分钟",
-    'ar': "🔎 تفريغ قاعدة البيانات بالكلمات الأساسية <i>{0}</i> ..\n\n# المدة 1 دقيقة",
+l_btn_link = {
+    'ru': "🔗 Ссылка",
+    'en': "🔗 Link",
+    'es': "🔗 Enlace",
+    'fr': "🔗 Lien",
+    'zh': "🔗 链接",
+    'ar': "🔗 رابط",
 }
-l_find_category_keywords = {
-    'ru': "📰 <b>Введи</b> ключевые слова для поиска через пробелы или разделители",
-    'en': "📰 <b>Enter</b> keywords to search through spaces or delimiters",
-    'es': "📰 <b>Ingrese</b> palabras clave para buscar a través de espacios o delimitadores",
-    'fr': "📰 <b>Entrez</b> des mots-clés pour rechercher dans des espaces ou des délimiteurs",
-    'zh': "📰<b>输入</b>关键字以通过空格或分隔符进行搜索",
-    'ar': "📰 <b>أدخل</b> كلمات أساسية للبحث من خلال المسافات أو المحددات",
+l_btn_pay = {
+    'ru': "💳 Оплата",
+    'en': "💳 Payment",
+    'es': "💳 Pago",
+    'fr': "💳 Paiement",
+    'zh': "💳付款",
+    'ar': "💳 الدفع",
 }
-l_find_reached = {
-    'ru': "<b>Охват</b>: <u>{0}</u> польз.",
-    'en': "<b>Reach</b> : <u>{0}</u> users",
-    'es': "<b>Alcance</b> : <u>{0}</u> usuarios",
-    'fr': "<b>Atteignez</b> : <u>{0}</u> utilisateurs",
-    'zh': "<b>覆盖</b>： <u>{0}</u>个用户",
-    'ar': "<b>الوصول</b> : <u>{0}</u> مستخدمين",
+l_btn_search = {
+    'ru': "🔎 Поиск",
+    'en': "🔎 Search",
+    'es': "🔎 Buscar",
+    'fr': "🔎 Rechercher",
+    'zh': "🔎 搜索",
+    'ar': "🔎 بحث",
 }
-l_find_watch = {
-    'ru': "🔎 Просмотр",
-    'en': "🔎 View",
-    'es': "🔎 Ver",
-    'fr': "🔎 Voir",
-    'zh': "🔎 查看",
-    'ar': "🔎 عرض",
+l_btn_like = {
+    'ru': "❤️ Лайк",
+    'en': "❤️ Like",
+    'es': "❤️ Me gusta",
+    'fr': "❤️ J'aime",
+    'zh': "❤️喜欢",
+    'ar': "❤️ مثل",
 }
-l_add_text = {
-    'ru': "🔎 <b>Добавь</b> свой канал/группу/пользователя/бота в базу командой: /add ССЫЛКА\n\n👩🏽‍💻 Условия: наличие аватара и @username/ссылки (+ для канала/группы > 100 участников + последнее сообщение < 100 дней назад + для бота и пользователя наличие описания)",
-    'en': "🔎 Add your channel/group/user/bot to the database with the command: /add ССЫЛКА\n\n👩🏽‍💻 Conditions: availability of an avatar and @username /link (+ for channel/group > 100 members + last message < 100 days ago + for the bot and the user, the presence of a description)",
-    'es': "🔎 Agregue su canal/grupo/usuario/bot a la base de datos con el comando: /add ССЫЛКА\n\n👩🏽‍💻 Condiciones: disponibilidad de un avatar y @username /link (+ para canal/grupo > 100 miembros + último mensaje < hace 100 días + para el bot y el usuario, la presencia de una descripción)",
-    'fr': "🔎 Ajoutez votre chaîne/groupe/utilisateur/bot à la base de données avec la commande : /add ССЫЛКА\n\n👩🏽‍💻 Conditions : disponibilité d'un avatar et @username /link (+ pour chaîne/groupe > 100 membres + dernier message il y a < 100 jours + pour le bot et l'utilisateur, la présence d'une description)",
-    'zh': "🔎 使用以下命令将您的频道/组/用户/机器人添加到数据库： /add ССЫЛКА\n\n👩🏽‍💻 条件：头像和@username /link 的可用性（+ 对于频道/组 > 100 个成员 + 最后一个消息 < 100 天前 + 对于机器人和用户，存在描述）",
-    'ar': "🔎 أضف قناتك / مجموعتك / مستخدم / بوت إلى قاعدة البيانات بالأمر: /add ССЫЛКА\n\n👩🏽‍💻 الشروط: توفر الصورة الرمزية و @username / الرابط (+ للقناة / المجموعة> 100 عضو + الأخير رسالة <100 يوم مضت + للبوت والمستخدم ، وجود وصف)",
+l_btn_button_kb = {
+    'ru': "✅ Кнопка ↓",
+    'en': "✅ Button ↓",
+    'es': "✅ Botón ↓",
+    'fr': "✅ Bouton ↓",
+    'zh': "✅按钮↓",
+    'ar': "✅ زر ↓",
 }
-l_add_join_err = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> (вставь корректную ссылку или повтори позже)",
-    'en': "🚫 Failed to add {0} to the database, you need to open free access to join",
-    'es': "🚫 No se pudo agregar {0} a la base de datos, debe abrir el acceso gratuito para unirse",
-    'fr': "🚫 Échec de l'ajout de {0} à la base de données, vous devez ouvrir un accès gratuit pour rejoindre",
-    'zh': "🚫 添加{0}到数据库失败，需要开通免费权限才能加入",
-    'ar': "🚫 فشل إضافة {0} إلى قاعدة البيانات ، تحتاج إلى فتح وصول مجاني للانضمام",
+l_btn_phone = {
+    'ru': "📞 Сотовый",
+    'en': "📞 Cellular",
+    'es': "📞 Celular",
+    'fr': "📞 Cellulaire",
+    'zh': "📞 手机",
+    'ar': "📞 خلوي",
 }
-
-l_add_chn_fail = {
-    'ru': "🚫 <b>Канал</b> {0} не добавлен в базу\n\n{1} аватар\n{2} >{4} подписчиков\n{3} последний пост <{5} дней назад",
-    'en': "🚫 Channel {0} - not added to the database\n\n{1} avatar\n{2} >100 subscribers\n{3} last post <100 days ago",
-    'es': "🚫 Canal {0} - no agregado a la base de datos\n\n{1} avatar\n{2} >100 suscriptores\n{3} última publicación <100 días atrás",
-    'fr': "🚫 Chaîne {0} - non ajoutée à la base de données\n\n{1} avatar\n{2} >100 abonnés\n{3} dernier message il y a <100 jours",
-    'zh': "🚫 频道 {0} - 未添加到数据库\n\n{1} 头像\n{2} >100 个订阅者\n{3} 上次发布 <100 天前",
-    'ar': "🚫 القناة {0} - لم تتم إضافتها إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2}> 100 مشترك\n{3} آخر مشاركة قبل أقل من 100 يوم",
+l_btn_geo = {
+    'ru': "📍 Гео",
+    'en': "📍 Geo",
+    'es': "📍 Geo",
+    'fr': "📍 Géo",
+    'zh': "📍地理",
+    'ar': "📍 جيو",
 }
-l_add_grp_fail = {
-    'ru': "🚫 <b>Группа</b> {0} не добавлена в базу\n\n{1} аватар\n{2} >{4} участников\n{3} последний пост <{5} дней назад",
-    'en': "🚫 Group {0} - not added to the database\n\n{1} avatar\n{2} >100 members\n{3} last post <100 days ago",
-    'es': "🚫 Grupo {0} - no agregado a la base de datos\n\n{1} avatar\n{2} >100 miembros\n{3} última publicación <100 días atrás",
-    'fr': "🚫 Groupe {0} - non ajouté à la base de données\n\n{1} avatar\n{2} >100 membres\n{3} dernier message il y a <100 jours",
-    'zh': "🚫 组 {0} - 未添加到数据库\n\n{1} 头像\n{2} >100 名成员\n{3} 上次发帖 <100 天前",
-    'ar': "🚫 المجموعة {0} - لم تتم إضافتها إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2}> 100 عضو\n{3} آخر مشاركة منذ أقل من 100 يوم",
+l_btn_blog = {
+    'ru': "📰 Блог",
+    'en': "📰 Blog",
+    'es': "📰Blog",
+    'fr': "📰 Blogue",
+    'zh': "📰 博客",
+    'ar': "📰 مدونة",
 }
-l_add_usr_fail = {
-    'ru': "🚫 <b>Пользователь</b> {0} не добавлен в базу\n\n{1} аватар\n{2} @username\n{3} био",
-    'en': "🚫 User {0} - not added to database\n\n{1} avatar\n{2} @username\n{3} bio",
-    'es': "🚫 Usuario {0}: no agregado a la base de datos\n\n{1} avatar\n{2} @username\n{3} biografía",
-    'fr': "🚫 Utilisateur {0} - non ajouté à la base de données\n\n{1} avatar\n{2} @username\n{3} bio",
-    'zh': "🚫 用户 {0} - 未添加到数据库\n\n{1} 头像\n{2} @username\n{3} 简介",
-    'ar': "🚫 المستخدم {0} - لم تتم إضافته إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2} @username\n{3} السيرة الذاتية",
+l_btn_name = {
+    'ru': "Имя:",
+    'en': "Name:",
+    'es': "Nombre:",
+    'fr': "Nom:",
+    'zh': "姓名：",
+    'ar': "اسم:",
 }
-l_add_bot_fail = {
-    'ru': "🚫 <b>Бот</b> {0} не добавлен в базу\n\n{1} аватар\n{2} описание",
-    'en': "🚫 Bot {0} - not added to the database\n\n{1} avatar\n{2} description",
-    'es': "🚫 Bot {0} - no agregado a la base de datos\n\n{1} avatar\n{2} descripción",
-    'fr': "🚫 Bot {0} - non ajouté à la base de données\n\n{1} description de l'avatar\n{2}",
-    'zh': "🚫 机器人 {0} - 未添加到数据库\n\n{1} 头像\n{2} 描述",
-    'ar': "🚫 بوت {0} - لم تتم إضافته إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2} الوصف",
+l_btn_type = {
+    'ru': "Тип:",
+    'en': "Type:",
+    'es': "Tipo:",
+    'fr': "Taper:",
+    'zh': "类型：",
+    'ar': "يكتب:",
 }
 
-l_add_chn_done = {
-    'ru': "✅ <b>Канал</b> {0} - добавлен в базу и обновлен",
-    'en': "✅ Channel {0} - added to the database and updated",
-    'es': "✅ Canal {0}: agregado a la base de datos y actualizado",
-    'fr': "✅ Chaîne {0} - ajoutée à la base de données et mise à jour",
-    'zh': "✅ 频道 {0} - 添加到数据库并更新",
-    'ar': "✅ القناة {0} - تمت إضافتها إلى قاعدة البيانات وتحديثها",
-}
-l_add_grp_done = {
-    'ru': "✅ <b>Группа</b> {0} - добавлена в базу и обновлена",
-    'en': "✅ Group {0} - added to the database and updated",
-    'es': "✅ Grupo {0}: agregado a la base de datos y actualizado",
-    'fr': "✅ Groupe {0} - ajouté à la base de données et mis à jour",
-    'zh': "✅ 组 {0} - 添加到数据库并更新",
-    'ar': "✅ المجموعة {0} - تمت إضافتها إلى قاعدة البيانات وتحديثها",
-}
-l_add_usr_done = {
-    'ru': "✅ <b>Пользователь</b> {0} - добавлен в базу и обновлен",
-    'en': "✅ User {0} - added to the database and updated",
-    'es': "✅ Usuario {0}: agregado a la base de datos y actualizado",
-    'fr': "✅ Utilisateur {0} - ajouté à la base de données et mis à jour",
-    'zh': "✅ 用户 {0} - 添加到数据库并更新",
-    'ar': "✅ المستخدم {0} - تمت إضافته إلى قاعدة البيانات وتحديثها",
+l_check_box_pin_message = {
+    'ru': "Закреп сообщения",
+    'en': "Pin messages",
+    'es': "Anclar mensajes",
+    'fr': "Épingler les messages",
+    'zh': "固定消息",
+    'ar': "تثبيت الرسائل",
 }
-l_add_bot_done = {
-    'ru': "✅ <b>Бот</b> {0} - добавлен в базу и обновлен",
-    'en': "✅ Bot {0} - added to the database and updated",
-    'es': "✅ Bot {0}: agregado a la base de datos y actualizado",
-    'fr': "✅ Bot {0} - ajouté à la base de données et mis à jour",
-    'zh': "✅ Bot {0} - 添加到数据库并更新",
-    'ar': "✅ بوت {0} - تمت إضافته إلى قاعدة البيانات وتحديثها",
+l_check_box_protect_message = {
+    'ru': "Защита сообщения",
+    'en': "Message protection",
+    'es': "Protección de mensajes",
+    'fr': "Protection des messages",
+    'zh': "消息保护",
+    'ar': "حماية الرسائل",
 }
-
-l_find_chn_done = {
-    'ru': "🔥 <b>Готово!</b> По {0} собрано <u>{1}</u> каналов, сегментированных по <i>ключевым</i> словам\n\n<b>Охват</b>: <u>{2}</u> польз\n\nМожно связаться с администраторами каналов, чтобы заказать рекламу",
-    'en': "🔥 <b>Done!</b> {0} collected <u>{1}</u> channels segmented by <i>keywords</i>\n\n<b>Reach</b> : <u>{2}</u> users\n\nYou can contact channel administrators to order advertising",
-    'es': "🔥 <b>Listo!</b> {0} recopilaron <u>{1}</u> canales segmentados por <i>palabras clave</i>\n\n<b>Alcance</b> : <u>{2}</u> usuarios\n\nPuede ponerse en contacto con los administradores del canal para solicitar publicidad",
-    'fr': "🔥 <b>C&#x27;est fait !</b> {0} a collecté <u>{1}</u> chaînes segmentées par <i>mots-clés</i>\n\n<b>Atteinte</b> : <u>{2}</u> utilisateurs\n\nVous pouvez contacter les administrateurs de chaîne pour commander de la publicité",
-    'zh': "🔥<b>完成！</b> {0} 收集了<u>{1} 个</u>按<i>关键字</i>细分的频道\n\n<b>覆盖</b>： <u>{2} 个</u>用户\n\n您可以联系频道管理员订购广告",
-    'ar': "🔥 <b>انتهى!</b> القنوات {0} المجمعة <u>{1}</u> المقسمة حسب <i>الكلمات الرئيسية</i>\n\n<b>الوصول إلى</b> : <u>{2}</u> المستخدمين\n\nيمكنك الاتصال بمسؤولي القناة لطلب الإعلانات",
+l_check_box_edit_message = {
+    'ru': "Изменить текущее сообщение",
+    'en': "Edit current message",
+    'es': "Editar mensaje actual",
+    'fr': "Modifier le message actuel",
+    'zh': "编辑当前消息",
+    'ar': "تحرير الرسالة الحالية",
 }
-l_find_grp_done = {
-    'ru': "🔥 <b>Готово!</b> По {0} собрано <u>{1}</u> чатов, сегментированных по <i>ключевым</i> словам\n\n<b>Охват</b>: <u>{2}</u> польз\n\nМожно сделать <b>рассылку</b> по группам",
-    'en': "🔥 <b>Done!</b> {0} collected <u>{1}</u> chats, segmented by <i>keywords</i>\n\n<b>Reach</b> : <u>{2}</u> users\n\nCan be <b>sent</b> to groups",
-    'es': "🔥 <b>Listo!</b> {0} <u>{1}</u> chats recopilados, segmentados por <i>palabras clave</i>\n\n<b>Alcance</b> : <u>{2}</u> usuarios\n\nSe puede <b>enviar</b> a grupos",
-    'fr': "🔥 <b>C&#x27;est fait !</b> {0} a collecté <u>{1}</u> chats, segmentés par <i>mots-clés</i>\n\n<b>Atteinte</b> : <u>{2}</u> utilisateurs\n\nPeut être <b>envoyé</b> à des groupes",
-    'zh': "🔥<b>完成！</b> {0} 收集了<u>{1} 个</u>聊天，按<i>关键字细分</i>\n\n<b>覆盖</b>： <u>{2} 个</u>用户\n\n可以<b>发送</b>到组",
-    'ar': "🔥 <b>انتهى!</b> {0} دردشات <u>{1}</u> مجمعة ، مقسمة حسب <i>الكلمات الرئيسية</i>\n\n<b>مدى الوصول</b> : <u>{2}</u> مستخدمين\n\nيمكن <b>إرسالها</b> إلى مجموعات",
+l_check_box_auto_format = {
+    'ru': "Авто формат сообщения",
+    'en': "Auto message format",
+    'es': "Formato de mensaje automático",
+    'fr': "Format de message automatique",
+    'zh': "自动消息格式",
+    'ar': "تنسيق الرسالة التلقائي",
 }
-l_find_usr_done = {
-    'ru': "🔥 <b>Готово!</b> По {0} собрано <u>{1}</u> пользователей, сегментированных по <i>ключевым</i> словам\n\nМожно сразу сделать <b>рассылку</b> или подписку-<b>инвайт</b> в чат по <i>полученным</i> лидам",
-    'en': "🔥 <b>Done!</b> {0} collected <u>{1}</u> users, segmented by <i>keywords</i>\n\nYou can immediately make <b>a mailing list</b> or subscribe <b>- invite</b> to the chat according to <i>the received</i> leads",
-    'es': "🔥 <b>Listo!</b> {0} recolectó <u>{1}</u> usuarios, segmentados por <i>palabras clave</i>\n\nPuede crear <b>una lista de correo</b> o suscribirse inmediatamente <b>: invite</b> al chat de acuerdo con <i>los clientes potenciales recibidos</i>",
-    'fr': "🔥 <b>C&#x27;est fait !</b> {0} utilisateurs collectés <u>{1}</u> , segmentés par <i>mots-clés</i>\n\nVous pouvez immédiatement créer <b>une liste de diffusion</b> ou vous abonner <b>- inviter</b> au chat en fonction <i>des prospects reçus</i>",
-    'zh': "🔥<b>完成！</b> {0} 收集了<u>{1} 个</u>用户，按<i>关键字</i>细分\n\n您可以立即制作<b>邮件列表</b>或订阅<b>-</b>根据<i>收到的</i>线索邀请聊天",
-    'ar': "🔥 <b>انتهى!</b> {0} تم تجميع <u>{1}</u> مستخدمين ، مقسمين حسب <i>الكلمات الرئيسية</i>\n\nيمكنك على الفور إنشاء <b>قائمة بريدية</b> أو الاشتراك <b>- قم بدعوة</b> إلى الدردشة وفقًا للعملاء <i>المحتملين المستلمين</i>",
+l_check_box_auto_typing = {
+    'ru': "Авто печатание сообщения",
+    'en': "Auto typing message",
+    'es': "Mensaje de escritura automática",
+    'fr': "Message de saisie automatique",
+    'zh': "自动输入信息",
+    'ar': "رسالة الكتابة التلقائية",
 }
-l_find_bot_done = {
-    'ru': "🔥 <b>Готово!</b> По {0} собрано <u>{1}</u> ботов, сегментированных по <i>ключевым</i> словам",
-    'en': "🔥 <b>Done!</b> {0} collected <u>{1}</u> bots segmented by <i>keywords</i>",
-    'es': "🔥 <b>Listo!</b> {0} recopilaron <u>{1}</u> bots segmentados por <i>palabras clave</i>",
-    'fr': "🔥 <b>C&#x27;est fait !</b> {0} collecté <u>{1}</u> bots segmentés par <i>mots-clés</i>",
-    'zh': "🔥<b>完成！</b> {0} 收集了<u>{1} 个</u><i>按关键字</i>细分的机器人",
-    'ar': "🔥 <b>انتهى!</b> {0} جمعت <u>{1}</u> برامج التتبع مقسمة حسب <i>الكلمات الرئيسية</i>",
+l_check_box_preview = {
+    'ru': "Превью контент",
+    'en': "Preview content",
+    'es': "Vista previa del contenido",
+    'fr': "Prévisualiser le contenu",
+    'zh': "预览内容",
+    'ar': "معاينة المحتوى",
 }
-l_hashtag_categories = {
-    "BLOG": ["blog", "блог", "влог", "блогер", "контентмейкер", 'contentmaker', 'youtube', 'путешестви',
-             "курс", 'getcourse', 'геткурс', "английск", 'школ', "school", "запуск", 'заняти', 'урок', 'воркшоп',
-             "language", "онлайн-школ", "онлайн школ", 'лингвист', 'linguist', 'марафон', 'практикум', 'семинар',
-             'вебинар', 'лаборатор', 'хакатон', 'интенсив', 'обучени', 'запуск', 'колледж', 'институт',
-             'университет', 'лекци', 'мастермайнд', 'симпозиум', 'тренинг', 'тимбилдинг', 'мастерск', 'образовани'],
-    "DIGIT": ['оцифров', "фин.", 'финан', 'бух', 'инвест', 'франш', 'трейд', 'бирж', 'кредит', "учет",
-              "банк", "торг", "кассы", "денежн", "консалт", 'consult', 'finan', 'business', "доход"],
-    "SMM": ['smm', 'смм', 'инста', 'inst', "facebook", 'tiktok', "тикток", 'tik-tok', "тик-ток", 'youtube', 'маркето',
-            'маркети', 'market', 'таргет', "target", 'распаковка', 'продвижение', 'seo', 'сео', 'бренд', "агентство",
-            "лиды", "vkontakte", "вконтакте", "лидов", "реклам", 'taplink', "прогрев", "блог", "визуал", "запуск",
-            "трафик", "mvp", "редакция",
-            'директ'],
-    "RECRUIT": ["рекрут", "роп", "работа", "фриланc", "freela", "найм", "hr", "pr", "персонал", "менеджер",
-                "продаж", "ассист", "риелтор", 'млм', 'mlm', "управлен", "наем", "сотрудн", "делегир", "карьер"],
-    "DESIGN": ["дизайн", "design", "интерьер", "декор", "мебел", "3d", "архитект", "двери", "ремонт", "строител",
-               "фасад", 'тексти', "рису", "креатив", "визуал", "ландшафт", "художн", "картин",
-               "имидж", "камин", "монтаж", 'граф', 'искусств', 'рукодел'],
-    "COACH": ["коуч", "coach", 'консульт', 'продюсер', "бизнес", "наставн", "оратор", "энерг", "эксперт", "психо",
-              "трекер", 'гайд',
-              "практик", "бренд", "тайм", "мотива", "логопед", "мышлен", "нумеролог", "таролог", "йог",
-              "ментор", "тренер", "гештальт", "предприним", "метафори", "денеж", "диагност", "icf"],
-    "IT": ["лендинг", "crm", 'kotlin', 'swift', 'flutter', 'c++', 'c#', 'unity', 'angular',
-           'amocrm', "powerbi", 'программирова', 'tilda', 'frontend', 'backend', 'python', 'ux/ui',
-           "битрикс", 'автоматизаци', 'автоворон', 'разработч', 'java',
-           "developer", 'блокчейн', 'blockchain', 'startup', 'coding'],
-    "BUSINESS": ["business", "бизнес", "инвест", "франш", "кредит", "торг", "консалт", "consult",
-                 "доход", "представит", "предпринимат", "коммерц", "фирм", "предприят", "компани", "промышл",
-                 "производст", "invest", "капитал", "capital", "корпорац", "агентств", "пассив",
-                 "дистриб", "акцио", "холдин", "прибыл", "рубл", "стартап", 'startup'],
-    "GOODS": ["wildbe", "вайлд", 'ozon', "озон", 'avito', "авито", "авторск", "одежд", "китай",
-              "китая", "складчина", "подарк", 'модн', 'маркетплейс', 'вещи'],
-    "OFFLINE": ["салон", "студи", "логист", "грузопер", 'свечи', "маникюр", "макияж", "букеты", "клиник",
-                "косметол", "магазин", "производств", 'эпиляц', 'парикмах', "ресниц", 'beauty', "кондитер",
-                'бьюти', "пищев", 'кулинар', 'оффлайн', 'offline', 'адрес', 'храм', 'церковь', 'транспорт',
-                'ресторан', 'недвижимость'],
-    "HEALTH": ["beautifull", "beauty", "бьюти", "красота", "здоров", 'нутрициолог', 'косметик', 'косметол', 'йога',
-               'питани', 'доктор', 'диет', 'похуден', 'волос', 'маникюр', 'макияж', 'клиник', 'ресниц', 'эпиляц',
-               'парикмах', 'nutrition', 'krasota', 'zdorov', 'dietol', 'медицин', 'medic', 'стоматол',
-               'врач', 'vrach', 'yoga', 'фитнес', 'fitnes', 'медиц', 'медик', 'лекарств', 'спортив', 'sport',
-               'семья',
-               'дети', 'ребенок'],
+l_check_box_spoiler = {
+    'ru': "Гиф/фото/видео спойлер",
+    'en': "GIF/photo/video spoiler",
+    'es': "Spoiler de GIF/foto/video",
+    'fr': "Spoiler GIF/photo/vidéo",
+    'zh': "GIF/照片/视频剧透",
+    'ar': "مفسد GIF / صور / فيديو",
 }
-l_hashtag_translate = {
-    "BLOG": {
-        'ru': "#блоггер",
-        'en': "#blogger",
-        'es': "#blogger",
-        'fr': "#blogger",
-        'zh': "#blogger",
-        'ar': "#blogger",
-    },
-    "DIGIT": {
-        'ru': "#оцифровка",
-        'en': "#digit",
-        'es': "#blogger",
-        'fr': "#blogger",
-        'zh': "#blogger",
-        'ar': "#blogger",
-    },
-    "SMM": {
-        'ru': "#смм",
-        'en': "#smm",
-        'es': "#blogger",
-        'fr': "#blogger",
-        'zh': "#blogger",
-        'ar': "#blogger",
-    },
-    "RECRUIT": {
-        'ru': "#рекрут",
-        'en': "#recruit",
-        'es': "#blogger",
-        'fr': "#blogger",
-        'zh': "#blogger",
-        'ar': "#blogger",
-    },
-    "DESIGN": {
-        'ru': "#дизайн",
-        'en': "#design",
-        'es': "#blogger",
-        'fr': "#blogger",
-        'zh': "#blogger",
-        'ar': "#blogger",
-    },
-    "COACH": {
-        'ru': "#коуч",
-        'en': "#coach",
-        'es': "#blogger",
-        'fr': "#blogger",
-        'zh': "#blogger",
-        'ar': "#blogger",
-    },
-    "IT": {
-        'ru': "#ИТ",
-        'en': "#IT",
-        'es': "#blogger",
-        'fr': "#blogger",
-        'zh': "#blogger",
-        'ar': "#blogger",
-    },
-    "BUSINESS": {
-        'ru': "#бизнес",
-        'en': "#business",
-        'es': "#blogger",
-        'fr': "#blogger",
-        'zh': "#blogger",
-        'ar': "#blogger",
-    },
-    "GOODS": {
-        'ru': "#товарка",
-        'en': "#goods",
-        'es': "#blogger",
-        'fr': "#blogger",
-        'zh': "#blogger",
-        'ar': "#blogger",
-    },
-    "OFFLINE": {
-        'ru': "#оффлайн",
-        'en': "#offline",
-        'es': "#blogger",
-        'fr': "#blogger",
-        'zh': "#blogger",
-        'ar': "#blogger",
-    },
-    "HEALTH": {
-        'ru': "#здоровье",
-        'en': "#health",
-        'es': "#blogger",
-        'fr': "#blogger",
-        'zh': "#blogger",
-        'ar': "#blogger",
-    },
-    "ISVERIFIED": {
-        'ru': "#верифиц",
-        'en': "#virified",
-        'es': "#blogger",
-        'fr': "#blogger",
-        'zh': "#blogger",
-        'ar': "#blogger",
-    },
-    "ISPREMIUM": {
-        'ru': "#премиум",
-        'en': "#premium",
-        'es': "#blogger",
-        'fr': "#blogger",
-        'zh': "#blogger",
-        'ar': "#blogger",
-    },
+l_check_box_silence = {
+    'ru': "Тихое сообщение",
+    'en': "Quiet message",
+    'es': "Mensaje tranquilo",
+    'fr': "Message silencieux",
+    'zh': "悄悄话",
+    'ar': "رسالة هادئة",
 }
+# endregion
+# endregion
 
-l_find_alert = {
-    'ru': "👩🏽‍💻 <b>Жми</b> на ✅/☑️, чтобы вкл/выкл <i>уведомления</i> о Telegram-заказчиках в freelance-группах/каналах\n\n🔔 Например, <i>#ищу ассистента для ведения Telegram-канала или #search разработчик telegram-ботов</i>",
-    'en': "👩🏽‍💻 <b>Click</b> on ✅/☑️ to turn on/off <i>notifications</i> about Telegram customers in freelance groups/channels\n\n🔔 For example, <i>#ищу</i> <i>an assistant to maintain a Telegram channel or</i> <i>#search</i> <i>a telegram bot developer</i>",
-    'es': "👩🏽‍💻 <b>Haz clic</b> en ✅/☑️ para activar/desactivar <i>las notificaciones</i> sobre los clientes de Telegram en grupos/canales independientes\n\n🔔 Por ejemplo, <i>#ищу</i> <i>un asistente para mantener un canal de Telegram o</i> <i>#search</i> <i>un desarrollador de bots de Telegram</i>",
-    'fr': "👩🏽‍💻 <b>Cliquez</b> sur ✅/☑️ pour activer/désactiver <i>les notifications</i> concernant les clients Telegram dans les groupes/canaux indépendants\n\n🔔 Par exemple, <i>#ищу</i> <i>un assistant pour gérer un canal Telegram ou</i> <i>#search</i> <i>un développeur de bot Telegram</i>",
-    'zh': "👩🏽‍💻<b>点击</b>✅/☑️ 开启/关闭自由群组/频道中有关 Telegram 客户的<i>通知</i>\n\n🔔 例如， <i>#ищу维护</i><i> Telegram 频道的助手或#search一个 telegram 机器人开发者</i>",
-    'ar': "👩🏽‍💻 <b>انقر</b> فوق ✅ / ☑️ لتشغيل / إيقاف تشغيل <i>الإشعارات</i> حول عملاء Telegram في مجموعات / قنوات مستقلة\n\n🔔 على سبيل المثال ، <i>#ищу</i> <i>مساعد للحفاظ على قناة Telegram أو</i> <i>#search</i> <i>مطور برامج Telegram bot</i>",
-}
-l_find_need_subscribe = {
-    'ru': "👩🏽‍💻 <b>Для</b> получения ссылки на сообщение и заказчика оформи подписку на @FereyFindBot-бота:\n\nhttps://t.me",
-    'en': "👩🏽‍💻 <b>To</b> get a link to the message and the customer, subscribe to @FereyFindBot -bot:\n\nhttps://t.me",
-    'es': "👩🏽‍💻 <b>Para</b> obtener un enlace al mensaje y al cliente, suscríbete a @FereyFindBot -bot:\n\nhttps://t.me",
-    'fr': "👩🏽‍💻 <b>Pour</b> obtenir un lien vers le message et le client, abonnez-vous à @FereyFindBot -bot :\n\nhttps://t.me",
-    'zh': "👩🏽‍💻<b>要</b>获取消息和客户的链接，请订阅@FereyFindBot -bot：\n\nhttps://t.me",
-    'ar': "👩🏽‍💻 <b>للحصول</b> على ارتباط للرسالة والعميل ، اشترك في @FereyFindBot -bot:\n\nhttps: //t.me",
+
+# region FereyUserBot
+l_subscribe_user = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️до 5 <b>рассылок</b> пользователям\n▪️<b>авто-ответ</b> с chatgpt\n▪️<b>экстра</b> бот\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 # endregion
 
 
 # region FereyChannelBot
 l_chn_btn1 = {
     'ru': "⛰️ Каналы",
@@ -3016,16 +2358,16 @@
     'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> администрирования <b>Telegram</b>-каналов:\n\n▪️<b>защита</b> канала от вступления шпионов\n▪️<b>организация</b> бана и антифлуда\n▪️<b>сбор</b> подписчиков\n▪️<b>счетчик</b> нажатий\n▪️<b>реакции</b> и просмотры\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to the <b>Telegram</b> channel администрирования <i>landing bot</i> :\n\n▪️ <b>protection</b> of the channel from spyware entry\n▪️display <b>of statistics</b> and engagement (%)\n▪️restriction of rights before <b>subscribing</b> to the channel\n▪️ <b>organization</b> of a ban and anti-flood\n\n❗️you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> администрирования de canales <b>de Telegram</b> :\n\ <b>n▪️protección</b> del canal contra la entrada de software espía\n▪️visualización <b>de estadísticas</b> e interacción (%)\n▪️restricción de derechos antes de <b>suscribirse</b> al canal\n▪️ <b>organización</b> de una prohibición y anti-inundación\n\n❗️también puedes encargar el desarrollo de un chatbot en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue dans le <i>landing bot</i> администрирования de la chaîne <b>Telegram</b> :\n\n▪️ <b>protection</b> de la chaîne contre l&#x27;entrée de logiciels espions\n▪️affichage <b>des statistiques</b> et de l&#x27;engagement (%)\n▪️restriction des droits avant de <b>s&#x27;abonner</b> à la chaîne\n<b>▪️organisation</b> d'une interdiction et anti-flood\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio de Ferey",
     'zh': "🌱 {0}，欢迎使用<b>Telegram</b>频道администрирования<i>登陆机器人</i>：\n\n▪️<b>保护</b>频道免受间谍软件入侵\n▪️ 显示<b>统计信息</b>和参与度 (%)\n▪️<b>订阅</b>频道前的权利限制\n▪️<b>组织</b>禁令和反洪水\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت</i> администрирования قناة <b>Telegram</b> :\n\n▪️ <b>حماية</b> القناة من إدخال برامج التجسس\n▪️ <b>عرض الإحصائيات</b> والمشاركة (٪)\n▪️ تقييد الحقوق قبل <b>الاشتراك</b> في القناة\n▪️ <b>تنظيم</b> حظر ومكافحة الفيضانات\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
-l_subscribe_channel= {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>реакции</b> и просмотры\n▪️<b>выгрузка</b> базы пользователей\n\n👩🏽‍💻 /balance",
+l_subscribe_channel = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️до 50 <b>реакций</b> и просмотров\n▪️<b>выгрузка</b> базы пользователей\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
     'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 
@@ -3640,23 +2982,23 @@
     'ar': "🔘️☐ Off مكافحة الغارة",
 }
 # endregion
 
 
 # region cban_
 l_cban_add = {
-    'ru': "🕵🏽 <b>Введи</b> id или @username пользователей  через пробельные символы или разделители, чтобы добавить их в /ban-список (*даже тех, кого нет <u>{0}</u>-файле)\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
+    'ru': "🕵🏽 <b>Введи</b> id или @username пользователей  через <i>пробельные или разделительные</i> символы, чтобы добавить их в /ban-список (*даже тех, кого нет <u>{0}</u>-файле)\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
     'en': "🕵🏽 <b>Enter</b> user id or @username separated by spaces or separators to add them to the /ban list (*even those not in the <u>{0}</u> file)\n\n👩🏽‍💻 <b>Current</b> number of users on the /ban list : <u>{1}</u>",
     'es': "🕵🏽 <b>Ingrese</b> id de usuario o @username usuario separados por espacios o separadores para agregarlos a la lista de /ban (*incluso aquellos que no están en el archivo <u>{0}</u> )\n\n👩🏽‍💻 Número <b>actual</b> de usuarios en la lista de /ban : <u>{1}</u>",
     'fr': "🕵🏽 <b>Entrez</b> id ou @username d&#x27;utilisateur séparés par des espaces ou des séparateurs pour les ajouter à la liste /ban (*même ceux qui ne figurent pas dans le fichier <u>{0}</u> )\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;utilisateurs sur la liste /ban : <u>{1}</u>",
     'zh': "🕵🏽<b>输入</b>用空格或分隔符分隔的用户id或@username ，将他们添加到 /ban 列表（*即使那些不在<u>{0}</u>文件中的）\n\n👩🏽‍💻 /ban 列表中的<b>当前</b>用户数： <u>{1}</u>",
     'ar': "🕵🏽 <b>أدخل</b> id المستخدم أو @username مفصولة بمسافات أو فواصل لإضافتهما إلى / قائمة الحظر (* حتى أولئك غير الموجودين في <u>{0}</u> الملف)\n\n👩🏽‍💻 العدد <b>الحالي</b> للمستخدمين في / قائمة الحظر : <u>{1}</u>",
 }
 l_cban_remove = {
-    'ru': "🕵🏽 <b>Введи</b> id или @username пользователей из <u>{0}</u>-файла через пробельные символы или разделители, чтобы удалить их из /ban-списка\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
+    'ru': "🕵🏽 <b>Введи</b> id или @username пользователей из <u>{0}</u>-файла через <i>пробельные или разделительные</i> символы, чтобы удалить их из /ban-списка\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
     'en': "🕵🏽 <b>Enter</b> id or @username of users from <u>{0}</u> -file separated by spaces or separators to remove them from /ban-list\n\n👩🏽‍💻 <b>Current</b> number of users /ban-list: <u>{1}</u>",
     'es': "🕵🏽 <b>Ingrese</b> id o @username de los usuarios de <u>{0}</u> -archivo separado por espacios o separadores para eliminarlos de /ban-list\n\n👩🏽‍💻 Número <b>actual</b> de usuarios /ban-list: <u>{1}</u>",
     'fr': "🕵🏽 <b>Entrez</b> id ou @username utilisateur des utilisateurs de <u>{0}</u> -fichier séparés par des espaces ou des séparateurs pour les supprimer de /ban-list\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;utilisateurs /ban-list : <u>{1}</u>",
     'zh': "🕵🏽<b>输入</b><u>{0}</u>文件中用户的id或@username ，以空格或分隔符分隔，以将其从 /ban-list 中删除\n\n👩🏽‍💻<b>当前</b>用户数 /ban-list： <u>{1}</u>",
     'ar': "🕵🏽 <b>أدخل</b> id أو @username للمستخدمين من <u>{0}</u> - ملف مفصول بمسافات أو فواصل لإزالتهم من / ban-list\n\n👩🏽‍💻 العدد <b>الحالي</b> للمستخدمين / قائمة الحظر: <u>{1}</u>",
 }
 l_cban_added = {
@@ -3778,14 +3120,15 @@
     'es': "☑️☐ Prohibición de compromiso de Vykl",
     'fr': "☑️☐Vykl pledge-ban",
     'zh': "☑️☐Vykl 质押禁令",
     'ar': "Vykl تعهد الحظر",
 }
 # endregion
 
+
 # region cpost_
 l_cpost_call = {
     'ru': "🔔 Нужно ⚙️Настроить хотя бы один пост",
     'en': "🔔 You need to ⚙️Customize at least one post",
     'es': "🔔 Necesitas ⚙️Personalizar al menos una publicación",
     'fr': "🔔 Vous devez ⚙️Personnaliser au moins une publication",
     'zh': "🔔 你需要⚙️自定义至少一个帖子",
@@ -4065,15 +3408,15 @@
     'en': "🌱 {0}, welcome to <i>the landing bot</i> администрирования <b>Telegram</b> groups:\n\n▪️ <b>protecting</b> the group from spyware\n▪️displaying <b>statistics</b> and engagement (%)\n▪️restricting rights before <b>subscribing</b> to the channel\n▪️ <b>organizing</b> a ban and anti-flood\n\n❗️you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> администрирования grupos <b>de Telegram</b> :\n\ <b>n▪️proteger</b> al grupo de spyware\n▪️mostrar <b>estadísticas</b> e interacción (%)\n▪️restringir los derechos antes de <b>suscribirse</b> al canal\ <b>n▪️organizar</b> un prohibición y anti-inundación\n\n❗️también puede solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue dans <i>le landing bot</i> администрирования des groupes <b>Telegram</b> :\n\n▪️ <b>protéger</b> le groupe des spywares\n▪️afficher <b>les statistiques</b> et l&#x27;engagement (%)\n▪️restreindre les droits avant de <b>s&#x27;abonner</b> à la chaîne\n▪️ <b>organiser</b> un interdiction et anti-flood\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio de Ferey",
     'zh': "🌱 {0}，欢迎使用администрирования <b>Telegram</b>群组的<i>登陆机器人</i>：\n\n▪️<b>保护</b>群组免受间谍软件的侵害\n▪️ 显示<b>统计数据</b>和参与度 (%)\n▪️ 在<b>订阅</b>频道之前限制权利\n▪️<b>组织</b>一个ban 和 anti-flood\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوط</i> администрирования مجموعات <b>Telegram</b> :\n\n▪️ <b>حماية</b> المجموعة من برامج التجسس\n▪️ عرض <b>الإحصائيات</b> والمشاركة (٪)\n▪️ تقييد الحقوق قبل <b>الاشتراك</b> في القناة\n▪️ <b>تنظيم</b> الحظر ومكافحة الفيضانات\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
 l_subscribe_group = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>стоп-слова</b> без ограничений\n▪️<b>старт-слова</b> без ограничений\n\n👩🏽‍💻 /balance",
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️до 50 <b>стоп-слов</b>\n▪️до 10 <b>старт-слова</b>\n▪️до 5 <b>авто-приглашений</b>\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
     'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 
@@ -4645,15 +3988,15 @@
     'en': "🚶🏽 Invite",
     'es': "🚶🏽 invitar",
     'fr': "🚶🏽 Inviter",
     'zh': "🚶🏽邀请",
     'ar': "🚶🏽 دعوة",
 }
 l_parse_start = {
-    'ru': "📇 Начинаем парсинг..",
+    'ru': "📇 <b>Начинаем</b> парсинг..",
     'en': "📇 Let's start parsing..",
     'es': "📇 Empecemos a analizar..",
     'fr': "📇 Commençons l'analyse..",
     'zh': "📇 让我们开始解析..",
     'ar': "📇 لنبدأ في التحليل ..",
 }
 l_ban_handler = {
@@ -5852,15 +5195,15 @@
     'en': "🚀 <b>Current</b> number <i>of start words</i> for post #{0}: <u>{1}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> start words",
     'es': "🚀 Número <b>actual</b> <i>de palabras de inicio</i> para la publicación n.º {0}: <u>{1}</u>\n\n<b>Haga clic</b> en ✅/🚫 para <b>agregar o quitar</b> palabras de inicio",
     'fr': "🚀 Nombre <b>actuel</b> <i>de mots de départ</i> pour le message #{0} : <u>{1}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des mots de départ",
     'zh': "🚀 帖子 #{0} 的<b>当前</b><i>起始词</i>数： <u>{1}</u>\n\n<b>单击</b>✅/🚫<b>添加/删除</b>起始词",
     'ar': "🚀 العدد <b>الحالي</b> <i>لكلمات البداية</i> للنشر # {0}: <u>{1}</u>\n\n<b>انقر</b> على ✅ / 🚫 <b>لإضافة / إزالة</b> كلمات البداية",
 }
 l_cstartoperation_handler = {
-    'ru': "\n\n▪️регистр не важен\n▪️поставь звездочку после слова, чтобы учитывать вхождение\n▪️например, если ввести <b>психо*</b>, то авто-постинг сработает на <u>все</u> сообщения, которые <b>содержат</b> данное сочетание: <i>анти<u>психо</u>лог, <u>Психо</u>терапевт..</i>",
+    'ru': "\n\n▪️регистр не важен\n▪️поставь звездочку в конце слова, чтобы учитывать вхождение\n▪️например, если ввести <b>психо*</b>, то авто-постинг сработает на <u>все</u> сообщения, которые <b>содержат</b> данное сочетание: <i>анти<u>психо</u>лог, <u>Психо</u>терапевт..</i>",
     'en': "\n\n▪️case insensitive\n▪️put an asterisk after the word to take into account the occurrence\n▪️for example, if you enter <b>psycho*</b> , then auto-posting will work on <u>all</u> messages that <b>contain</b> this combination: <i>anti- <u>psychologist</u> , <u>Psycho-</u> therapist. .</i>",
     'es': "\n\n▪️sin distinción entre mayúsculas y minúsculas\n▪️ponga un asterisco después de la palabra para tener en cuenta la ocurrencia\n▪️por ejemplo, si ingresa <b>psico*</b> , la publicación automática funcionará en <u>todos</u> los mensajes que <b>contengan</b> esta combinación: <i>anti- <u>psicóloga</u> , <u>psicoterapeuta</u> .</i>",
     'fr': "\n\n▪️insensible à la casse\n▪️mettre un astérisque après le mot pour prendre en compte l'occurrence\n▪️par exemple, si vous entrez <b>psycho*</b> , alors la publication automatique fonctionnera sur <u>tous</u> les messages qui <b>contiennent</b> cette combinaison : <i>anti- <u>psychologue</u> , <u>Psychothérapeute</u> . .</i>",
     'zh': "\n\n▪️不区分大小写\n▪️在单词后加上星号以考虑出现情况\n▪️例如，如果您输入<b>psycho*</b> ，那么自动发布将对<b>包含</b>此组合的<u>所有</u>消息起作用： <i>anti-<u>心理学家</u>，<u>心理</u>治疗师。。</i>",
     'ar': "\n\n▪️ <i>حالة</i> غير حساسة\n▪️ أدخل علامة النجمة بعد الكلمة لمراعاة الحدوث\n▪️ على سبيل المثال ، إذا أدخلت <b>نفسية *</b> ، فسيعمل النشر التلقائي على <u>جميع</u> الرسائل التي <b>تحتوي على</b> هذه المجموعة: <i><u>عالم نفس</u> ومعالج <u>نفسي</u> .</i>",
 }
 l_cstartoperation_answer = {
@@ -5937,15 +5280,15 @@
     'en': "🧾 Current number of stop words <u>{0}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> stop words",
     'es': "🧾 Número actual de palabras vacías <u>{0}</u>\n\n<b>Haga clic</b> en ✅/🚫 para <b>agregar o</b> quitar palabras vacías",
     'fr': "🧾 Nombre actuel de mots vides <u>{0}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des mots vides",
     'zh': "🧾 当前停用词数<u>{0}</u>\n\n<b>点击</b>✅/🚫<b>添加/删除</b>停用词",
     'ar': "🧾 العدد الحالي لكلمات التوقف <u>{0}</u>\n\n<b>انقر</b> على ✅ / 🚫 <b>لإضافة / إزالة</b> كلمات التوقف",
 }
 l_cstopchange_add = {
-    'ru': "\n\n▪️регистр не важен\n▪️поставь звездочку после слова, чтобы учитывать вхождение\n▪️например, если ввести <b>психо*</b>, то будут удаляться <u>все</u> сообщения, которые <b>содержат</b> данное сочетание: <i>анти<u>психо</u>лог, <u>Психо</u>терапевт..</i>",
+    'ru': "\n\n▪️регистр не важен\n▪️поставь звездочку в конце слова, чтобы учитывать вхождение\n▪️например, если ввести <b>психо*</b>, то будут удаляться <u>все</u> сообщения, которые <b>содержат</b> данное сочетание: <i>анти<u>психо</u>лог, <u>Психо</u>терапевт..</i>",
     'en': "\n\n▪️case insensitive\n▪️put an asterisk after the word to take into account the occurrence\n▪️for example, if you enter <b>psycho*</b> , then <u>all</u> messages that <b>contain</b> this combination will be deleted: <i>anti <u>-psychologist</u> , <u>Psycho-</u> therapist..</i>",
     'es': "\n\n▪️sin distinción entre mayúsculas y minúsculas\n▪️ponga un asterisco después de la palabra para tener en cuenta la ocurrencia\n▪️por ejemplo, si ingresa <b>psico*</b> , se eliminarán <u>todos</u> los mensajes que <b>contengan</b> esta combinación: <i>anti <u>-psicólogo</u> , <u>psico -</u> terapeuta..</i>",
     'fr': "\n\n▪️insensible à la casse\n▪️mettez un astérisque après le mot pour prendre en compte l'occurrence\n▪️par exemple, si vous saisissez <b>psycho*</b> , alors <u>tous</u> les messages qui <b>contiennent</b> cette combinaison seront supprimés : <i>anti <u>-psychologue</u> , <u>Psycho -</u> thérapeute..</i>",
     'zh': "\n\n▪️不区分大小写\n▪️在单词后加一个星号以考虑出现情况\n▪️例如，如果您输入<b>psycho*</b> ，那么<u>所有</u><b>包含</b>此组合的消息都将被删除： <i>anti <u>-psychologist</u> , <u>Psycho -</u>治疗师..</i>",
     'ar': "\n\n▪️ حالة غير حساسة\n▪️ أدخل علامة النجمة بعد الكلمة لمراعاة الحدوث\n▪️ على سبيل المثال ، إذا أدخلت <b>نفسية *</b> ، فسيتم حذف <u>جميع</u> الرسائل التي <b>تحتوي على</b> هذه المجموعة: <i>معاداة النفس ، <u>وطبيب</u> <u>نفسي</u> <u>-</u> معالج ..</i>",
 }
 l_cstopchange_answer = {
@@ -6390,1346 +5733,2071 @@
     'ar': "🗣 غير مسموح بالرسائل <i>مع ملاحظات الفيديو</i>",
 }
 # endregion
 
 # endregion
 
 
-# region FereyBotBot
-l_bot_btn1 = {
-    'ru': "⛰ Боты",
-    'en': "⛰ Bots",
-    'es': "⛰ Bots",
-    'fr': "⛰ Bots",
-    'zh': "⛰ 靴子",
-    'ar': "⛰ أحذية",
+# region FereyAIBot
+l_ai_btn1 = {
+    'ru': "⛰️ Нейросети",
+    'en': "⛰️ Neural networks",
+    'es': "⛰️ Redes neuronales",
+    'fr': "⛰️ Réseaux de neurones",
+    'zh': "⛰️ 神经网络",
+    'ar': "⛰️ الشبكات العصبية",
 }
-l_bot_btn2 = {
+l_ai_btn2 = {
     'ru': "🌬 Подписка",
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
-l_bot_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> автоматизации <b>Telegram</b>-ботов:\n\n▪️авто-постинг и <b>авто-перевод</b>\n▪️<b>авто-ответы</b> и оповещения\n▪️нейросети: графика и текст бота\n▪️интеграции и платежи\n\n❗️также можно заказать разработку чат-бота в нашей <a href='https://t.me/{1}'>ferey</a>-студии",
-    'en': "🌱 {0}, welcome to the <b>Telegram</b> bot автоматизации <i>landing bot</i> :\n\n▪️auto-posting and <b>auto-translation</b>\n▪️ <b>auto-replies</b> and notifications\n▪️integrations and payments\n▪️users and administrators\n\n❗️You can also order the development of a chatbot in our ferey studio",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> автоматизации de bots <b>de Telegram</b> :\n\n▪️auto-publicación y <b>auto-traducción</b>\n▪️auto <b>-respuestas</b> y notificaciones\n▪️integraciones y pagos\n▪️usuarios y administradores\n\n❗️también puedes encargar el desarrollo de un chatbot en nuestro ferey studio",
-    'fr': "🌱 {0}, bienvenue dans le <i>bot d&#x27;atterrissage</i> автоматизации du bot <b>Telegram</b> :\n\n▪️publication et <b>traduction automatiques</b>\n▪️ <b>réponses et notifications automatiques</b>\n▪️intégrations et paiements\n▪️utilisateurs et administrateurs\n\n❗️Vous pouvez également commander le développement d'un chatbot dans notre studio ferey",
-    'zh': "🌱 {0}，欢迎使用<b>Telegram</b>机器人автоматизации<i>登陆机器人</i>：\n\n▪️自动发布和<b>自动翻译</b>\n▪️<b>自动回复</b>和通知\n▪️集成和支付\n▪️用户和管理员\n\n❗️您也可以在我们的ferey工作室订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوط</i> автоматизации لروبوت <b>Telegram</b> :\n\n▪️ النشر التلقائي <b>والترجمة التلقائية</b>\n▪️ <b>الردود التلقائية</b> والإشعارات\n▪️ عمليات الدمج والمدفوعات\nالمستخدمون والمسؤولون\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو ferey الخاص بنا",
+l_ai_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для генерации контента:\n\n▪️<b>текст/изображение</b>\n▪️<b>анализ @telegram-канала</b>\n▪️<b>распознавание</b> речи\n▪️<b>очистка ⁰истории</b> /start\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to the content генерации <i>landing bot</i> :\n\n▪️ <b>text</b>\n▪️ <b>image</b>\n▪️ <b>analysis of the Telegram channel</b>\n\n❗️ you can also order the development of a chat bot in our studio Ferey",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> генерации de contenido :\n\n▪️ <b>texto</b>\n▪️ <b>imagen</b>\n▪️ <b>análisis del canal de Telegram</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue dans le <i>landing bot</i> генерации de contenu :\n\n▪️ <b>texte</b>\n▪️ <b>image</b>\n▪️ <b>analyse de la chaîne Telegram</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎使用内容генерации<i>登陆机器人</i>：\n\n▪️<b>文字</b>\n▪️<b>图片</b>\n▪️ <b>Telegram 频道分析</b>\n\n❗️ 您也可以在我们的工作室Ferey订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت إنشاء</i> генерации :\n\n▪️ <b>نص</b>\n▪️ <b>صورة</b>\n▪️ <b>تحليل قناة Telegram</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
-l_subscribe_bot = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️авто-перевод\n(<i>в том числе, текста кнопок</i>)\n▪️авто-ответ\n(<i>chatgpt видит блоки бота</i>)\n▪️приоритетная поддержка\n\n👩🏽‍💻 /balance",
+l_subscribe_ai = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️отсутствие <b>режима ожидания</b>\n▪️аналитика постов канала\n(<i>+финансовый потенциал</i>)\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
     'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 
-l_add_bot_button = {
-    'ru': "➕ Добавить бота",
-    'en': "➕ Add a bot",
-    'es': "➕ Agregar un bot",
-    'fr': "➕ Ajouter un robot",
-    'zh': "➕ 添加机器人",
-    'ar': "➕ أضف بوت",
+l_gen_txt = {
+    'ru': "📘 Текст{0}",
+    'en': "📘 Text{0}",
+    'es': "📘 Texto{0}",
+    'fr': "📘 Texte{0}",
+    'zh': "📘 文字{0}",
+    'ar': "📘 نص {0}",
 }
-l_add_bot_call = {
-    'ru': "➕ Оформи подписку для >1 бота или открепи активного бота, чтобы добавить нового",
-    'en': "➕ Subscribe for >1 bot or unsubscribe active bot to add a new one",
-    'es': "➕ Suscríbete a >1 bot o cancela la suscripción de un bot activo para agregar uno nuevo",
-    'fr': "➕ Abonnez-vous pour > 1 bot ou désabonnez-vous du bot actif pour en ajouter un nouveau",
-    'zh': "➕ 订阅 >1 个机器人或取消订阅活动机器人以添加新机器人",
-    'ar': "➕ اشترك في> 1 bot أو إلغاء الاشتراك في bot النشط لإضافة واحد جديد",
+l_gen_img = {
+    'ru': "🌌 Образ",
+    'en': "🌌 Image",
+    'es': "🌌 Imagen",
+    'fr': "🌌 Image",
+    'zh': "🌌 图片",
+    'ar': "🌌 صورة",
 }
-l_test_bot_desc = {
-    'ru': "🫥 Описание @{0}-бота:\n\n▪️телеграф блог\n▪️авто-перевод\n▪️оповещения и utm-рефералы\n▪️интеграции",
-    'en': "🫥 @{0}-bot description:\n\n▪️telegraph blog\n▪️auto-translation\n▪️alerts and utm referrals\n▪️integrations",
-    'es': "🫥 @{0}-bot description:\n\n▪️telegraph blog\n▪️traducción automática\n▪️alertas y referencias utm\n▪️integraciones",
-    'fr': "🫥 @{0}-bot description :\n\n▪️blog télégraphique\n▪️traduction automatique\n▪️alertes et références utm\n▪️intégrations",
-    'zh': "🫥 @{0}-bot 描述：\n\n▪️电报博客\n▪️自动翻译\n▪️提醒和 utm 推荐\n▪️集成",
-    'ar': "🫥 @ {0} وصف البرنامج الآلي:\n\n▪️ مدونة telegraph\n▪️ ترجمة تلقائية\n▪️ تنبيهات وإحالات UTM\n▪️ تكامل",
+l_gen_tlg = {
+    'ru': "👩🏽‍💻 Анализ @telegram-канала",
+    'en': "👩🏽‍💻 Telegram channel analysis",
+    'es': "👩🏽‍💻 Análisis de canales de Telegram",
+    'fr': "👩🏽‍💻 Analyse des chaînes de télégrammes",
+    'zh': "👩🏽‍💻电报频道分析",
+    'ar': "👩🏽‍💻 تحليل قناة Telegram",
 }
-l_clone_bot_button = {
-    'ru': "©️ Клонировать бота",
-    'en': "©️ Clone the bot",
-    'es': "©️ Clonar el bot",
-    'fr': "©️ Cloner le bot",
-    'zh': "©️ 克隆机器人",
-    'ar': "© ️ استنساخ الروبوت",
+l_generate_main = {
+    'ru': "👩🏽‍💻 <b>Выбери режим</b>",
+    'en': "👩🏽‍💻 <b>Choose a mode</b>",
+    'es': "👩🏽‍💻 <b>Elige un modo</b>",
+    'fr': "👩🏽‍💻 <b>Choisissez un mode</b>",
+    'zh': "👩🏽‍💻<b>选择模式</b>",
+    'ar': "👩🏽‍💻 <b>اختر الوضع</b>",
 }
-l_clone_bot_call = {
-    'ru': "©️ Оформи подписку для >1 бота или открепи активного бота, чтобы склонировать бота конкурента",
-    'en': "©️ Subscribe >1 bot or unpin an active bot to clone a competitor's bot",
-    'es': "©️ Suscríbete >1 bot o desancla un bot activo para clonar el bot de un competidor",
-    'fr': "©️ Abonnez-vous >1 bot ou désépinglez un bot actif pour cloner le bot d'un concurrent",
-    'zh': "©️ 订阅 >1 个机器人或取消固定一个活跃的机器人以克隆竞争对手的机器人",
-    'ar': "© ️ اشترك> 1 بوت أو قم بإلغاء تثبيت روبوت نشط لاستنساخ روبوت منافس",
+l_generate_prompt = {
+    'ru': "👩🏽‍💻 <b>Введи</b> запрос для <b>{0}</b> 👇🏼..",
+    'en': "👩🏽‍💻 <b>Enter</b> a query for <b>{0}</b> 👇🏼..",
+    'es': "👩🏽‍💻 <b>Ingrese</b> una consulta para <b>{0}</b> 👇🏼..",
+    'fr': "👩🏽‍💻 <b>Entrez</b> une requête pour <b>{0}</b> 👇🏼..",
+    'zh': "👩🏽‍💻<b>输入</b>查询<b>{0}</b> 👇🏼..",
+    'ar': "👩🏽‍💻 <b>أدخل</b> استعلامًا عن <b>{0}</b> 👇🏼 ..",
 }
-l_clone_bot_text = {
-    'ru': "©️ <b>Вставь</b> корректную ссылку на бота, чтобы склонировать его",
-    'en': "©️ <b>Paste</b> the correct link to the bot to clone it",
-    'es': "©️ <b>Pega</b> el enlace correcto al bot para clonarlo",
-    'fr': "©️ <b>Collez</b> le bon lien vers le bot pour le cloner",
-    'zh': "©️ 将正确的链接<b>粘贴</b>到机器人以克隆它",
-    'ar': "© ️ <b>الصق</b> الرابط الصحيح إلى الروبوت لاستنساخه",
+l_generate_chn = {
+    'ru': "👩🏽‍💻 <b>Вставь</b> ссылку на @telegram-канал для анализа финансовых показателей",
+    'en': "👩🏽‍💻 <b>Insert</b> a link to the Telegram channel to analyze financial performance",
+    'es': "👩🏽‍💻 <b>Inserta</b> un enlace al canal de Telegram para analizar el desempeño financiero",
+    'fr': "👩🏽‍💻 <b>Insérez</b> un lien vers la chaîne Telegram pour analyser les performances financières",
+    'zh': "👩🏽‍💻<b>插入</b>到 Telegram 频道的链接以分析财务绩效",
+    'ar': "👩🏽‍💻 <b>أدخل</b> رابطًا إلى قناة Telegram لتحليل الأداء المالي",
 }
-l_clone_bot_wait = {
-    'ru': "©️ <b>Клонирование</b> бота\n\n#длительность 1мин",
-    'en': "©️ Bot <b>cloning</b>\n\n#duration 1 min",
-    'es': "©️ <b>Clonación</b> de bots\n\n#duración 1 min",
-    'fr': "©️ <b>Clonage</b> de bot\n\n#durée 1 min",
-    'zh': "©️ Bot<b>克隆</b>\n\n#duration 1 分钟",
-    'ar': "© ️ <b>استنساخ</b> الروبوت\n\n# المدة 1 دقيقة",
+l_generate_wait = {
+    'ru': "👩🏽‍💻 <b>Выбери режим</b> или <b>дождись</b> окончания генерации..",
+    'en': "👩🏽‍💻 <b>Choose a mode</b> or <b>wait for</b> the generation to finish..",
+    'es': "👩🏽‍💻 <b>Elija un modo</b> o <b>espere a</b> que termine la generación..",
+    'fr': "👩🏽‍💻 <b>Choisissez un mode</b> ou <b>attendez la fin de</b> la génération..",
+    'zh': "👩🏽‍💻<b>选择一种模式</b>或<b>等待</b>生成完成..",
+    'ar': "👩🏽‍💻 <b>اختر وضعًا</b> أو <b>انتظر حتى</b> ينتهي الجيل ..",
 }
-l_addbot_handler = {
-    'ru': "➕ Пришли корректный <b>ТОКЕН</b> Telegram-бота, полученный с помощью @botFather-бота\n\n👩🏽‍💻 Например, 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
-    'en': "➕ We sent the correct Telegram bot <b>TOKEN</b> received using @botFather bot\n\n👩🏽‍💻 For example, 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
-    'es': "➕ Enviamos el <b>TOKEN</b> de bot de Telegram correcto recibido usando @botFather bot\n\n👩🏽‍💻 Por ejemplo, 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
-    'fr': "➕ Nous avons envoyé le bon <b>jeton</b> de bot Telegram reçu à l&#x27;aide du bot @botFather\n\n👩🏽‍💻 Par exemple, 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
-    'zh': "➕ 我们发送了使用@botFather bot\n\n👩🏽‍💻 收到的正确的 Telegram bot <b>TOKEN</b>例如， 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
-    'ar': "➕ أرسلنا <b>برنامج</b> Telegram bot الصحيح الذي تم استلامه باستخدام @botFather bot\n\n👩🏽‍💻 على سبيل المثال ، 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
+l_generate_subcribe = {
+    'ru': "👩🏽‍💻 Подожди {0}сек или оформи подписку",
+    'en': "👩🏽‍💻 Wait {0}sec or subscribe",
+    'es': "👩🏽‍💻 Espera {0}segundos o suscríbete",
+    'fr': "👩🏽‍💻 Attendez {0}sec ou abonnez-vous",
+    'zh': "👩🏽‍💻 等待 {0} 秒或订阅",
+    'ar': "👩🏽‍💻 انتظر {0} ثانية أو اشترك",
 }
-l_wait_for_translate_bot = {
-    'ru': "👩🏽‍💻 <b>Перевод</b> {0}-бота на <i>{1}</i>-язык\n\n#длительность 0мин",
-    'en': "👩🏽‍💻 <b>Translation of</b> {0}-bot into <i>{1}</i> -language\n\n#duration 0min",
-    'es': "👩🏽‍💻 <b>Traducción de</b> {0}-bot a <i>{1}</i> -idioma\n\n#duración 0min",
-    'fr': "👩🏽‍💻 <b>Traduction de</b> {0}-bot en <i>{1}</i> -langue\n\n#durée 0min",
-    'zh': "👩🏽‍💻 将 {0}-bot<b>翻译</b>成<i>{1}</i> -language\n\n#duration 0min",
-    'ar': "👩🏽‍💻 <b>ترجمة</b> {0} - الروبوت إلى <i>{1}</i> -اللغة\n\n# المدة 0 دقيقة",
+l_generate_subcribe_channel = {
+    'ru': "👩🏽‍💻 Оформи подписку, чтобы узнать финансовый потенциал твоего @telegram-канала",
+    'en': "👩🏽‍💻 Wait {0}sec or subscribe",
+    'es': "👩🏽‍💻 Espera {0}segundos o suscríbete",
+    'fr': "👩🏽‍💻 Attendez {0}sec ou abonnez-vous",
+    'zh': "👩🏽‍💻 等待 {0} 秒或订阅",
+    'ar': "👩🏽‍💻 انتظر {0} ثانية أو اشترك",
 }
-l_template_is_ready = {
-    'ru': "👩🏽‍💻 <b>Шаблон</b> для @{0} готов!",
-    'en': "👩🏽‍💻 <b>Template</b> for @{0} is ready!",
-    'es': "👩🏽‍💻 ¡ <b>La plantilla</b> para @{0} está lista!",
-    'fr': "👩🏽‍💻 <b>Le modèle</b> pour @{0} est prêt !",
-    'zh': "👩🏽‍💻 @{0} 的<b>模板</b>已准备就绪！",
-    'ar': "👩🏽‍💻 <b>نموذج</b> @ {0} جاهز!",
+l_generate_error = {
+    'ru': "👩🏽‍💻 <b>Ошибка</b> генерации",
+    'en': "👩🏽‍💻 Generation <b>Error</b>",
+    'es': "👩🏽‍💻 <b>Error</b> de generación",
+    'fr': "👩🏽‍💻 <b>Erreur</b> de génération",
+    'zh': "👩🏽‍💻 生成<b>错误</b>",
+    'ar': "👩🏽‍💻 <b>خطأ</b> في التوليد",
 }
-l_payment_successful = {
-    'ru': "👩🏽‍💻 <b>Пользователь</b> {0} 💰Внес оплату в размере {1} {2}",
-    'en': "👩🏽‍💻 <b>User</b> {0} 💰Paid payment in the amount of {1} {2}",
-    'es': "👩🏽‍💻 <b>Usuario</b> {0} 💰Pago pagado por la cantidad de {1} {2}",
-    'fr': "👩🏽‍💻 <b>Utilisateur</b> {0} 💰Paiement payé d'un montant de {1} {2}",
-    'zh': "👩🏽‍💻<b>用户</b>{0} 💰支付金额为{1} {2}",
-    'ar': "👩🏽‍💻 <b>المستخدم</b> {0} 💰 دفعة مدفوعة بمبلغ {1} {2}",
+l_generate_errchn = {
+    'ru': "👩🏽‍💻 <b>Ошибка</b> доступа к каналу (попробуй позже или сделай канал публичным)",
+    'en': "👩🏽‍💻 Channel access <b>error</b> (try later or make the channel public)",
+    'es': "👩🏽‍💻 <b>Error</b> de acceso al canal (inténtalo más tarde o haz público el canal)",
+    'fr': "👩🏽‍💻 <b>Erreur</b> d'accès à la chaîne (essayez plus tard ou rendez la chaîne publique)",
+    'zh': "👩🏽‍💻频道访问<b>错误</b>（稍后再试或公开频道）",
+    'ar': "👩🏽‍💻 <b>خطأ</b> في الوصول إلى القناة (حاول لاحقًا أو اجعل القناة عامة)",
 }
-l_promocode_activated = {
-    'ru': "👩🏽‍💻 *Промокод*: `{txt}` активирован",
-    'en': "👩🏽‍💻 *Promo code*: `{txt}` activated",
-    'es': "👩🏽‍💻 *Código promocional*: `{txt}` activado",
-    'fr': "👩🏽‍💻 *Code promotionnel* : `{txt}` activé",
-    'zh': "👩🏽‍💻 *促销代码*：`{txt}` 激活",
-    'ar': "👩🏽‍💻 * الرمز الترويجي *: '{txt}` مفعل",
+# endregion
+
+
+# region FereyFindBot
+l_find_btn1 = {
+    'ru': "⛰️ Поиск",
+    'en': "⛰️ Search",
+    'es': "⛰️ Buscar",
+    'fr': "⛰️ Rechercher",
+    'zh': "⛰️ 搜索",
+    'ar': "⛰️ بحث",
+}
+l_find_btn2 = {
+    'ru': "📍 Geo поиск",
+    'en': "📍 Geo search",
+    'es': "📍 Búsqueda geográfica",
+    'fr': "📍 Recherche géographique",
+    'zh': "📍地理搜索",
+    'ar': "📍 البحث الجغرافي",
+}
+l_find_btn3 = {
+    'ru': "🔔 Уведомления",
+    'en': "🔔 Notifications",
+    'es': "🔔 Notificaciones",
+    'fr': "🔔 Notifications",
+    'zh': "🔔 通知",
+    'ar': "🔔 الإخطارات",
+}
+l_find_btn4 = {
+    'ru': "🌬 Подписка",
+    'en': "🌬 Subscription",
+    'es': "🌬 Suscripción",
+    'fr': "🌬 Abonnement",
+    'zh': "🌬订阅",
+    'ar': "🌬 الاشتراك",
+}
+l_find_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> поиска в <b>Telegram</b>:\n\n▪️<b>top</b> каналы/группы\n▪️<b>vip</b> пользователи/боты\n▪️<b>гео</b> парсинг\n▪️<b>пассивный</b> маркетинг\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <b>Telegram</b> поиска <i>landing bot</i> :\n\n▪️ <b>top</b> channels/groups\n▪️ <b>vip</b> users/bots\n▪️ <b>geo</b> parsing\n▪️ <b>passive</b> marketing\n\n❗️ you can also order development Telegram promotions in our Ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> поиска <b>de Telegram</b> :\n\n▪️ canales/grupos <b>principales</b>\n▪️ usuarios <b>vip</b> /bots\n▪️ análisis <b>geográfico</b>\n▪️ marketing <b>pasivo</b>\n\n❗️ también puedes solicitar promociones de desarrollo de Telegram en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue sur <b>Telegram</b> поиска <i>landing bot</i> :\n\n▪️ <b>meilleurs</b> canaux/groupes\n▪️ utilisateurs/bots <b>vip</b>\n▪️ analyse <b>géographique</b>\n▪️ marketing <b>passif</b>\n\n❗️ vous pouvez également commander des promotions de développement Telegram dans notre atelier de Ferey",
+    'zh': "🌱 {0}，欢迎使用<b>Telegram</b> поиска<i>登陆机器人</i>：\n\n▪️<b>热门</b>频道/群组\n▪️ <b>vip</b>用户/机器人\n▪️<b>地理</b>解析\n▪️<b>被动</b>营销\n\n❗️ 您也可以订购开发 Telegram 促销在我们的Ferey工作室",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوطي</i> поиска <b>Telegram</b> :\n\n▪️ <b>أفضل</b> القنوات / المجموعات\n▪️ مستخدمين / برامج تتبع <b>لكبار</b> الشخصيات\n▪️ تحليل <b>جغرافي</b>\n▪️ تسويق <b>سلبي</b>\n\n❗️ يمكنك أيضًا طلب ترويجات Telegram للتطوير في استوديو Ferey الخاص بنا",
+}
+l_subscribe_find = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>уведомления</b> о ключевых словах\n(<i>ссылка на сообщение</i>)\n▪️<b>увеличение</b> лимитов уведомлений\n(<i>до 10 ключевых слов/групп/каналов</i>)\n▪️<b>приоритетная</b> выдача при поиске\n(<i>выше чем premium/verified</i>)\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
+l_find_bot_text_find = {
+    'ru': "👩🏽‍💻 <b>Источник</b>: {0}, ссылка на публикацию: [{1}] (ключевое слово: <u>{2}</u>)",
+    'en': "👩🏽‍💻 <b>Источник</b>: {name} нажал на: [{button}] (пост #<u>{post_id}</u>)",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 
-# region commands
-l_bot_commands_handler = {
-    'ru': "⚙️ <b>Команды</b> /cmd для <b>@{0}</b>\n\n/info   <i>информация</i>\n/stat   <i>аналитика</i>\n/status <i>статус</i>\n/on     <i>включение</i>\n/off    <i>выключение</i>\n/restart  <i>перезагрузка</i>\n\n/parse [premium|admin|utm|ban]\n/admin [id]    <i>администраторы</i>\n/promo      <i>промокод</i>\n/ban [id/@username]   <i>список</i>\n/unban     <i>разбан</i>",
-    'en': "⚙️ <b>Commands</b> /cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>promo code</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'es': "⚙️ <b>Comandos</b> /cmd para <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disabled</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>administradores</i>\n/promo <i>código de promoción</i>\n/ban [id/ @username ] <i>lista</i>\n/unban <i>no baneado</i>",
-    'fr': "⚙️ <b>Commandes</b> /cmd pour <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>recharger</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>code promo</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'zh': "⚙️<b>命令</b>/cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo<i>促销代码</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'ar': "⚙️ <b>أوامر</b> / cmd لـ <b>@ {0}</b>\n\n/ info <i>info</i>\n/ stat <i>analytics</i>\n/ status <i>status</i>\n/ on <i>تمكين</i>\n/off <i>تعطيل</i>\n/restart <i>تحميل</i>\n\n/ parse [premium | admin | utm | ban]\n/ admin [id] <i>admins</i>\n/ <i>promo code</i>\n/ ban [id / @username ] <i>list</i>\n/ <i>unsanned</i>",
+l_geo_minus = {
+    'ru': "-",
+    'en': "-",
+    'es': "-",
+    'fr': "-",
+    'zh': "-",
+    'ar': "-",
 }
-l_bot_status_handler = {
-    'ru': "👩🏽‍💻 <b>Статус</b> @{0}-бота: {1}",
-    'en': "👩🏽‍💻 <b>Status</b> @{0}-bot: {1}",
-    'es': "👩🏽‍💻 <b>Estado</b> @{0}-bot: {1}",
-    'fr': "👩🏽‍💻 <b>Statut</b> @{0}-bot : {1}",
-    'zh': "👩🏽‍💻<b>状态</b>@{0}-bot：{1}",
-    'ar': "👩🏽‍💻 <b>الحالة</b> @ {0} -روبوت: {1}",
+l_geo_current = {
+    'ru': "📍R: {0}m",
+    'en': "📍R: {0}m",
+    'es': "📍R: {0}m",
+    'fr': "📍R : {0}mois",
+    'zh': "📍R：{0}米",
+    'ar': "📍R: {0} م",
 }
-l_bot_on_handler = {
-    'ru': "👩🏽‍💻 <b>Запуск</b> @{0}-бота..\n\n#длительность 1мин",
-    'en': "👩🏽‍💻 <b>Launch</b> @{0}-bot..\n\n#duration 1 min",
-    'es': "👩🏽‍💻 <b>Lanzar</b> @{0}-bot..\n\n#duración 1 min",
-    'fr': "👩🏽‍💻 <b>Lancer</b> @{0}-bot..\n\n#durée 1 min",
-    'zh': "👩🏽‍💻<b>启动</b>@{0}-bot..\n\n#duration 1 分钟",
-    'ar': "👩🏽‍💻 <b>Launch</b> @ {0} -bot ..\n\n# المدة 1 دقيقة",
+l_geo_plus = {
+    'ru': "+",
+    'en': "+",
+    'es': "+",
+    'fr': "+",
+    'zh': "+",
+    'ar': "+",
 }
-l_bot_on_handler_already = {
-    'ru': "👩🏽‍💻 <b>@{0}</b>-бот уже запущен",
-    'en': "👩🏽‍💻 <b>@{0}</b> - the bot is already running",
-    'es': "👩🏽‍💻 <b>@{0}</b> : el bot ya se está ejecutando",
-    'fr': "👩🏽‍💻 <b>@{0}</b> - le bot est déjà en cours d'exécution",
-    'zh': "👩🏽‍💻 <b>@{0}</b> - 机器人已经在运行",
-    'ar': "👩🏽‍💻 <b>@ {0}</b> - الروبوت قيد التشغيل بالفعل",
+l_geo_text1 = {
+    'ru': "📍 <b>GEO-поиск</b> пользователей\n\n👩🏽‍💻 <b>Жми</b> на -/+, чтобы настроить 📍Radius",
+    'en': "📍 <b>Geo-search</b> users by coordinates\n\n👩🏽‍💻 <b>Click</b> on -/+ to adjust 📍Radius",
+    'es': "📍 Usuarios <b>de búsqueda geográfica</b> por coordenadas\n\n👩🏽‍💻 <b>Haz clic</b> en -/+ para ajustar el 📍Radio",
+    'fr': "📍 <b>Géo-recherche</b> des utilisateurs par coordonnées\n\n👩🏽‍💻 <b>Cliquez</b> sur -/+ pour ajuster 📍Rayon",
+    'zh': "📍 按坐标<b>地理搜索</b>用户\n\n👩🏽‍💻<b>点击</b>-/+ 调整📍半径",
+    'ar': "📍 <b>البحث الجغرافي</b> للمستخدمين عن طريق الإحداثيات\n\n👩🏽‍💻 <b>انقر</b> فوق - / + لضبط 📍Radius",
 }
-l_bot_off_handler = {
-    'ru': "👩🏽‍💻 <b>Остановка</b> @{0}-бота..\n\n#длительность 1мин",
-    'en': "👩🏽‍💻 @{0}-bot <b>stop</b> ..\n\n#duration 1 min",
-    'es': "👩🏽‍💻 @{0}-bot <b>parada</b> ..\n\n#duración 1 min",
-    'fr': "👩🏽‍💻 @{0}-bot <b>stop</b> ..\n\n#durée 1 min",
-    'zh': "👩🏽‍💻 @{0}-bot<b>停止</b>..\n\n#duration 1 分钟",
-    'ar': "👩🏽‍💻 @ {0} -bot <b>stop</b> ..\n\n# المدة 1 دقيقة",
+l_geo_text2 = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> геопозицию через 📎-меню вложений или <b>Жми</b> на кнопку ниже\n[📍Отправить Geo] 👇🏽",
+    'en': "👩🏽‍💻 <b>Attach</b> a location via the 📎 attachment menu or <b>click</b> on the button below\n[📍Send Geo] 👇🏽",
+    'es': "👩🏽‍💻 <b>Adjunte</b> una ubicación a través del 📎 menú de archivos adjuntos o <b>haga clic</b> en el botón a continuación\n[📍Send Geo] 👇🏽",
+    'fr': "👩🏽‍💻 <b>Joignez</b> un lieu via le 📎 menu de pièces jointes ou <b>cliquez</b> sur le bouton ci-dessous\n[📍Envoyer Géo] 👇🏽",
+    'zh': "👩🏽‍💻通过📎附件菜单<b>附加</b>位置或<b>单击</b>下面的按钮\n[📍发送地理信息]👇🏽",
+    'ar': "👩🏽‍💻 <b>قم بإرفاق</b> موقع عبر قائمة 📎 المرفقات أو <b>انقر</b> فوق الزر أدناه\n[Send Geo] 👇🏽",
 }
-l_bot_off_handler_already = {
-    'ru': "👩🏽‍💻 <b>@{0}</b>-бот уже выключен",
-    'en': "👩🏽‍💻 <b>@{0}</b> -bot is already off",
-    'es': "👩🏽‍💻 <b>@{0}</b> -bot ya está apagado",
-    'fr': "👩🏽‍💻 <b>@{0}</b> -bot est déjà désactivé",
-    'zh': "👩🏽‍💻 <b>@{0}</b> -bot 已经关闭",
-    'ar': "الروبوت 👩🏽‍💻 <b>@ {0}</b> متوقف بالفعل",
+l_geo_send = {
+    'ru': "📍Отправить Geo",
+    'en': "📍Send Geo",
+    'es': "📍Enviar Geo",
+    'fr': "📍Envoyer Géo",
+    'zh': "📍发送地理位置",
+    'ar': "📍إرسال جيو",
 }
-l_bot_off_handler_done = {
-    'ru': "👩🏽‍💻 <b>@{0}</b>-бот выключен",
-    'en': "👩🏽‍💻 <b>@{0}</b> -bot is off",
-    'es': "👩🏽‍💻 <b>@{0}</b> -bot está apagado",
-    'fr': "👩🏽‍💻 <b>@{0}</b> -bot est désactivé",
-    'zh': "👩🏽‍💻 <b>@{0}</b> -bot 已关闭",
-    'ar': "👩🏽‍💻 <b>@ {0}</b> -الروبوت غير مفعّل",
+l_geo_start = {
+    'ru': "🔎 <b>Начинаем</b> поиск..",
+    'en': "🔎 Let's start the search..",
+    'es': "🔎 Comencemos la búsqueda..",
+    'fr': "🔎 Commençons la recherche..",
+    'zh': "🔎 让我们开始搜索..",
+    'ar': "🔎 لنبدأ البحث ..",
 }
-l_bot_restart_handler = {
-    'ru': "👩🏽‍💻 <b>Перезапуск</b> @{0}-бота..\n\n#длительность 1мин",
-    'en': "👩🏽‍💻 @{0}-bot <b>restart</b> ..\n\n#duration 1 min",
-    'es': "👩🏽‍💻 @{0}-bot <b>reinicio</b> ..\n\n#duración 1 min",
-    'fr': "👩🏽‍💻 @{0}-bot <b>restart</b> ..\n\n#durée 1 min",
-    'zh': "👩🏽‍💻@{0}-bot<b>重启</b>..\n\n#duration 1 分钟",
-    'ar': "👩🏽‍💻 @ {0} -bot <b>إعادة التشغيل</b> ..\n\n# المدة 1 دقيقة",
+l_geo_no = {
+    'ru': "📍 Пользователей (@username) в данной геопозиции не найдено",
+    'en': "📍 No users ( @username ) found in this location",
+    'es': "📍 No se encontraron usuarios ( @username ) en esta ubicación",
+    'fr': "📍 Aucun utilisateur ( @username ) trouvé à cet emplacement",
+    'zh': "📍 在此位置找不到用户 ( @username )",
+    'ar': "📍 لم يتم العثور على مستخدمين ( @username ) في هذا الموقع",
+}
+l_geo_finish = {
+    'ru': "🔥 <b>Готово!</b> Найдено пользователей: <u>{0}</u>",
+    'en': "🔥 <b>Done!</b> Found users: <u>{0}</u>",
+    'es': "🔥 <b>Listo!</b> Usuarios encontrados: <u>{0}</u>",
+    'fr': "🔥 <b>C&#x27;est fait !</b> Utilisateurs trouvés : <u>{0}</u>",
+    'zh': "🔥<b>完成！</b>找到的用户： <u>{0}</u>",
+    'ar': "🔥 <b>انتهى!</b> المستخدمون الموجودون: <u>{0}</u>",
 }
-# endregion
-
-
-# region bot
-l_bot_config = {
-    ("cctor", "👩🏽‍💻", "☑"): {
-        'ru': "Конструктор ᴺᴱᵂ",
-        'en': "Builder ᴺᴱᵂ",
-        'es': "Builder ᴺᴱᵂ",
-        'fr': "Builder ᴺᴱᵂ",
-        'zh': "Builder ᴺᴱᵂ",
-        'ar': "Builder ᴺᴱᵂ",
-    },
-    ("cban", "🕵🏽", "☑"): {
-        'ru': "Авто-бан",
-        'en': "Auto-ban",
-        'es': "Prohibición automática",
-        'fr': "Interdiction automatique",
-        'zh': "自動禁止",
-        'ar': "حظر تلقائي",
-    },
-    ("ctranslate", "文", "☐"): {
-        'ru': "Авто-перевод",
-        'en': "Auto-translate",
-        'es': "Saludo automático",
-        'fr': "Message d'accueil automatique",
-        'zh': "自動問候",
-        'ar': "الترحيب التلقائي",
-    },
-    ("canswer", "👋🏽", "☐"): {
-        'ru': "Авто-ответ",
-        'en': "Auto-answer",
-        'es': "Saludo automático",
-        'fr': "Message d'accueil automatique",
-        'zh': "自動問候",
-        'ar': "الترحيب التلقائي",
-    },
-    ("cpost", "🔔", "☐"): {
-        'ru': "Авто-постинг",
-        'en': "Auto-posting",
-        'es': "Publicación automática",
-        'fr': "Publication automatique",
-        'zh': "自動發布",
-        'ar': "النشر التلقائي",
-    },
 
-    ("cpayment", "💳", "☐"): {
-        'ru': "Платежи",
-        'en': "Payments",
-        'es': "Prohibición automática",
-        'fr': "Interdiction automatique",
-        'zh': "自動禁止",
-        'ar': "حظر تلقائي",
-    },
-    ("cintegration", "🗝️", "☐"): {
-        'ru': "Интеграции",
-        'en': "Integrations",
-        'es': "Publicación automática",
-        'fr': "Publication automatique",
-        'zh': "自動發布",
-        'ar': "النشر التلقائي",
-    },
-    ("cnotification", "💬", "☑"): {
-        'ru': "Оповещения",
-        'en': "Notifications",
-        'es': "Mensajes con 文/ب/y",
-        'fr': "Messagerie avec 文/ب/y",
-        'zh': "與消息 文/ب/y",
-        'ar': "文/ب/y الرسائل ذات",
-    },
-    ("cuser", "👥", "☑"): {
-        'ru': "Пользователи",
-        'en': "Users",
-        'es': "Mensajes con 文/ب/y",
-        'fr': "Messagerie avec 文/ب/y",
-        'zh': "與消息 文/ب/y",
-        'ar': "文/ب/y الرسائل ذات",
-    },
-    ("cadmin", "👮🏽", "☑"): {
-        'ru': "Администраторы",
-        'en': "Administrators",
-        'es': "Mensajes con 文/ب/y",
-        'fr': "Messagerie avec 文/ب/y",
-        'zh': "與消息 文/ب/y",
-        'ar': "文/ب/y الرسائل ذات",
-    },
+l_find_add_cmd = {
+    'ru': "👩🏽‍💻 <b>Пришли</b> ссылку на канал/группу/пользователя/бота",
+    'en': "👩🏽‍💻 <b>Send</b> a link to a channel/group/user/bot",
+    'es': "👩🏽‍💻 <b>Enviar</b> un enlace a un canal/grupo/usuario/bot",
+    'fr': "👩🏽‍💻 <b>Envoyer</b> un lien vers un canal/groupe/utilisateur/bot",
+    'zh': "👩🏽‍💻<b>发送</b>指向频道/组/用户/机器人的链接",
+    'ar': "👩🏽‍💻 <b>أرسل</b> رابطًا إلى قناة / مجموعة / مستخدم / روبوت",
 }
-l_remove_bot = {
-    'ru': "🚫Убрать бота",
-    'en': "🚫Remove bot",
-    'es': "🚫Eliminar bot",
-    'fr': "🚫Supprimer le robot",
-    'zh': "🚫删除机器人",
-    'ar': "🚫 إزالة البوت",
+l_find_err_cmd = {
+    'ru': "👩🏽‍💻 <b>Ошибка</b> (вставь корректную ссылку или повтори позже)",
+    'en': "👩🏽‍💻 <b>Error</b> (insert correct link or try again later)",
+    'es': "👩🏽‍💻 <b>Error</b> (inserta el enlace correcto o vuelve a intentarlo más tarde)",
+    'fr': "👩🏽‍💻 <b>Erreur</b> (insérez le lien correct ou réessayez plus tard)",
+    'zh': "👩🏽‍💻<b>错误</b>（插入正确的链接或稍后重试）",
+    'ar': "👩🏽‍💻 <b>خطأ</b> (أدخل الرابط الصحيح أو حاول مرة أخرى لاحقًا)",
 }
-
-l_show_bots = {
-    'ru': "👩🏽‍💻 <b>Добавленные боты</b>\n\n[команды /cmd]",
-    'en': "👩🏽‍💻 <b>Added bots</b>\n\n[commands /cmd]",
-    'es': "👩🏽‍💻 <b>Se agregaron bots</b>\n\n[comandos /cmd]",
-    'fr': "👩🏽‍💻 <b>Ajout de bots</b>\n\n[commandes /cmd]",
-    'zh': "👩🏽‍💻<b>添加了机器人</b>\n\n[命令/cmd]",
-    'ar': "👩🏽‍💻 <b>الروبوتات المضافة</b>\n\n[أوامر / cmd]",
+l_find_ok_cmd = {
+    'ru': "👩🏽‍💻 <b>Ссылка</b> успешно добавлена!",
+    'en': "👩🏽‍💻 <b>Link</b> added successfully!",
+    'es': "👩🏽‍💻 ¡ <b>Enlace</b> agregado exitosamente!",
+    'fr': "👩🏽‍💻 <b>Lien</b> ajouté avec succès !",
+    'zh': "👩🏽‍💻<b>链接</b>添加成功！",
+    'ar': "👩🏽‍💻 تمت إضافة <b>الرابط</b> بنجاح!",
+}
+l_find_check = {
+    'ru': "🔗 Проверка",
+    'en': "🔗 Check",
+    'es': "🔗 Comprobar",
+    'fr': "🔗 Vérifier",
+    'zh': "🔗 检查",
+    'ar': "🔗 تحقق",
 }
 
-l_creturntext = {
-    'ru': "✖️ <b>Сбросить</b> настройки по умолчанию (до рекомендуемых) для бота [<b>{0}</b>]?",
-    'en': "✖️ <b>Reset</b> default settings (recommended) for bot [<b>{0}</b>]?",
-    'es': "✖️ <b>¿Restablecer</b> la configuración predeterminada (recomendado) para el bot [<b>{0}</b>]?",
-    'fr': "✖️ <b>Réinitialiser</b> les paramètres par défaut (recommandé) pour le bot [<b>{0}</b>] ?",
-    'zh': "✖️<b>重置</b>机器人 [<b>{0}</b>] 的默认设置（推荐）？",
-    'ar': "✖️ <b>إعادة تعيين</b> الإعدادات الافتراضية (موصى به) للروبوت [<b>{0}</b>]؟",
+l_find_menu = {
+    'ru': "↩ Menu",
+    'en': "↩ Menu",
+    'es': "↩ Menú",
+    'fr': "↩Menu",
+    'zh': "↩ 菜单",
+    'ar': "↩ القائمة",
 }
-l_creturnanswer = {
-    'ru': "✖️ Настройки бота [<b>{0}</b>] успешно сброшены!",
-    'en': "✖️ Bot settings [<b>{0}</b>] successfully reset!",
-    'es': "✖️ ¡La configuración del bot [<b>{0}</b>] se restableció correctamente!",
-    'fr': "✖️ Les paramètres du bot [<b>{0}</b>] ont été réinitialisés avec succès !",
-    'zh': "✖️ 机器人设置 [<b>{0}</b>] 成功重置！",
-    'ar': "✖️ تم إعادة تعيين إعدادات البوت [<b>{0}</b>] بنجاح!",
+l_find_text = {
+    'ru': "<b>🔎 Сбор целевой аудитории (ЦА)</b>\n\n▪️выгрузка тематических каналов\n▪️выгрузка групп с ЦА\n▪️выгрузка конкурентов по нише\n▪️каталог ботов\n\n<b>Итог:</b> <i>получение <u>горячей</u> ЦА, анализ ЦА конкурентов</i>",
+    'en': "<b>🔎 Gathering the target audience (CA)</b>\n\n▪️uploading thematic channels\n▪️uploading leads/chats from the target audience\n▪️uploading competitors by niche\n▪️bot directory\n\n<b>Result:</b> <i>getting <u>a hot target</u> audience, analyzing the target audience of competitors</i>",
+    'es': "<b>🔎 Reunir el público objetivo (CA)</b>\n\n▪️cargar canales temáticos\n▪️cargar clientes potenciales/chats del público objetivo\n▪️cargar competidores por nicho\n▪️directorio de bots\n\n<b>Resultado:</b> <i>obtener <u>un público objetivo atractivo</u> , analizando el público objetivo de los competidores</i>",
+    'fr': "<b>🔎 Rassembler le public cible (CA)</b>\n\n▪️télécharger des chaînes thématiques\n▪️télécharger des prospects/chats du public cible\n▪️télécharger des concurrents par niche\n▪️répertoire de robots\n\n<b>Résultat :</b> <i>obtenir <u>un public cible chaud</u> , analysant le public cible des concurrents</i>",
+    'zh': "<b>🔎 收集目标受众 (CA)</b>\n\n▪️上传主题频道\n▪️从目标受众上传线索/聊天\n▪️按利基上传竞争对手\n▪️bot 目录\n\n<b>结果：</b><i>获得<u>热门目标</u>受众, 分析竞争对手的目标受众</i>",
+    'ar': "<b>🔎 تجميع الجمهور المستهدف (CA)</b>\n\n▪️ تحميل القنوات الموضوعية\n▪️ تحميل العملاء المتوقعين / الدردشات من الجمهور المستهدف\n▪️ تحميل المنافسين حسب المجال المناسب\n▪️ الدليل الآلي\n\n<b>النتيجة:</b> <i>الحصول على جمهور <u>مستهدف نشط</u> ، وتحليل الجمهور المستهدف من المنافسين</i>",
 }
-l_cdeletetext = {
-    'ru': "🚫 Убрать привязку бота [<b>{0}</b>]?",
-    'en': "🚫 Remove bot binding [<b>{0}</b>]?",
-    'es': "🚫 ¿Eliminar el enlace del bot [<b>{0}</b>]?",
-    'fr': "🚫 Supprimer la liaison du bot [<b>{0}</b>] ?",
-    'zh': "🚫 删除机器人绑定 [<b>{0}</b>]？",
-    'ar': "🚫 إزالة ربط البوت [<b>{0}</b>]؟",
+l_find_category_typing = {
+    'ru': "✅ #ввести свои параметры",
+    'en': "✅ #ввести your parameters",
+    'es': "✅ #ввести sus parámetros",
+    'fr': "✅ #ввести vos paramètres",
+    'zh': "✅ # #ввести你的参数",
+    'ar': "✅ # #ввести المعلمات الخاصة بك",
 }
-l_cdeleteanswer = {
-    'ru': "🚫 Бот успешно откреплен [<b>{0}</b>]",
-    'en': "🚫 Bot successfully unlocked [<b>{0}</b>]",
-    'es': "🚫 Bot desbloqueado con éxito [<b>{0}</b>]",
-    'fr': "🚫 Bot déverrouillé avec succès [<b>{0}</b>]",
-    'zh': "🚫 机器人成功解锁 [<b>{0}</b>]",
-    'ar': "🚫 تم فتح بوت بنجاح [<b>{0}</b>]",
+l_find_desc = {
+    'ru': "<b>Описание:</b> {0}",
+    'en': "<b>Description:</b> {0}",
+    'es': "<b>Descripción:</b> {0}",
+    'fr': "<b>Descriptif :</b> {0}",
+    'zh': "<b>说明：</b> {0}",
+    'ar': "<b>الوصف:</b> {0}",
 }
-l_transfer_success = {
-    'ru': "👩🏽‍💻 <b>Права</b> владения на @{0}-бота успешно переданы @{1}-аккаунту!\n\n👩🏽‍💻 Теперь для передачи прав/настройки можно использовать @botfather-бота",
-    'en': "👩🏽‍💻 <b>Ownership</b> of @{0}-bot successfully transferred to @{1}-account!\n\n👩🏽‍💻 You can now use @botfather -bot to transfer ownership/configuration",
-    'es': "👩🏽‍💻 ¡ <b>La propiedad</b> de @{0}-bot se transfirió con éxito a @{1}-cuenta!\n\n👩🏽‍💻 Ahora puedes usar @botfather -bot para transferir la propiedad/configuración",
-    'fr': "👩🏽‍💻 <b>La propriété</b> de @{0}-bot a été transférée avec succès vers @{1}-compte !\n\n👩🏽‍💻 Vous pouvez maintenant utiliser @botfather -bot pour transférer la propriété/configuration",
-    'zh': "👩🏽‍💻 @{0}-bot 的<b>所有权</b>已成功转移到@{1}-帐户！\n\n👩🏽‍💻 您现在可以使用@botfather -bot 转移所有权/配置",
-    'ar': "👩🏽‍💻 تم نقل <b>ملكية</b> @ {0} -bot بنجاح إلى @ {1} -account!\n\n👩🏽‍💻 يمكنك الآن استخدام @botfather -bot لنقل الملكية / التهيئة",
+l_find_reacts = {
+    'ru': "<b>Реакции:</b> {0}",
+    'en': "<b>Reactions:</b> {0}",
+    'es': "<b>Reacciones:</b> {0}",
+    'fr': "<b>Réactions :</b> {0}",
+    'zh': "<b>反应：</b> {0}",
+    'ar': "<b>التفاعلات:</b> {0}",
 }
-# endregion
-
-
-# region config
-# region ctranslate_
-l_ctranslate_text = {
-    'ru': "文 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> авто-перевод для <i>исходящих</i> сообщений бота на язык пользователя при /start-запуске бота",
-    'en': "文<b>Click</b> on ✅/☑️ to <b>enable/disable</b> auto-translate for <i>outgoing</i> bot messages into the user's language when /start-starting the bot",
-    'es': "文<b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> la traducción automática de los mensajes <i>salientes</i> del bot al idioma del usuario cuando/inicie el bot",
-    'fr': "文<b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> la traduction automatique des messages <i>sortants</i> du bot dans la langue de l'utilisateur lors du/démarrage du bot",
-    'zh': "文<b>单击</b>✅/☑️<b>启用/禁用</b>在/启动机器人时将<i>传出的</i>机器人消息自动翻译成用户的语言",
-    'ar': "文<b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> الترجمة التلقائية لرسائل الروبوت <i>الصادرة</i> إلى لغة المستخدم عند / بدء تشغيل الروبوت",
+l_find_send = {
+    'ru': "<b>Сообщ/медиа/инлайн/инвайт:</b> {0}/{1}/{2}/{3}",
+    'en': "<b>Message/Media/Inline/Invite:</b> {0}/{1}/{2}/{3}",
+    'es': "<b>Mensaje/Medios/En línea/Invitación:</b> {0}/{1}/{2}/{3}",
+    'fr': "<b>Message/Média/Inline/Invitation :</b> {0}/{1}/{2}/{3}",
+    'zh': "<b>消息/媒体/内联/邀请：</b> {0}/{1}/{2}/{3}",
+    'ar': "<b>رسالة / وسائط / مضمنة / دعوة:</b> {0} / {1} / {2} / {3}",
 }
-l_ctranslate_in_on = {
-    'ru': "✅☑Вкл перевод входящих",
-    'en': "✅☑On translation of incoming",
-    'es': "✅☑Sobre la traducción de entrantes",
-    'fr': "✅☑Sur la traduction des entrants",
-    'zh': "✅☑关于来电翻译",
-    'ar': "✅☑على ترجمة واردة",
+l_find_bio = {
+    'ru': "<b>Био:</b> {0}",
+    'en': "<b>Bio:</b> {0}",
+    'es': "<b>Biografía:</b> {0}",
+    'fr': "<b>Biographie :</b> {0}",
+    'zh': "<b>简历：</b> {0}",
+    'ar': "<b>السيرة الذاتية:</b> {0}",
 }
-l_ctranslate_in_off = {
-    'ru': "☑️☐Выкл перевод входящих",
-    'en': "☑️☐Off incoming translation",
-    'es': "☑️☐Traducción entrante desactivada",
-    'fr': "☑️☐Désactiver la traduction entrante",
-    'zh': "☑️☐关闭传入翻译",
-    'ar': "☑️☐ إيقاف الترجمة الواردة",
+l_find_about = {
+    'ru': "<b>Описание:</b> {0}",
+    'en': "<b>Description:</b> {0}",
+    'es': "<b>Descripción:</b> {0}",
+    'fr': "<b>Descriptif :</b> {0}",
+    'zh': "<b>说明：</b> {0}",
+    'ar': "<b>الوصف:</b> {0}",
 }
-l_ctranslate_out_on = {
-    'ru': "✅☑Вкл перевод исходящих",
-    'en': "✅☑On outgoing translation",
-    'es': "✅☑Sobre la traducción saliente",
-    'fr': "✅☑Sur la traduction sortante",
-    'zh': "✅☑关于传出翻译",
-    'ar': "✅☑ على الترجمة الصادرة",
+l_find_description = {
+    'ru': "<b>Подробнее:</b> {0}",
+    'en': "<b>Read more:</b> {0}",
+    'es': "<b>Leer más:</b> {0}",
+    'fr': "<b>En savoir plus :</b> {0}",
+    'zh': "<b>阅读更多：</b> {0}",
+    'ar': "<b>اقرأ المزيد:</b> {0}",
 }
-l_ctranslate_out_off = {
-    'ru': "☑️☐Выкл перевод исходящих",
-    'en': "☑️☐Off transfer outgoing",
-    'es': "☑️☐Fuera de transferencia saliente",
-    'fr': "☑️☐Off transfert sortant",
-    'zh': "☑️☐关闭转出",
-    'ar': "☑️☐Off تحويل الصادرة",
+l_find_commands = {
+    'ru': "<b>Команды:</b> {0}",
+    'en': "<b>Commands:</b> {0}",
+    'es': "<b>Comandos:</b> {0}",
+    'fr': "<b>Commandes :</b> {0}",
+    'zh': "<b>命令：</b> {0}",
+    'ar': "<b>الأوامر:</b> {0}",
 }
-# endregion
 
-
-# region canswer_
-l_canswer_text = {
-    'ru': "👋🏽 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> режим авто-ответа на текстовые сообщения с помощью нейросети",
-    'en': "👋🏽 <b>Press</b> ✅/☑️ to <b>turn on/off</b> auto-reply to text messages using neural network",
-    'es': "👋🏽 <b>Presione</b> ✅/☑️ para <b>activar/desactivar</b> la respuesta automática a los mensajes de texto usando la red neuronal",
-    'fr': "👋🏽 <b>Appuyez sur</b> ✅/☑️ pour <b>activer/désactiver</b> la réponse automatique aux messages texte à l'aide du réseau neuronal",
-    'zh': "👋🏽<b>按</b>✅/☑️ 使用神经网络<b>打开/关闭</b>自动回复短信",
-    'ar': "👋🏽 <b>اضغط</b> <b>على ✅ / ☑️ لتشغيل / إيقاف</b> الرد التلقائي على الرسائل النصية باستخدام الشبكة العصبية",
+l_find_chn = {
+    'ru': "📰 Каналы",
+    'en': "📰 Channels",
+    'es': "📰 Canales",
+    'fr': "📰 Chaînes",
+    'zh': "📰频道",
+    'ar': "📰 القنوات",
+}
+l_find_grp = {
+    'ru': "📁 Группы",
+    'en': "📁 Groups",
+    'es': "📁 Grupos",
+    'fr': "📁 Groupes",
+    'zh': "📁 团体",
+    'ar': "📁 المجموعات",
+}
+l_find_usr = {
+    'ru': "🕵️ Конкуренты",
+    'en': "🕵️ Competitors",
+    'es': "🕵️ Competidores",
+    'fr': "🕵️ Concurrents",
+    'zh': "🕵️ 参赛者",
+    'ar': "🕵️ المنافسون",
+}
+l_find_bot = {
+    'ru': "🫥 Боты",
+    'en': "🫥 Tg bots",
+    'es': "🫥Tg bots",
+    'fr': "🫥 Robots Tg",
+    'zh': "🫥 Tg 机器人",
+    'ar': "🫥 Tg bots",
 }
-# endregion
 
+l_find_chn_choose = {
+    'ru': "📰 <b>Выбери категорию</b> для выгрузки каналов",
+    'en': "📰 <b>Choose a category</b> for uploading channels",
+    'es': "📰 <b>Elige una categoría</b> para subir canales",
+    'fr': "📰 <b>Choisissez une catégorie</b> pour télécharger des chaînes",
+    'zh': "📰<b>选择上传频道的类别</b>",
+    'ar': "📰 <b>اختر فئة</b> لتحميل القنوات",
+}
+l_find_grp_choose = {
+    'ru': "📁 <b>Выбери категорию</b> для выгрузки групп",
+    'en': "📁 <b>Choose a category</b> for uploading groups",
+    'es': "📁 <b>Elige una categoría</b> para subir grupos",
+    'fr': "📁 <b>Choisissez une catégorie</b> pour télécharger des groupes",
+    'zh': "📁<b>选择上传群组的类别</b>",
+    'ar': "📁 <b>اختر فئة</b> لتحميل المجموعات",
+}
+l_find_usr_choose = {
+    'ru': "🕵️ <b>Выбери категорию</b> для выгрузки пользователей",
+    'en': "🕵️ <b>Choose a category</b> to upload users",
+    'es': "🕵️ <b>Elige una categoría</b> para subir usuarios",
+    'fr': "🕵️ <b>Choisissez une catégorie</b> pour télécharger des utilisateurs",
+    'zh': "🕵️<b>选择一个类别</b>上传用户",
+    'ar': "🕵️ <b>اختر فئة</b> لتحميل المستخدمين",
+}
+l_find_bot_choose = {
+    'ru': "🥾 <b>Выбери категорию</b> для выгрузки ботов",
+    'en': "🥾 <b>Choose a category</b> for uploading bots",
+    'es': "🥾 <b>Elija una categoría</b> para cargar bots",
+    'fr': "🥾 <b>Choisissez une catégorie</b> pour télécharger des bots",
+    'zh': "🥾<b>选择上传机器人的类别</b>",
+    'ar': "🥾 <b>اختر فئة</b> لتحميل الروبوتات",
+}
 
-# region cpayment_
-l_cpayment_alert = {
-    'ru': "💳️ Нужно ⚙️Настроить хотя бы один платежный токен",
-    'en': "💳️ You need to ⚙️Set up at least one payment token",
-    'es': "💳️ Debes ⚙️Configurar al menos un token de pago",
-    'fr': "💳️ Vous devez ⚙️Configurer au moins un jeton de paiement",
-    'zh': "💳️您需要⚙️设置至少一个支付令牌",
-    'ar': "💳️ تحتاج إلى إعداد رمز دفع واحد على الأقل",
+l_find_chn_find = {
+    'ru': "🔎 Поиск по каналам",
+    'en': "🔎 Channel search",
+    'es': "🔎 Búsqueda de canales",
+    'fr': "🔎 Recherche de chaînes",
+    'zh': "🔎 频道搜索",
+    'ar': "🔎 قناة البحث",
 }
-l_cpayment_text = {
-    'ru': "💳️ <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> платежи в @{0}-боте\n\n👩🏽‍💻 <b>Текущий</b> платежный токен:\n{1}",
-    'en': "💳️ <b>Click</b> on ✅/☑️ to <b>turn on/off</b> payments in @{0}-bot\n\n👩🏽‍💻 <b>Current</b> payment token:\n{1}",
-    'es': "💳️ <b>Haz clic</b> en ✅/☑️ para <b>activar o desactivar</b> los pagos en @{0}-bot\n\n👩🏽‍💻 Token de pago <b>actual</b> :\n{1}",
-    'fr': "💳️ <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> les paiements dans @{0}-bot\n\n👩🏽‍💻 Jeton de paiement <b>actuel</b> :\n{1}",
-    'zh': "💳️<b>点击</b>✅/☑️ 在@{0}-bot 中<b>打开/关闭</b>支付\n\n👩🏽‍💻<b>当前</b>支付令牌：\n{1}",
-    'ar': "💳️ <b>انقر</b> على ✅ / ☑️ <b>لتشغيل / إيقاف</b> المدفوعات في @ {0} -bot\n\n👩🏽‍💻 رمز الدفع <b>الحالي</b> :\n{1}",
+l_find_grp_find = {
+    'ru': "🔎 Поиск по группам",
+    'en': "🔎 Group search",
+    'es': "🔎 Búsqueda de grupos",
+    'fr': "🔎 Recherche de groupe",
+    'zh': "🔎 群组搜索",
+    'ar': "🔎 بحث المجموعة",
 }
-l_cpayment_token = {
-    'ru': "💳️ <b>Вставь</b> платежный токен, полученный из @BotFather-бота\n\n👩🏽‍💻 <b>Например</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 <b>Текущий</b> токен:\n{0}",
-    'en': "💳️ <b>Insert</b> payment token received from @BotFather -bot\n\n👩🏽‍💻 <b>For example</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 <b>Current</b> token:\n{0}",
-    'es': "💳️ <b>Inserte</b> el token de pago recibido de @BotFather -bot\n\n👩🏽‍💻 <b>Por ejemplo,</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 Token <b>actual</b> :\n{0}",
-    'fr': "💳️ <b>Insérez</b> le jeton de paiement reçu de @BotFather -bot\n\n👩🏽‍💻 <b>Par exemple</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 Jeton <b>actuel</b> :\n{0}",
-    'zh': "💳️<b>插入</b>从@BotFather -bot 收到的支付令牌\n\n👩🏽‍💻<b>例如</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻<b>当前</b>令牌：\n{0}",
-    'ar': "💳️ <b>أدخل</b> رمز الدفع المستلم من @BotFather -bot\n\n👩🏽‍💻 <b>على سبيل المثال</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 الرمز <b>المميز الحالي</b> :\n{0}",
+l_find_usr_find = {
+    'ru': "🔎 Поиск по конкурентам",
+    'en': "🔎 Search by competitors",
+    'es': "🔎 Búsqueda por competidores",
+    'fr': "🔎 Recherche par concurrents",
+    'zh': "🔎 按竞争对手搜索",
+    'ar': "🔎 البحث عن طريق المنافسين",
 }
-l_cpayment_done = {
-    'ru': "💳️ <b>Готово!</b>\n\n👩🏽‍💻 <b>Текущий</b> платежный токен для @{0}-бота:\n\n{1}",
-    'en': "💳️ <b>Done!</b>\n\n👩🏽‍💻 <b>Current</b> payment token for @{0}-bot:\n\n{1}",
-    'es': "💳️ <b>Listo!</b>\n\n👩🏽‍💻 Token de pago <b>actual</b> para @{0}-bot:\n\n{1}",
-    'fr': "💳️ <b>C&#x27;est fait !</b>\n\n👩🏽‍💻 Jeton de paiement <b>actuel</b> pour @{0}-bot :\n\n{1}",
-    'zh': "💳️<b>完成！</b>\n\n👩🏽‍💻 @{0}-bot 的<b>当前</b>支付令牌：\n\n{1}",
-    'ar': "💳️ <b>انتهى!</b>\n\n👩🏽‍💻 رمز الدفع <b>الحالي</b> لـ @ {0} -bot:\n\n{1}",
+l_find_bot_find = {
+    'ru': "🔎 Поиск по ботам",
+    'en': "🔎 Search by bots",
+    'es': "🔎 Búsqueda por bots",
+    'fr': "🔎 Recherche par bots",
+    'zh': "🔎 机器人搜索",
+    'ar': "🔎 البحث عن طريق الروبوتات",
 }
-# endregion
 
+l_find_chn_link = {
+    'ru': "🔗 Перейти к каналу",
+    'en': "🔗 Go to channel",
+    'es': "🔗 Ir al canal",
+    'fr': "🔗 Aller à la chaîne",
+    'zh': "🔗 前往频道",
+    'ar': "🔗 اذهب إلى القناة",
+}
+l_find_grp_link = {
+    'ru': "🔗 Перейти к группе",
+    'en': "🔗 Go to group",
+    'es': "🔗 Ir al grupo",
+    'fr': "🔗 Aller au groupe",
+    'zh': "🔗 进群",
+    'ar': "🔗 اذهب إلى المجموعة",
+}
+l_find_usr_link = {
+    'ru': "🔗 Перейти к пользователю",
+    'en': "🔗 Go to user",
+    'es': "🔗 Ir a usuario",
+    'fr': "🔗 Aller à l'utilisateur",
+    'zh': "🔗 转到用户",
+    'ar': "🔗 اذهب إلى المستخدم",
+}
+l_find_bot_link = {
+    'ru': "🔗 Перейти к боту",
+    'en': "🔗 Go to bot",
+    'es': "🔗 Ir al bot",
+    'fr': "🔗 Aller au robot",
+    'zh': "🔗 转到机器人",
+    'ar': "🔗 اذهب إلى bot",
+}
 
-# region cintegration_
-l_cintegration_alert = {
-    'ru': "🗝️ Нужно ⚙️Настроить ССЫЛКУ доступа",
-    'en': "🗝️ You need to ⚙️Set up an access link",
-    'es': "🗝️ Debes ⚙️Configurar un enlace de acceso",
-    'fr': "🗝️ Vous devez ⚙️Configurer un lien d'accès",
-    'zh': "🗝️您需要⚙️设置访问链接",
-    'ar': "🗝️ تحتاج إلى إعداد ارتباط وصول",
+l_find_category_blog = {
+    'ru': "#блогер",
+    'en': "#blogger",
+    'es': "#bloguero",
+    'fr': "#blogueur",
+    'zh': "#博主",
+    'ar': "#مدَّوِن",
 }
-l_cintegration_text = {
-    'ru': "🗝️ <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> интеграцию базы пользователей с <i><b>google</b>-crm/<b>airtable</b>-crm</i>\n\n👩🏽‍💻 Например, опция [<b>{0}</b>] означает возможность интеграции базы пользователей с <i>google-crm</i>",
-    'en': "🗝️ <b>Click</b> on ✅/☑️ to <b>enable/disable</b> integration of user base with <i><b>google</b> -crm/ <b>airtable</b> -crm</i>\n\n👩🏽‍💻 For example, option [<b>{0}</b>] means the ability to integrate user base with <i>google-crm</i>",
-    'es': "🗝️ <b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> la integración de la base de usuarios con <i><b>google</b> -crm/ <b>airtable</b> -crm</i>\n\n👩🏽‍💻 Por ejemplo, la opción [<b>{0}</b>] significa la capacidad de integrar la base de usuarios con <i>google-crm</i>",
-    'fr': "🗝️ <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> l&#x27;intégration de la base d&#x27;utilisateurs avec <i><b>google</b> -crm/ <b>airtable</b> -crm</i>\n\n👩🏽‍💻 Par exemple, l&#x27;option [<b>{0}</b>] signifie la possibilité d&#x27;intégrer la base d&#x27;utilisateurs avec <i>google-crm</i>",
-    'zh': "🗝️<b>点击</b>✅/☑️<b>启用/禁用</b>用户群与<i><b>google</b> -crm/ <b>airtable</b> -crm</i>\n\n👩🏽‍💻 例如，选项 [<b>{0}</b>] 表示能够将用户群与<i>google-crm</i>集成",
-    'ar': "🗝️ <b>انقر</b> على ✅ / ☑️ <b>لتمكين / تعطيل</b> تكامل قاعدة المستخدمين مع <i><b>google</b> -crm / <b>airtable</b> -crm</i>\n\n👩🏽‍💻 على سبيل المثال ، الخيار [<b>{0}</b>] يعني القدرة على تكامل قاعدة المستخدمين مع <i>google-crm</i>",
+l_find_category_digit = {
+    'ru': "#оцифровка",
+    'en': "#digitizer",
+    'es': "#digitalizador",
+    'fr': "#numériseur",
+    'zh': "#数字转换器",
+    'ar': "#جهاز التحويل الرقمي",
+}
+l_find_category_smm = {
+    'ru': "#смм",
+    'en': "#smm",
+    'es': "#mmm",
+    'fr': "#nm",
+    'zh': "#嗯",
+    'ar': "#سم",
+}
+l_find_category_recruit = {
+    'ru': "#рекрут",
+    'en': "#recruit",
+    'es': "#recluta",
+    'fr': "#recruter",
+    'zh': "#招募",
+    'ar': "#تجنيد",
+}
+l_find_category_design = {
+    'ru': "#дизайн",
+    'en': "#design",
+    'es': "#diseño",
+    'fr': "#conception",
+    'zh': "#设计",
+    'ar': "#تصميم",
+}
+l_find_category_coach = {
+    'ru': "#коуч",
+    'en': "#coach",
+    'es': "#entrenador",
+    'fr': "#entraîneur",
+    'zh': "#教练",
+    'ar': "#مدرب",
+}
+l_find_category_it = {
+    'ru': "#ИТ",
+    'en': "#DOG",
+    'es': "#PERRO",
+    'fr': "#CHIEN",
+    'zh': "#狗",
+    'ar': "#كلب",
+}
+l_find_category_course = {
+    'ru': "#курсы",
+    'en': "#courses",
+    'es': "#cursos",
+    'fr': "#cours",
+    'zh': "#培训班",
+    'ar': "#الدورات",
+}
+l_find_category_business = {
+    'ru': "#бизнес",
+    'en': "#business",
+    'es': "#negocio",
+    'fr': "#entreprise",
+    'zh': "#商业",
+    'ar': "#عمل",
+}
+l_find_category_goods = {
+    'ru': "#товарка",
+    'en': "#cargo",
+    'es': "#carga",
+    'fr': "#cargaison",
+    'zh': "#货物",
+    'ar': "#البضائع",
+}
+l_find_category_offline = {
+    'ru': "#оффлайн",
+    'en': "#offline",
+    'es': "#desconectado",
+    'fr': "#hors ligne",
+    'zh': "#离线",
+    'ar': "#غير متصل على الانترنت",
+}
+l_find_category_lawyer = {
+    'ru': "#юрист",
+    'en': "#lawyer",
+    'es': "#abogado",
+    'fr': "#avocat",
+    'zh': "#律师",
+    'ar': "#محامي",
+}
+l_find_category_verified = {
+    'ru': "#верифиц",
+    'en': "#verification",
+    'es': "#verificación",
+    'fr': "#vérification",
+    'zh': "#确认",
+    'ar': "#تَحَقّق",
+}
+l_find_category_premium = {
+    'ru': "#премиум",
+    'en': "#premium",
+    'es': "#de primera calidad",
+    'fr': "#prime",
+    'zh': "#优质的",
+    'ar': "#غالي",
+}
+l_find_category_health = {
+    'ru': "#здоровье",
+    'en': "#health",
+    'es': "#salud",
+    'fr': "#santé",
+    'zh': "#健康",
+    'ar': "#صحة",
 }
 
-l_cintegration_google_on = {
-    'ru': "✅☑Вкл google-crm",
-    'en': "✅☑Includes google-crm",
-    'es': "✅☑Incluye google-crm",
-    'fr': "✅☑Inclut google-crm",
-    'zh': "✅☑包括谷歌客户关系管理",
-    'ar': "✅☑ يشمل google-crm",
+l_find_category_getting = {
+    'ru': "🔎 Выгружаем <b>категорию</b> {0}..\n\n#длительность 0мин",
+    'en': "🔎 Upload <b>category</b> {0}..\n\n#duration 0min",
+    'es': "🔎 Subir <b>categoría</b> {0}..\n\n#duración 0min",
+    'fr': "🔎 <b>Catégorie</b> de téléchargement {0}..\n\n#durée 0min",
+    'zh': "🔎 上传<b>类别</b>{0}..\n\n#duration 0min",
+    'ar': "🔎 <b>فئة</b> التحميل {0} ..\n\n# المدة 0 دقيقة",
 }
-l_cintegration_google_off = {
-    'ru': "☑️☐Выкл google-crm",
-    'en': "☑️☐Выкл google-crm",
-    'es': "☑️☐Выкл google-crm",
-    'fr': "☑️☐Выкл google-crm",
-    'zh': "☑️☐Выкл 谷歌客户关系管理",
-    'ar': "☑️☐Выкл google-crm",
+l_find_keyword_getting = {
+    'ru': "🔎 Выгружаем базу по ключевым словам <i>{0}</i>..\n\n#длительность 1мин",
+    'en': "🔎 Unload the database by keywords <i>{0}</i> ..\n\n#duration 1 min",
+    'es': "🔎 Descarga la base de datos por palabras clave <i>{0}</i> ..\n\n#duración 1 min",
+    'fr': "🔎 Décharger la base de données par mots clés <i>{0}</i> ..\n\n#durée 1 min",
+    'zh': "🔎 通过关键字<i>{0}</i>卸载数据库 ..\n\n#duration 1 分钟",
+    'ar': "🔎 تفريغ قاعدة البيانات بالكلمات الأساسية <i>{0}</i> ..\n\n# المدة 1 دقيقة",
 }
-l_cintegration_airtable_on = {
-    'ru': "✅☑Вкл airtable-crm",
-    'en': "✅☑Includes airtable-crm",
-    'es': "✅☑Incluye airtable-crm",
-    'fr': "✅☑Comprend airtable-crm",
-    'zh': "✅☑包括 airtable-crm",
-    'ar': "✅☑ يشمل airtable-crm",
+l_find_category_keywords = {
+    'ru': "📰 <b>Введи</b> ключевые слова для поиска через пробелы или разделители",
+    'en': "📰 <b>Enter</b> keywords to search through spaces or delimiters",
+    'es': "📰 <b>Ingrese</b> palabras clave para buscar a través de espacios o delimitadores",
+    'fr': "📰 <b>Entrez</b> des mots-clés pour rechercher dans des espaces ou des délimiteurs",
+    'zh': "📰<b>输入</b>关键字以通过空格或分隔符进行搜索",
+    'ar': "📰 <b>أدخل</b> كلمات أساسية للبحث من خلال المسافات أو المحددات",
 }
-l_cintegration_airtable_off = {
-    'ru': "☑️☐Выкл airtable-crm",
-    'en': "☑️☐Выкл airtable-crm",
-    'es': "☑️☐Выкл airtable-crm",
-    'fr': "☑️☐Выкл airtable-crm",
-    'zh': "☑️☐Выкл airtable-crm",
-    'ar': "☑️☐Выкл airtable-crm",
+l_find_reached = {
+    'ru': "<b>Охват</b>: <u>{0}</u> польз.",
+    'en': "<b>Reach</b> : <u>{0}</u> users",
+    'es': "<b>Alcance</b> : <u>{0}</u> usuarios",
+    'fr': "<b>Atteignez</b> : <u>{0}</u> utilisateurs",
+    'zh': "<b>覆盖</b>： <u>{0}</u>个用户",
+    'ar': "<b>الوصول</b> : <u>{0}</u> مستخدمين",
+}
+l_find_watch = {
+    'ru': "🔎 Просмотр",
+    'en': "🔎 View",
+    'es': "🔎 Ver",
+    'fr': "🔎 Voir",
+    'zh': "🔎 查看",
+    'ar': "🔎 عرض",
+}
+l_add_join_err = {
+    'ru': "👩🏽‍💻 <b>Ошибка</b> (вставь корректную ссылку или повтори позже)",
+    'en': "🚫 Failed to add {0} to the database, you need to open free access to join",
+    'es': "🚫 No se pudo agregar {0} a la base de datos, debe abrir el acceso gratuito para unirse",
+    'fr': "🚫 Échec de l'ajout de {0} à la base de données, vous devez ouvrir un accès gratuit pour rejoindre",
+    'zh': "🚫 添加{0}到数据库失败，需要开通免费权限才能加入",
+    'ar': "🚫 فشل إضافة {0} إلى قاعدة البيانات ، تحتاج إلى فتح وصول مجاني للانضمام",
 }
 
-l_cintegration_google = {
-    'ru': "🗝️ <b>Вставь ссылку</b> на пустую google-таблицу (<i>с открытым доступом для редактирования</i>) для интеграции с базой пользователей @{0}-бота\n\n👩🏽‍💻 <b>Например</b>, https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 <b>Текущая</b> ссылка:\n{1}",
-    'en': "🗝️ <b>Insert a link</b> to an empty google spreadsheet ( <i>with open access for editing</i> ) to integrate with the @{0}-bot user base\n\n👩🏽‍💻 <b>For example</b> , https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 <b>Current</b> URL:\n{1}",
-    'es': "🗝️ <b>Inserta un enlace</b> a una hoja de cálculo de Google vacía ( <i>con acceso abierto para editar</i> ) para integrarla con la base de usuarios de @{0}-bot\n\n👩🏽‍💻 <b>Por ejemplo</b> , https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 URL <b>actual</b> :\n{1}",
-    'fr': "🗝️ <b>Insérez un lien</b> vers une feuille de calcul Google vide ( <i>avec accès ouvert pour modification</i> ) à intégrer à la base d&#x27;utilisateurs @{0}-bot\n\n👩🏽‍💻 <b>Par exemple</b> , https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 URL <b>actuelle</b> :\n{1}",
-    'zh': "🗝️<b>插入指向空谷歌电子表格的链接</b>（<i>开放编辑权限</i>）以与@{0}-bot 用户群集成\n\n👩🏽‍💻<b>例如</b>，https: https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻<b>当前</b>网址：\n{1}",
-    'ar': "🗝️ <b>أدخل رابطًا</b> إلى جدول بيانات google فارغ ( <i>مع وصول مفتوح للتعديل</i> ) للتكامل مع @ {0} -bot user base\n\n👩🏽‍💻 <b>على سبيل المثال</b> ، https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 عنوان URL <b>الحالي</b> :\n{1}",
+l_add_chn_fail = {
+    'ru': "🚫 <b>Канал</b> {0} не добавлен в базу\n\n{1} аватар\n{2} описание\n{3} более {4} подписчиков\n{5} последний пост менее {6} дней назад",
+    'en': "🚫 Channel {0} - not added to the database\n\n{1} avatar\n{2} >100 subscribers\n{3} last post <100 days ago",
+    'es': "🚫 Canal {0} - no agregado a la base de datos\n\n{1} avatar\n{2} >100 suscriptores\n{3} última publicación <100 días atrás",
+    'fr': "🚫 Chaîne {0} - non ajoutée à la base de données\n\n{1} avatar\n{2} >100 abonnés\n{3} dernier message il y a <100 jours",
+    'zh': "🚫 频道 {0} - 未添加到数据库\n\n{1} 头像\n{2} >100 个订阅者\n{3} 上次发布 <100 天前",
+    'ar': "🚫 القناة {0} - لم تتم إضافتها إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2}> 100 مشترك\n{3} آخر مشاركة قبل أقل من 100 يوم",
 }
-l_cintegration_airtable = {
-    'ru': "🗝️ <b>Вставь ссылку</b> на пустую airtable-таблицу (<i>с открытым доступом для редактирования и любого e-mail</i>) для интеграции с базой пользователей @{0}-бота\n\n👩🏽‍💻 <b>Например</b>, https://airtable.com/invite/l?inviteId=inv4VGM&inviteToken=f1d31f9aba6b&utm_medium=email\n\n👩🏽‍💻 <b>Текущая</b> ссылка:\n{1}",
-    'en': "🗝️ <b>Insert a link</b> to an empty airtable-table ( <i>with open access for editing and any e-mail</i> ) for integration with the @{0}-bot user base\n\n👩🏽‍💻 <b>For example</b> , https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email\n\n👩🏽‍💻 <b>Current</b> URL:\n{1}",
-    'es': "🗝️ <b>Inserte un enlace</b> a una mesa de aire vacía ( <i>con acceso abierto para editar y cualquier correo electrónico</i> ) para la integración con la base de usuarios de @{0}-bot\n\n👩🏽‍💻 <b>Por ejemplo</b> , https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email\n\n👩🏽‍💻 URL <b>actual</b> :\n{1}",
-    'fr': "🗝️ <b>Insérez un lien</b> vers une table airtable vide ( <i>avec un accès ouvert pour l&#x27;édition et tout e-mail</i> ) pour l&#x27;intégration avec la base d&#x27;utilisateurs @{0}-bot\n\n👩🏽‍💻 <b>Par exemple</b> , https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email\n\n👩🏽‍💻 URL <b>actuelle</b> :\n{1}",
-    'zh': "🗝️<b>插入一个指向空的 airtable-table 的链接</b>（<i>具有编辑和任何电子邮件的开放访问权限</i>）以与 @{0}-bot 用户群集成\n\n👩🏽‍💻<b>例如</b>， https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email\n\n👩🏽‍💻<b>当前</b>网址：\n{1}",
-    'ar': "🗝️ <b>أدخل ارتباطًا</b> إلى جدول airtable فارغ ( <i>مع وصول مفتوح للتحرير وأي بريد إلكتروني</i> ) للتكامل مع @ {0} -bot user base\n\n👩🏽‍💻 <b>على سبيل المثال</b> ، https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email <b>؟</b>",
+l_add_grp_fail = {
+    'ru': "🚫 <b>Группа</b> {0} не добавлена в базу\n\n{1} аватар\n{2} описание\n{3} более {4} участников\n{5} последний пост менее {6} дней назад",
+    'en': "🚫 Group {0} - not added to the database\n\n{1} avatar\n{2} >100 members\n{3} last post <100 days ago",
+    'es': "🚫 Grupo {0} - no agregado a la base de datos\n\n{1} avatar\n{2} >100 miembros\n{3} última publicación <100 días atrás",
+    'fr': "🚫 Groupe {0} - non ajouté à la base de données\n\n{1} avatar\n{2} >100 membres\n{3} dernier message il y a <100 jours",
+    'zh': "🚫 组 {0} - 未添加到数据库\n\n{1} 头像\n{2} >100 名成员\n{3} 上次发帖 <100 天前",
+    'ar': "🚫 المجموعة {0} - لم تتم إضافتها إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2}> 100 عضو\n{3} آخر مشاركة منذ أقل من 100 يوم",
 }
-l_cintegration_done = {
-    'ru': "🗝️ <b>Готово!</b>\n\n👩🏽‍💻 <b>Текущая</b> ссылка:\n{0}",
-    'en': "🗝️ <b>Done!</b>\n\n👩🏽‍💻 <b>Current</b> URL:\n{0}",
-    'es': "🗝️ <b>Listo!</b>\n\n👩🏽‍💻 URL <b>actual</b> :\n{0}",
-    'fr': "🗝️ <b>C&#x27;est fait !</b>\n\n👩🏽‍💻 URL <b>actuelle</b> :\n{0}",
-    'zh': "🗝️<b>完成！</b>\n\n👩🏽‍💻<b>当前</b>网址：\n{0}",
-    'ar': "🗝️ <b>انتهى!</b>\n\n👩🏽‍💻 عنوان URL <b>الحالي</b> :\n{0}",
+l_add_usr_fail = {
+    'ru': "🚫 <b>Пользователь</b> {0} не добавлен в базу\n\n{1} аватар\n{2} @username\n{3} био",
+    'en': "🚫 User {0} - not added to database\n\n{1} avatar\n{2} @username\n{3} bio",
+    'es': "🚫 Usuario {0}: no agregado a la base de datos\n\n{1} avatar\n{2} @username\n{3} biografía",
+    'fr': "🚫 Utilisateur {0} - non ajouté à la base de données\n\n{1} avatar\n{2} @username\n{3} bio",
+    'zh': "🚫 用户 {0} - 未添加到数据库\n\n{1} 头像\n{2} @username\n{3} 简介",
+    'ar': "🚫 المستخدم {0} - لم تتم إضافته إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2} @username\n{3} السيرة الذاتية",
+}
+l_add_bot_fail = {
+    'ru': "🚫 <b>Бот</b> {0} не добавлен в базу\n\n{1} аватар\n{2} описание",
+    'en': "🚫 Bot {0} - not added to the database\n\n{1} avatar\n{2} description",
+    'es': "🚫 Bot {0} - no agregado a la base de datos\n\n{1} avatar\n{2} descripción",
+    'fr': "🚫 Bot {0} - non ajouté à la base de données\n\n{1} description de l'avatar\n{2}",
+    'zh': "🚫 机器人 {0} - 未添加到数据库\n\n{1} 头像\n{2} 描述",
+    'ar': "🚫 بوت {0} - لم تتم إضافته إلى قاعدة البيانات\n\n{1} الصورة الرمزية\n{2} الوصف",
 }
-# endregion
 
+l_add_chn_done = {
+    'ru': "✅ <b>Канал</b> {0} - добавлен в базу и обновлен",
+    'en': "✅ Channel {0} - added to the database and updated",
+    'es': "✅ Canal {0}: agregado a la base de datos y actualizado",
+    'fr': "✅ Chaîne {0} - ajoutée à la base de données et mise à jour",
+    'zh': "✅ 频道 {0} - 添加到数据库并更新",
+    'ar': "✅ القناة {0} - تمت إضافتها إلى قاعدة البيانات وتحديثها",
+}
+l_add_grp_done = {
+    'ru': "✅ <b>Группа</b> {0} - добавлена в базу и обновлена",
+    'en': "✅ Group {0} - added to the database and updated",
+    'es': "✅ Grupo {0}: agregado a la base de datos y actualizado",
+    'fr': "✅ Groupe {0} - ajouté à la base de données et mis à jour",
+    'zh': "✅ 组 {0} - 添加到数据库并更新",
+    'ar': "✅ المجموعة {0} - تمت إضافتها إلى قاعدة البيانات وتحديثها",
+}
+l_add_usr_done = {
+    'ru': "✅ <b>Пользователь</b> {0} - добавлен в базу и обновлен",
+    'en': "✅ User {0} - added to the database and updated",
+    'es': "✅ Usuario {0}: agregado a la base de datos y actualizado",
+    'fr': "✅ Utilisateur {0} - ajouté à la base de données et mis à jour",
+    'zh': "✅ 用户 {0} - 添加到数据库并更新",
+    'ar': "✅ المستخدم {0} - تمت إضافته إلى قاعدة البيانات وتحديثها",
+}
+l_add_bot_done = {
+    'ru': "✅ <b>Бот</b> {0} - добавлен в базу и обновлен",
+    'en': "✅ Bot {0} - added to the database and updated",
+    'es': "✅ Bot {0}: agregado a la base de datos y actualizado",
+    'fr': "✅ Bot {0} - ajouté à la base de données et mis à jour",
+    'zh': "✅ Bot {0} - 添加到数据库并更新",
+    'ar': "✅ بوت {0} - تمت إضافته إلى قاعدة البيانات وتحديثها",
+}
 
-# region cnotification_
-l_cnotification_text = {
-    'ru': "💬 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> оповещения о <i><b>/start-stop</b> запуске/блокировке бота пользователем и попадании пользователя в <b>/ban</b>-список/<b>нажатии</b> на кнопки пользователем/<b>диалоге</b> с администраторами/<b>всех</b> действиях пользователя</i>\n\n👩🏽‍💻 Например, опция [<b>{0}</b>] означает показ сообщений от пользователя администраторам бота (/admin) с возможностью реплай-ответа на сообщения",
-    'en': "💬 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> notifications about <i><b>/start-stop</b> launching/blocking the bot by the user and getting the user into the <b>/ban</b> -list/ <b>pressing</b> buttons by the user/ <b>dialog</b> with administrators/ <b>all</b> user actions</i>\n\n👩🏽‍💻 For example, the option [<b>{0}</b>] means показ messages from the user to bot administrators (/admin) with the ability to replay response to messages",
-    'es': "💬 <b>Haga clic</b> en ✅/☑️ para <b>activar/desactivar</b> las notificaciones sobre <i><b>/iniciar y detener</b> el lanzamiento/bloqueo del bot por parte del usuario y colocar al usuario en la <b>/lista de prohibición</b> / <b>pulsar</b> botones por parte del usuario/ <b>diálogo</b> con los administradores/ <b>todas</b> las acciones del usuario \</i> n\n👩🏽‍💻 Por ejemplo, la opción [<b>{0}</b>] significa показ los mensajes del usuario a los administradores del bot (/admin) con la capacidad de reproducir la respuesta a los mensajes.",
-    'fr': "💬 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> les notifications sur <i><b>/start-stop</b> lancer/bloquer le bot par l&#x27;utilisateur et faire entrer l&#x27;utilisateur dans la <b>/banni</b> -liste/ <b>appuyer sur</b> les boutons par l&#x27;utilisateur/ <b>dialogue</b> avec les administrateurs/ <b>toutes</b> les actions de l&#x27;utilisateur \</i> n\n👩🏽‍💻 Par exemple, l&#x27;option [<b>{0}</b>] signifie показ les messages de l'utilisateur aux administrateurs du bot (/admin) avec la possibilité de rejouer la réponse aux messages",
-    'zh': "💬<b>单击</b>✅/☑️ 以<b>打开/关闭</b><i>关于<b>/start-stop</b>启动/阻止用户的机器人并让用户进入<b>/ban</b>列表/用户<b>按下</b>按钮/与管理员<b>对话</b>/<b>所有</b>用户操作的通知 \</i> n\n👩🏽‍💻 例如，选项 [<b>{0}</b>] 表示将用户的消息показ给机器人管理员 (/admin)，并能够重播对消息的响应",
-    'ar': "💬 <b>انقر</b> فوق ✅ / ☑️ <b>لتشغيل / إيقاف تشغيل</b> <i>الإشعارات حول <b>/ بدء - إيقاف</b> تشغيل / حظر الروبوت من قبل المستخدم وإدخال المستخدم في أزرار <b>/ قائمة الحظر</b> / <b>الضغط</b> بواسطة المستخدم / <b>الحوار</b> مع المسؤولين / <b>جميع</b> إجراءات المستخدم \</i> n\n👩🏽‍💻 على سبيل المثال ، الخيار [<b>{0}</b>] يعني показ الرسائل من المستخدم إلى المشرفين (/ admin) مع إمكانية إعادة الرد على الرسائل",
+l_find_chn_done = {
+    'ru': "🔥 <b>Готово!</b> По {0} собрано <u>{1}</u> каналов, сегментированных по <i>ключевым</i> словам\n\n<b>Охват</b>: <u>{2}</u> польз\n\nМожно связаться с администраторами каналов, чтобы заказать рекламу",
+    'en': "🔥 <b>Done!</b> {0} collected <u>{1}</u> channels segmented by <i>keywords</i>\n\n<b>Reach</b> : <u>{2}</u> users\n\nYou can contact channel administrators to order advertising",
+    'es': "🔥 <b>Listo!</b> {0} recopilaron <u>{1}</u> canales segmentados por <i>palabras clave</i>\n\n<b>Alcance</b> : <u>{2}</u> usuarios\n\nPuede ponerse en contacto con los administradores del canal para solicitar publicidad",
+    'fr': "🔥 <b>C&#x27;est fait !</b> {0} a collecté <u>{1}</u> chaînes segmentées par <i>mots-clés</i>\n\n<b>Atteinte</b> : <u>{2}</u> utilisateurs\n\nVous pouvez contacter les administrateurs de chaîne pour commander de la publicité",
+    'zh': "🔥<b>完成！</b> {0} 收集了<u>{1} 个</u>按<i>关键字</i>细分的频道\n\n<b>覆盖</b>： <u>{2} 个</u>用户\n\n您可以联系频道管理员订购广告",
+    'ar': "🔥 <b>انتهى!</b> القنوات {0} المجمعة <u>{1}</u> المقسمة حسب <i>الكلمات الرئيسية</i>\n\n<b>الوصول إلى</b> : <u>{2}</u> المستخدمين\n\nيمكنك الاتصال بمسؤولي القناة لطلب الإعلانات",
 }
-l_cnotification_start_on = {
-    'ru': "✅☑Вкл /start-stop-/ban",
-    'en': "✅☑On /start-stop-/ban",
-    'es': "✅☑Activar/iniciar-detener-/prohibir",
-    'fr': "✅☑On /start-stop-/interdiction",
-    'zh': "✅☑开/启-停-/禁",
-    'ar': "✅☑ On / start-stop- / ban",
+l_find_grp_done = {
+    'ru': "🔥 <b>Готово!</b> По {0} собрано <u>{1}</u> чатов, сегментированных по <i>ключевым</i> словам\n\n<b>Охват</b>: <u>{2}</u> польз\n\nМожно сделать <b>рассылку</b> по группам",
+    'en': "🔥 <b>Done!</b> {0} collected <u>{1}</u> chats, segmented by <i>keywords</i>\n\n<b>Reach</b> : <u>{2}</u> users\n\nCan be <b>sent</b> to groups",
+    'es': "🔥 <b>Listo!</b> {0} <u>{1}</u> chats recopilados, segmentados por <i>palabras clave</i>\n\n<b>Alcance</b> : <u>{2}</u> usuarios\n\nSe puede <b>enviar</b> a grupos",
+    'fr': "🔥 <b>C&#x27;est fait !</b> {0} a collecté <u>{1}</u> chats, segmentés par <i>mots-clés</i>\n\n<b>Atteinte</b> : <u>{2}</u> utilisateurs\n\nPeut être <b>envoyé</b> à des groupes",
+    'zh': "🔥<b>完成！</b> {0} 收集了<u>{1} 个</u>聊天，按<i>关键字细分</i>\n\n<b>覆盖</b>： <u>{2} 个</u>用户\n\n可以<b>发送</b>到组",
+    'ar': "🔥 <b>انتهى!</b> {0} دردشات <u>{1}</u> مجمعة ، مقسمة حسب <i>الكلمات الرئيسية</i>\n\n<b>مدى الوصول</b> : <u>{2}</u> مستخدمين\n\nيمكن <b>إرسالها</b> إلى مجموعات",
 }
-l_cnotification_start_off = {
-    'ru': "☑️☐Выкл /start-stop-/ban",
-    'en': "☑️☐Выкл /start-stop-/ban",
-    'es': "☑️☐Выкл /start-stop-/ban",
-    'fr': "☑️☐Выкл /start-stop-/ban",
-    'zh': "☑️☐Выкл /开始-停止-/禁止",
-    'ar': "☑️☐Выкл / start-stop- / الحظر",
+l_find_usr_done = {
+    'ru': "🔥 <b>Готово!</b> По {0} собрано <u>{1}</u> пользователей, сегментированных по <i>ключевым</i> словам\n\nМожно сразу сделать <b>рассылку</b> или подписку-<b>инвайт</b> в чат по <i>полученным</i> лидам",
+    'en': "🔥 <b>Done!</b> {0} collected <u>{1}</u> users, segmented by <i>keywords</i>\n\nYou can immediately make <b>a mailing list</b> or subscribe <b>- invite</b> to the chat according to <i>the received</i> leads",
+    'es': "🔥 <b>Listo!</b> {0} recolectó <u>{1}</u> usuarios, segmentados por <i>palabras clave</i>\n\nPuede crear <b>una lista de correo</b> o suscribirse inmediatamente <b>: invite</b> al chat de acuerdo con <i>los clientes potenciales recibidos</i>",
+    'fr': "🔥 <b>C&#x27;est fait !</b> {0} utilisateurs collectés <u>{1}</u> , segmentés par <i>mots-clés</i>\n\nVous pouvez immédiatement créer <b>une liste de diffusion</b> ou vous abonner <b>- inviter</b> au chat en fonction <i>des prospects reçus</i>",
+    'zh': "🔥<b>完成！</b> {0} 收集了<u>{1} 个</u>用户，按<i>关键字</i>细分\n\n您可以立即制作<b>邮件列表</b>或订阅<b>-</b>根据<i>收到的</i>线索邀请聊天",
+    'ar': "🔥 <b>انتهى!</b> {0} تم تجميع <u>{1}</u> مستخدمين ، مقسمين حسب <i>الكلمات الرئيسية</i>\n\nيمكنك على الفور إنشاء <b>قائمة بريدية</b> أو الاشتراك <b>- قم بدعوة</b> إلى الدردشة وفقًا للعملاء <i>المحتملين المستلمين</i>",
 }
-l_cnotification_push_on = {
-    'ru': "✅☑Вкл нажатие на кнопки",
-    'en': "✅☑On pressing buttons",
-    'es': "✅☑Al presionar botones",
-    'fr': "✅☑En appuyant sur les boutons",
-    'zh': "✅☑按下按钮",
-    'ar': "✅☑ عند الضغط على الأزرار",
+l_find_bot_done = {
+    'ru': "🔥 <b>Готово!</b> По {0} собрано <u>{1}</u> ботов, сегментированных по <i>ключевым</i> словам",
+    'en': "🔥 <b>Done!</b> {0} collected <u>{1}</u> bots segmented by <i>keywords</i>",
+    'es': "🔥 <b>Listo!</b> {0} recopilaron <u>{1}</u> bots segmentados por <i>palabras clave</i>",
+    'fr': "🔥 <b>C&#x27;est fait !</b> {0} collecté <u>{1}</u> bots segmentés par <i>mots-clés</i>",
+    'zh': "🔥<b>完成！</b> {0} 收集了<u>{1} 个</u><i>按关键字</i>细分的机器人",
+    'ar': "🔥 <b>انتهى!</b> {0} جمعت <u>{1}</u> برامج التتبع مقسمة حسب <i>الكلمات الرئيسية</i>",
 }
-l_cnotification_push_off = {
-    'ru': "☑️☐Выкл нажатие на кнопки",
-    'en': "☑️☐Off pressing the buttons",
-    'es': "☑️☐Apagado presionando los botones",
-    'fr': "☑️☐Off en appuyant sur les boutons",
-    'zh': "☑️☐关闭按钮",
-    'ar': "☑️☐ إيقاف الضغط على الأزرار",
+l_hashtag_categories = {
+    "BLOG": ["blog", "блог", "влог", "блогер", "контентмейкер", 'contentmaker', 'youtube', 'путешестви',
+             "курс", 'getcourse', 'геткурс', "английск", 'школ', "school", "запуск", 'заняти', 'урок', 'воркшоп',
+             "language", "онлайн-школ", "онлайн школ", 'лингвист', 'linguist', 'марафон', 'практикум', 'семинар',
+             'вебинар', 'лаборатор', 'хакатон', 'интенсив', 'обучени', 'запуск', 'колледж', 'институт',
+             'университет', 'лекци', 'мастермайнд', 'симпозиум', 'тренинг', 'тимбилдинг', 'мастерск', 'образовани',
+             'المدونة', 'blogue', '博客',
+             ],
+    "DIGIT": ['оцифров', "фин.", 'финан', 'бух', 'инвест', 'франш', 'трейд', 'бирж', 'кредит', "учет",
+              "банк", "торг", "кассы", "денежн", "консалт", 'consult', 'finan', 'business', "доход",
+              '数字化', 'digitalización', 'numérisation', 'الرقمنة',
+              'استشارة', '谘询', 'consulter', 'consultar',
+              ],
+    "SMM": ['smm', 'смм', 'инста', 'inst', "facebook", 'tiktok', "тикток", 'tik-tok', "тик-ток", 'youtube', 'маркето',
+            'маркети', 'market', 'таргет', "target", 'распаковка', 'продвижение', 'seo', 'сео', 'бренд', "агентство",
+            "лиды", "vkontakte", "вконтакте", "лидов", "реклам", 'taplink', "прогрев", "блог", "визуал", "запуск",
+            "трафик", "mvp", "редакция", 'директ',
+            'سم', '市场推广', 'التسويق', 'comercialización', 'commercialisation', '',
+            ],
+    "RECRUIT": ["рекрут", "роп", "работа", "фриланc", "freela", "найм", "hr", "pr", "персонал", "менеджер",
+                "продаж", "ассист", "риелтор", 'млм', 'mlm', "управлен", "наем", "сотрудн", "делегир", "карьер",
+                'recruit', 'تجنيد', '招聘人员', 'recruter', 'recluta',
+                'لحسابهم الخاص', '自由撰稿人', 'indépendant',
+                ],
+    "DESIGN": ["дизайн", "design", "интерьер", "декор", "мебел", "3d", "архитект", "двери", "ремонт", "строител",
+                "фасад", 'тексти', "рису", "креатив", "визуал", "ландшафт", "художн", "картин",
+                 "имидж", "камин", "монтаж", 'граф', 'искусств', 'рукодел',
+                 '设计', 'التصميم', 'conception', 'diseño',
+                 'interior', 'interior', 'intérieur', 'الداخلية', 'الداخلية',
+               'architecture', 'architecture', 'arquitectura', '建筑设计', 'العمارة',
+               'creative', '创意', 'creativo', 'créativité', 'الإبداع',
+               ],
+    "COACH": ["коуч", "coach", 'консульт', 'продюсер', "бизнес", "наставн", "оратор", "энерг", "эксперт", "психо",
+              "трекер", 'гайд',
+              "практик", "бренд", "тайм", "мотива", "логопед", "мышлен", "нумеролог", "таролог", "йог",
+              "ментор", "тренер", "гештальт", "предприним", "метафори", "денеж", "диагност", "icf",
+              '教练', 'مدرب',
+              'producer', 'productor', 'producteur', '生产商', 'المنتج',
+              'mentor', '导师', 'مينتور', '',
+              ],
+    "IT": ["лендинг", "crm", 'kotlin', 'swift', 'flutter', 'c++', 'c#', 'unity', 'angular',
+           'amocrm', "powerbi", 'программирова', 'tilda', 'frontend', 'backend', 'python', 'ux/ui',
+           "битрикс", 'автоматизаци', 'автоворон', 'разработч', 'java',
+           "developer", 'блокчейн', 'blockchain', 'startup', 'coding',
+           'développeur', 'desarrollador', '开发人员', 'المطور',
+           ],
+    "BUSINESS": ["business", "бизнес", "инвест", "франш", "кредит", "торг", "консалт", "consult",
+                 "доход", "представит", "предпринимат", "коммерц", "фирм", "предприят", "компани", "промышл",
+                 "производст", "invest", "капитал", "capital", "корпорац", "агентств", "пассив",
+                 "дистриб", "акцио", "холдин", "прибыл", "рубл", "стартап", 'startup',
+                 'الأعمال', '业务', 'negocios', 'affaires',
+                 ],
+    "GOODS": ["wildbe", "вайлд", 'ozon', "озон", 'avito', "авито", "авторск", "одежд", "китай",
+              "китая", "складчина", "подарк", 'модн', 'маркетплейс', 'вещи',
+              'clothes', 'vêtements', 'ropa', '衣服', 'الملابس',
+              'السوق', '市场', 'mercado', 'marketplace',
+              ],
+    "OFFLINE": ["салон", "студи", "логист", "грузопер", 'свечи', "букеты", "клиник",
+                "магазин", "производств", 'эпиляц', 'парикмах', "кондитер",
+                "пищев", 'кулинар', 'оффлайн', 'offline', 'адрес', 'храм', 'церковь', 'транспорт',
+                'temple', 'church',
+                'барбер', 'barber', 'barbero', 'coiffeur', '理发师', 'الحلاق',
+                'salon', 'salón', 'صالون', '沙龙',
+                'недвижимость', 'real estate', 'inmueble', 'immobilier', '房地产', 'العقارات',
+                'shop', 'tienda', 'boutique', '商店', 'تسوق',
+                'كوك', '库克', 'cuisinier', 'gastrónomo',
+                'ресторан', 'restaurant', 'restaurant', 'restaurante', '食肆', 'مطعم',
+                ],
+    "HEALTH": ["beautifull", "beauty", "бьюти", "красота", "здоров", 'нутрициолог', 'косметик', 'косметол', 'йога',
+               'питани', 'доктор', 'диет', 'похуден', 'волос', 'маникюр', 'макияж', 'клиник', 'ресниц', 'эпиляц',
+               'парикмах', 'nutrition', 'krasota', 'zdorov', 'dietol', 'медицин', 'medic', 'стоматол',
+               'врач', 'vrach', 'yoga', 'фитнес', 'fitnes', 'медиц', 'медик', 'лекарств', 'спортив', 'sport',
+               'семья', 'дети', 'ребенок',
+               'health', 'الصحة', '健康', 'salud', 'santé',
+               'beauté', 'belleza', '美貌', 'الجمال',
+               'medicine', '医学', 'الطب', 'medicina', 'médecine',
+               ],
+}
+l_hashtag_translate = {
+    "BLOG": {
+        'ru': "#блогер",
+        'en': "#blogger",
+        'es': "#blogger",
+        'fr': "#blogueur",
+        'zh': "#博客作者",
+        'ar': "#مدون",
+    },
+    "DIGIT": {
+        'ru': "#оцифровка",
+        'en': "#digit",
+        'es': "#digitalización",
+        'fr': "#numérisation",
+        'zh': "#数字化",
+        'ar': "#الرقمنة",
+    },
+    "SMM": {
+        'ru': "#смм",
+        'en': "#smm",
+        'es': "#blogger",
+        'fr': "#blogger",
+        'zh': "#blogger",
+        'ar': "#سم",
+    },
+    "RECRUIT": {
+        'ru': "#рекрут",
+        'en': "#recruit",
+        'es': "#recluta",
+        'fr': "#recruter",
+        'zh': "#招聘人员",
+        'ar': "#تجنيد",
+    },
+    "DESIGN": {
+        'ru': "#дизайн",
+        'en': "#design",
+        'es': "#diseño",
+        'fr': "#conception",
+        'zh': "#设计",
+        'ar': "#التصميم",
+    },
+    "COACH": {
+        'ru': "#коуч",
+        'en': "#coach",
+        'es': "#entrenador",
+        'fr': "#entraîneur",
+        'zh': "#教练",
+        'ar': "#مدرب",
+    },
+    "IT": {
+        'ru': "#ИТ",
+        'en': "#IT",
+        'es': "#IT",
+        'fr': "#IT",
+        'zh': "#信息技术",
+        'ar': "#تقانةالمعلومات",
+    },
+    "BUSINESS": {
+        'ru': "#бизнес",
+        'en': "#business",
+        'es': "#negocios",
+        'fr': "#affaires",
+        'zh': "#业务",
+        'ar': "#الأعمال",
+    },
+    "GOODS": {
+        'ru': "#товарка",
+        'en': "#products",
+        'es': "#mercancía",
+        'fr': "#articles",
+        'zh': "#产品中心",
+        'ar': "#المنتجات",
+    },
+    "OFFLINE": {
+        'ru': "#оффлайн",
+        'en': "#offline",
+        'es': "#fueradelínea",
+        'fr': "#horsligne",
+        'zh': "#离线状态",
+        'ar': "#غيرمتصل",
+    },
+    "HEALTH": {
+        'ru': "#здоровье",
+        'en': "#health",
+        'es': "#blogger",
+        'fr': "#blogger",
+        'zh': "#blogger",
+        'ar': "#blogger",
+    },
+    "ISVERIFIED": {
+        'ru': "#верифиц",
+        'en': "#verified",
+        'es': "#verificado",
+        'fr': "#vérifié",
+        'zh': "#已核实",
+        'ar': "#التحقق",
+    },
+    "ISPREMIUM": {
+        'ru': "#премиум",
+        'en': "#premium",
+        'es': "#prima",
+        'fr': "#prime",
+        'zh': "#保费",
+        'ar': "#قسط",
+    },
 }
 
-l_cnotification_dialog_on = {
-    'ru': "✅☑Вкл диалог",
-    'en': "✅☑Dialogue included",
-    'es': "✅☑Diálogo incluido",
-    'fr': "✅☑Dialogue inclus",
-    'zh': "✅☑包括对话",
-    'ar': "✅☑ متضمن الحوار",
+l_find_alert = {
+    'ru': "👩🏽‍💻 <b>Жми</b> на ✅/☑️, чтобы вкл/выкл <i>уведомления</i> о появлении отслеживаемых слов в публичных группах/каналах\n\n🔔 <b>Отслеживаемые</b>  слова: <code>{0}</code>\n🔔 <b>Отслеживаемые</b> группы/каналы: <code>{1}</code>",
+    'en': "👩🏽‍💻 <b>Click</b> on ✅/☑️ to turn on/off <i>notifications</i> about Telegram customers in freelance groups/channels\n\n🔔 For example, <i>#ищу</i> <i>an assistant to maintain a Telegram channel or</i> <i>#search</i> <i>a telegram bot developer</i>",
+    'es': "👩🏽‍💻 <b>Haz clic</b> en ✅/☑️ para activar/desactivar <i>las notificaciones</i> sobre los clientes de Telegram en grupos/canales independientes\n\n🔔 Por ejemplo, <i>#ищу</i> <i>un asistente para mantener un canal de Telegram o</i> <i>#search</i> <i>un desarrollador de bots de Telegram</i>",
+    'fr': "👩🏽‍💻 <b>Cliquez</b> sur ✅/☑️ pour activer/désactiver <i>les notifications</i> concernant les clients Telegram dans les groupes/canaux indépendants\n\n🔔 Par exemple, <i>#ищу</i> <i>un assistant pour gérer un canal Telegram ou</i> <i>#search</i> <i>un développeur de bot Telegram</i>",
+    'zh': "👩🏽‍💻<b>点击</b>✅/☑️ 开启/关闭自由群组/频道中有关 Telegram 客户的<i>通知</i>\n\n🔔 例如， <i>#ищу维护</i><i> Telegram 频道的助手或#search一个 telegram 机器人开发者</i>",
+    'ar': "👩🏽‍💻 <b>انقر</b> فوق ✅ / ☑️ لتشغيل / إيقاف تشغيل <i>الإشعارات</i> حول عملاء Telegram في مجموعات / قنوات مستقلة\n\n🔔 على سبيل المثال ، <i>#ищу</i> <i>مساعد للحفاظ على قناة Telegram أو</i> <i>#search</i> <i>مطور برامج Telegram bot</i>",
 }
-l_cnotification_dialog_off = {
-    'ru': "☑️☐Выкл диалог",
-    'en': "☑️☐Disable dialogue",
-    'es': "☑️☐Desactivar diálogo",
-    'fr': "☑️☐Désactiver les dialogues",
-    'zh': "☑️☐禁用对话",
-    'ar': "☑️☐ تعطيل الحوار",
+l_find_alert_alert = {
+    'ru': "🔔 Нет отслеживаемых слов/групп/каналов\nЖми ⚙️Настроить",
+    'en': "🪄 The footer is empty, you need to set it up ⚙️",
+    'es': "🪄 El pie de página está vacío, debes configurarlo ⚙️",
+    'fr': "🪄 Le pied de page est vide, vous devez le paramétrer ⚙️",
+    'zh': "🪄 footer 是空的，需要设置一下⚙️",
+    'ar': "🪄 التذييل فارغ ، تحتاج إلى إعداده ⚙️",
 }
-l_cnotification_all_on = {
-    'ru': "✅☑Вкл все действия",
-    'en': "✅☑Including all actions",
-    'es': "✅☑Incluyendo todas las acciones",
-    'fr': "✅☑Incluant toutes les actions",
-    'zh': "✅☑包括所有动作",
-    'ar': "✅☑ بما في ذلك جميع الإجراءات",
+l_find_alert_words = {
+    'ru': "👩🏽‍💻 <b>Вставь</b> отслеживаемые слова (более <u>3</u> символов) через <i>пробельные или разделительные</i> символы (без подписки: <u>1</u> слово)\n▪️регистр не важен\n▪️* в конце слова учитывает вхождение\n\n👩🏽‍💻 <b>Например</b>, для <b>психо*</b> отслеживание сработает на фразы: <i>анти<u>психо</u>лог, <u>Психо</u>терапевт..</i>\n🔔 <b>Отслеживаемые</b>  слова: <code>{0}</code>\n🔔 <b>Отслеживаемые</b> группы/каналы: <code>{1}</code>",
+    'en': "👩🏽‍💻 <b>Enter</b> recipient Ids separated by spaces or separator characters",
+    'es': "👩🏽‍💻 <b>Ingrese</b> las identificaciones de los destinatarios separadas por espacios o caracteres separadores",
+    'fr': "👩🏽‍💻 <b>Entrez</b> les identifiants des destinataires séparés par des espaces ou des caractères de séparation",
+    'zh': "👩🏽‍💻<b>输入</b>以空格或分隔符分隔的收件人 ID",
+    'ar': "👩🏽‍💻 <b>أدخل</b> معرفات المستلمين مفصولة بمسافات أو أحرف فاصلة",
 }
-l_cnotification_all_off = {
-    'ru': "☑️☐Выкл все действия",
-    'en': "☑️☐Off all actions",
-    'es': "☑️☐Desactivar todas las acciones",
-    'fr': "☑️☐Désactiver toutes les actions",
-    'zh': "☑️☐关闭所有操作",
-    'ar': "☑️☐ إيقاف جميع الإجراءات",
+l_find_alert_sources = {
+    'ru': "👩🏽‍💻 <b>Вставь</b> публичные ссылки на группы/каналы (для отслеживаемых слов) через <i>пробельные или разделительные</i> символы (без подписки: <u>5</u> групп/каналов)\n\n🔔 <b>Отслеживаемые</b>  слова: <code>{0}</code>\n🔔 <b>Отслеживаемые</b> группы/каналы: <code>{1}</code>",
+    'en': "👩🏽‍💻 <b>Enter</b> recipient Ids separated by spaces or separator characters",
+    'es': "👩🏽‍💻 <b>Ingrese</b> las identificaciones de los destinatarios separadas por espacios o caracteres separadores",
+    'fr': "👩🏽‍💻 <b>Entrez</b> les identifiants des destinataires séparés par des espaces ou des caractères de séparation",
+    'zh': "👩🏽‍💻<b>输入</b>以空格或分隔符分隔的收件人 ID",
+    'ar': "👩🏽‍💻 <b>أدخل</b> معرفات المستلمين مفصولة بمسافات أو أحرف فاصلة",
 }
-
-l_cnotification_dialog = {
-    'ru': "💬 <b>Пользователь</b>: {0} [<b>id</b>={1}] написал в @{2}-боте:",
-    'en': "💬 <b>User</b> : {0} [<b>id</b> = {1}] wrote in @{2}-bot:",
-    'es': "💬 <b>Usuario</b> : {0} [<b>id</b> = {1}] escribió en @{2}-bot:",
-    'fr': "💬 <b>Utilisateur</b> : {0} [<b>id</b> = {1}] a écrit dans @{2}-bot :",
-    'zh': "💬<b>用户</b>：{0} [<b>id</b> = {1}] 在@{2}-bot 中写道：",
-    'ar': "💬 <b>المستخدم</b> : {0} [<b>id</b> = {1}] كتب في @ {2} -bot:",
+l_find_need_subscribe = {
+    'ru': "👩🏽‍💻 <b>Для</b> получения ссылки на сообщение и заказчика оформи подписку на @FereyFindBot-бота:\n\nhttps://t.me",
+    'en': "👩🏽‍💻 <b>To</b> get a link to the message and the customer, subscribe to @FereyFindBot -bot:\n\nhttps://t.me",
+    'es': "👩🏽‍💻 <b>Para</b> obtener un enlace al mensaje y al cliente, suscríbete a @FereyFindBot -bot:\n\nhttps://t.me",
+    'fr': "👩🏽‍💻 <b>Pour</b> obtenir un lien vers le message et le client, abonnez-vous à @FereyFindBot -bot :\n\nhttps://t.me",
+    'zh': "👩🏽‍💻<b>要</b>获取消息和客户的链接，请订阅@FereyFindBot -bot：\n\nhttps://t.me",
+    'ar': "👩🏽‍💻 <b>للحصول</b> على ارتباط للرسالة والعميل ، اشترك في @FereyFindBot -bot:\n\nhttps: //t.me",
 }
 # endregion
 
 
-# region cuser_
-l_cuser_text2 = {
-    'ru': "👥 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> <i>замену голосовых/телескопов на <b>audio/video</b> (*рекомендуется, если premium-пользователи установили такой запрет)/сервисные <b>статусы</b> бота (печатает..записывает видео..)/ведение списка <b>/utm-рефералов</b></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse - вывести всех пользователей\n/utm - вывести utm-рефералов\n/link - создать реферальную /utm ссылку",
-    'en': "👥 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> <i>the replacement of voice/telescopes with <b>audio/video</b> (*recommended if</i> premium <i>users have set such a ban)/bot service <b>statuses</b> (prints..records video..)/maintaining a list of <b>/utm referrals</b></i>\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/parse - display all users\n/utm - display utm referrals\n/link - create a referral /utm link",
-    'es': "👥 <b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> <i>el reemplazo de voz/telescopios con <b>audio/video</b> (*recomendado si</i> los usuarios premium <i>han establecido dicha prohibición)/ <b>estados</b> de servicio de bot (imprime... graba video...)/mantiene una lista de <b>/utm referencias</b></i>\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/parse - mostrar todos los usuarios\n/utm - mostrar referencias utm\n/link - crear un enlace de referencia /utm",
-    'fr': "👥 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>le remplacement de la voix/des télescopes par <b>l&#x27;audio/la vidéo</b> (*recommandé si</i> les utilisateurs premium <i>ont défini une telle interdiction)/ <b>les statuts</b> du service de bot (imprime..enregistre la vidéo..)/maintient une liste de <b>/références utm</b></i>\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/parse - afficher tous les utilisateurs\n/utm - afficher les références utm\n/lien - créer une référence /lien utm",
-    'zh': "👥<b>点击</b>✅/☑️<b>启用/禁用</b><i>用音频<b>/视频</b>替换语音/望远镜（*如果</i>premium<i>用户设置了此类禁令，则推荐）/机器人服务<b>状态</b>（打印..记录视频..）/维护列表<b>/utm referrals</b></i>\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/parse - 显示所有用户\n/utm - 显示 utm referrals\n/link - 创建一个推荐 /utm 链接",
-    'ar': "👥 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <i>استبدال الصوت / التلسكوبات بالصوت <b>/ الفيديو</b> (* يوصى به إذا</i> قام المستخدمون premium <i>بتعيين مثل هذا الحظر) / <b>حالات</b> خدمة الروبوت (طباعة .. تسجيلات فيديو ..) / الاحتفاظ بقائمة من <b>إحالات / utm</b></i>\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - كافة الأوامر\n/ parse - عرض كافة المستخدمين\n/ utm - عرض إحالات utm\n/ link - إنشاء ارتباط إحالة / utm",
+# region FereyMediaBot
+l_media_btn1 = {
+    'ru': "⛰️ Медиа",
+    'en': "⛰️ Media",
+    'es': "⛰️ Medios",
+    'fr': "⛰️ Médias",
+    'zh': "⛰️ 媒体",
+    'ar': "⛰️ ميديا",
 }
-l_cuser_restricted_on = {
-    'ru': "✅☑Вкл audio/video замена",
-    'en': "✅☑Includes audio/video replacement",
-    'es': "✅☑Incluye reemplazo de audio/video",
-    'fr': "✅☑Comprend le remplacement audio/vidéo",
-    'zh': "✅☑包括音频/视频替换",
-    'ar': "✅☑ يشمل استبدال الصوت / الفيديو",
+l_media_btn2 = {
+    'ru': "🌬 Подписка",
+    'en': "🌬 Subscription",
+    'es': "🌬 Suscripción",
+    'fr': "🌬 Abonnement",
+    'zh': "🌬订阅",
+    'ar': "🌬 الاشتراك",
 }
-l_cuser_restricted_off = {
-    'ru': "☑️☐Выкл audio/video замена",
-    'en': "☑️☐Off audio/video replacement",
-    'es': "☑️☐Reemplazo de audio/video apagado",
-    'fr': "☑️☐Off remplacement audio/vidéo",
-    'zh': "☑️☐关闭音频/视频替换",
-    'ar': "☑️☐ إيقاف استبدال الصوت / الفيديو",
+l_media_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> медиа-заметок:\n\n▪️<b>стикеры</b> из текста и фото\n▪️<b>аудио-тренды</b>\n▪️<b>видео-заметки</b>\n▪️инлайн-<b>телескопы</b>\n▪️<b>кнопочные</b> премиум-заметки\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <i>the landing bot of</i> медиа notes:\n\n▪️ <b>stickers</b> from text and photos\n▪️ <b>audio sounds</b>\n▪️ <b>video notes</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido <i>al bot de aterrizaje de</i> notas медиа :\n\n▪️ <b>pegatinas</b> de texto y fotos\n▪️ <b>sonidos de audio</b>\n▪️ <b>notas de video</b>\n\n❗️ también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue dans <i>le bot de débarquement des</i> notes медиа :\n\n▪️ <b>autocollants</b> à partir de textes et de photos\n▪️ <b>sons audio</b>\n▪️ <b>notes vidéo</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎来到медиа笔记<i>的登陆机器人</i>：\n\n▪️文字和照片的<b>贴纸</b>\n▪️<b>音频声音</b>\n▪️<b>视频笔记</b>\n\n❗️您也可以在我们的Ferey工作室",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الأساسي</i> لملاحظات медиа :\n\n▪️ <b>ملصقات</b> من النصوص والصور\n▪️ <b>الأصوات الصوتية</b>\n▪️ <b>ملاحظات الفيديو</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت الدردشة في استوديو Ferey الخاص بنا",
 }
-l_cuser_status_on = {
-    'ru': "✅☑Вкл сервисные статусы",
-    'en': "✅☑On service statuses",
-    'es': "✅☑Sobre estados de servicio",
-    'fr': "✅☑Sur les états de service",
-    'zh': "✅☑关于服务状态",
-    'ar': "✅☑على حالات الخدمة",
+l_subscribe_media = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>кнопочные</b> премиум-заметки\n(<i>динамические медиа</i>)\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
-l_cuser_status_off = {
-    'ru': "☑️☐Выкл сервисные статусы",
-    'en': "☑️☐Off service statuses",
-    'es': "☑️☐Estados de servicio desactivados",
-    'fr': "☑️☐Hors statuts de service",
-    'zh': "☑️☐关闭服务状态",
-    'ar': "☑️☐ إيقاف حالات الخدمة",
+
+l_media_text = {
+    'ru': "👩🏽‍💻 <b>Здесь</b> можно выбрать тип выпадающих media-заметок (/add | /del)",
+    'en': "👩🏽‍💻 <b>Here</b> you can select the type of drop-down media notes (/add | /del)",
+    'es': "👩🏽‍💻 <b>Aquí</b> puede seleccionar el tipo de notas multimedia desplegables (/add | /del)",
+    'fr': "👩🏽‍💻 <b>Ici,</b> vous pouvez sélectionner le type de notes multimédia déroulantes (/add | /del)",
+    'zh': "👩🏽‍💻<b>在这里</b>可以选择下拉媒体备注的类型（/add | /del）",
+    'ar': "👩🏽‍💻 <b>هنا</b> يمكنك تحديد نوع ملاحظات الوسائط المنسدلة (/ إضافة | / ديل)",
 }
-l_cuser_utm_on = {
-    'ru': "✅☑Вкл utm-рефералы",
-    'en': "✅☑On utm referrals",
-    'es': "✅☑Sobre referencias utm",
-    'fr': "✅☑Sur les références utm",
-    'zh': "✅☑关于 utm 推荐",
-    'ar': "✅☑On الإحالات UTM",
+l_media_del = {
+    'ru': "👩🏽‍💻 <b>Выбери</b> media-заметку для удаления",
+    'en': "👩🏽‍💻 <b>Select</b> media note to delete",
+    'es': "👩🏽‍💻 <b>Seleccione</b> la nota multimedia para eliminar",
+    'fr': "👩🏽‍💻 <b>Sélectionnez</b> la note multimédia à supprimer",
+    'zh': "👩🏽‍💻<b>选择</b>要删除的媒体备注",
+    'ar': "<b>حدد</b> ملاحظة وسائط لحذفها",
 }
-l_cuser_utm_off = {
-    'ru': "☑️☐Выкл utm-рефералы",
-    'en': "☑️☐Off utm referrals",
-    'es': "☑️☐Off referencias utm",
-    'fr': "☑️☐Hors références utm",
-    'zh': "☑️☐关闭utm推荐",
-    'ar': "☑️☐ Off إحالات UTM",
+l_media_show = {
+    'ru': "👩🏽‍💻 <b>Введи</b> текст для поиска по media-заметкам",
+    'en': "👩🏽‍💻 <b>Enter</b> text to search media notes",
+    'es': "👩🏽‍💻 <b>Ingrese</b> texto para buscar notas multimedia",
+    'fr': "👩🏽‍💻 <b>Entrez</b> du texte pour rechercher des notes multimédias",
+    'zh': "👩🏽‍💻<b>输入</b>文字搜索媒体笔记",
+    'ar': "👩🏽‍💻 <b>أدخل</b> نصًا للبحث في ملاحظات الوسائط",
 }
-l_bot_is_off = {
-    'ru': "👩🏽‍💻 <b>@{0}-бот</b> выключен\n\n/on - включить бот",
-    'en': "👩🏽‍💻 <b>@{0}-bot</b> off\n\n/on - enable bot",
-    'es': "👩🏽‍💻 <b>@{0}-bot</b> apagado\n\n/encendido - habilitar bot",
-    'fr': "👩🏽‍💻 <b>@{0}-bot</b> off\n\n/on - activer le bot",
-    'zh': "👩🏽‍💻 <b>@{0}-bot</b> off\n\n/on - 启用机器人",
-    'ar': "👩🏽‍💻 <b>@ {0} -bot</b> off\n\n/ on - قم بتمكين الروبوت",
+l_media_random = {
+    'ru': "🎲 <b>Случайный</b> выбор",
+    'en': "🎲 <b>Random</b> selection",
+    'es': "🎲 Selección <b>aleatoria</b>",
+    'fr': "🎲 Sélection <b>aléatoire</b>",
+    'zh': "🎲<b>随机</b>选择",
+    'ar': "🎲 اختيار <b>عشوائي</b>",
 }
-l_cuser_utm = {
-    'ru': "👥 <b>Готово!</b> <b>/utm-список</b> реферальных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Вывести</b> рефералов конкретного пользователя можно командой:\n/utm id или /utm @username\n\n👩🏽‍💻 <b>Текущее</b> число utm-рефералов: <u>{1}</u>",
-    'en': "👥 <b>Done!</b> <b>/utm-list</b> of referral users of @{0}-bot\n\n👩🏽‍💻 You can <b>display</b> referrals of a specific user with the command:\n/utm id or /utm @username\n\n👩🏽‍💻 <b>Current</b> number of utm-referrals : <u>{1}</u>",
-    'es': "👥 <b>Listo!</b> <b>/utm-lista</b> de usuarios de referencia de @{0}-bot\n\n👩🏽‍💻 Puede <b>mostrar</b> referencias de un usuario específico con el comando:\n/utm id o /utm @username\n\n👩🏽 ‍💻 Número <b>actual</b> de referencias utm: <u>{1}</u>",
-    'fr': "👥 <b>C&#x27;est fait !</b> <b>/utm-list</b> des utilisateurs référents de @{0}-bot\n\n👩🏽‍💻 Vous pouvez <b>afficher</b> les références d&#x27;un utilisateur spécifique avec la commande :\n/utm id ou /utm @username\n\n👩🏽 ‍💻 Nombre <b>actuel</b> de références utm : <u>{1}</u>",
-    'zh': "👥<b>完成！</b> <b>/utm-@{0}-bot 的推荐用户列表</b>\n\n👩🏽‍💻 您可以使用以下命令<b>显示</b>特定用户的推荐：\n/utm id或/utm @username\n\n👩🏽 ‍💻<b>当前</b>的 utm-referrals 数量： <u>{1}</u>",
-    'ar': "👥 <b>انتهى!</b> <b>/ utm-list</b> لمستخدمي الإحالة لـ @ {0} -bot\n\n👩🏽‍💻 يمكنك <b>عرض</b> إحالات مستخدم معين بالأمر:\n/utm id أو /utm @username\n\n👩🏽 ‍💻 العدد <b>الحالي</b> لإحالات UTM: <u>{1}</u>",
+l_media_none = {
+    'ru': "👩🏽‍💻 <b>Media</b>-заметок не найдено",
+    'en': "👩🏽‍💻 <b>Media</b> - no notes found",
+    'es': "👩🏽‍💻 <b>Medios</b> : no se encontraron notas",
+    'fr': "👩🏽‍💻 <b>Médias</b> - aucune note trouvée",
+    'zh': "👩🏽‍💻<b>媒体</b>- 未找到笔记",
+    'ar': "👩🏽‍💻 <b>وسائط</b> - لم يتم العثور على ملاحظات",
 }
-l_cuser_link_done = {
-    'ru': "👥 <b>Готово!</b> Реферальная /utm ссылка на @{0}-бота (размести ее на любой площадке, чтобы понимать, что пользователи перешли в бота с этой площадки):\n\n{1}",
-    'en': "👥 <b>Done!</b> Referral /utm link to the @{0}-bot (place it on any site to understand that users have switched to the bot from this site):\n\n{1}",
-    'es': "👥 <b>Listo!</b> Enlace de referencia /utm al @{0}-bot (colóquelo en cualquier sitio para comprender que los usuarios han cambiado al bot desde este sitio):\n\n{1}",
-    'fr': "👥 <b>C&#x27;est fait !</b> Lien de parrainage /utm vers le @{0}-bot (placez-le sur n&#x27;importe quel site pour comprendre que les utilisateurs sont passés au bot depuis ce site) :\n\n{1}",
-    'zh': "👥<b>完成！</b> @{0}-bot 的引荐 /utm 链接（将其放在任何站点上以了解用户已从该站点切换到该 bot）：\n\n{1}",
-    'ar': "👥 <b>انتهى!</b> رابط الإحالة / utm إلى @ {0} -bot (ضعه على أي موقع لفهم أن المستخدمين قد تحولوا إلى الروبوت من هذا الموقع):\n\n{1}",
+l_media_file = {
+    'ru': "👩🏽‍💻 1/2. <b>Прикрепи</b> audio/video, text/photo контент для создания media-заметки",
+    'en': "👩🏽‍💻 1/2. <b>Attach</b> audio/video, text/photo content to create a media note",
+    'es': "👩🏽‍💻 1/2. <b>Adjunte</b> contenido de audio/video, texto/foto para crear una nota multimedia",
+    'fr': "👩🏽‍💻 1/2. <b>Joignez</b> du contenu audio/vidéo, texte/photo pour créer une note multimédia",
+    'zh': "👩🏽‍💻 1/2。<b>附加</b>音频/视频、文本/照片内容以创建媒体说明",
+    'ar': "👩🏽‍💻 1/2. <b>قم بإرفاق</b> محتوى صوت / فيديو ونص / صورة لإنشاء ملاحظة وسائط",
 }
-l_cuser_link_start = {
-    'ru': "👥 <b>Придумай</b> название для /utm ссылки (*после ?start= может быть <u>любое</u> имя источника из цифр и/или латинских букв)\n\n👩🏽‍💻 <b>Например</b>, ссылки /utm-рефералов для отслеживания:\nhttps://t.me/{0}?start={1} - <i>реферальных пользователей</i> {1}-<i>пользователя</i>\nhttps://t.me/{0}?start=instagram - <i>пользователей из instagram</i>",
-    'en': "👥 <b>Think of</b> a name for the /utm link (*after ?start= there can be <u>any</u> source name from numbers and/or Latin letters)\n\n👩🏽‍💻 <b>For example</b> , /utm referral links for tracking:\nhttps://t .me/{0}?start={1} - <i>referral users</i> {1} - <i>user</i>\nhttps://t.me/{0}?start=instagram - <i>users from instagram</i>",
-    'es': "👥 <b>Piense en</b> un nombre para el enlace /utm (*después de ?start= puede haber <u>cualquier</u> nombre de fuente de números y/o letras latinas)\n\n👩🏽‍💻 <b>Por ejemplo</b> , enlaces de referencia /utm para el seguimiento:\nhttps ://t .me/{0}?start={1} - <i>usuarios de referencia</i> {1} - <i>usuario</i>\nhttps://t.me/{0}?start=instagram - <i>usuarios de instagram</i>",
-    'fr': "👥 <b>Pensez à</b> un nom pour le lien /utm (*après ?start= il peut y avoir <u>n&#x27;importe quel</u> nom de source à partir de chiffres et/ou de lettres latines)\n\n👩🏽‍💻 <b>Par exemple</b> , les liens de référence /utm pour le suivi :\nhttps ://t .me/{0}?start={1} - <i>utilisateurs de référence</i> {1} - <i>utilisateur</i>\nhttps://t.me/{0}?start=instagram - <i>utilisateurs d&#x27;instagram</i>",
-    'zh': "👥<b>为 /utm 链接想</b>一个名字（*在?start=之后可以有<u>任何</u>来自数字和/或拉丁字母的源名称）\n\n👩🏽‍💻<b>例如</b>，用于跟踪的 /utm 推荐链接：\nhttps ://t .me/{0}?start={1} -<i>推荐用户</i>{1} -<i>用户</i>\nhttps://t.me/{0}?start=instagram -<i>来自 instagram 的用户</i>",
-    'ar': "👥 <b>فكر في</b> اسم ارتباط / utm (* after ?start= يمكن أن يكون هناك <u>أي</u> اسم مصدر من الأرقام و / أو الأحرف اللاتينية)\n\n👩🏽‍💻 <b>على سبيل المثال</b> ، روابط الإحالة / utm للتتبع:\nhttps : // t .me / {0}؟ start = {1} - <i>المستخدمون المحالون</i> {1} - <i>المستخدم</i>\nhttps: //t.me/ {0}؟ start = instagram - <i>المستخدمون من instagram</i>",
+l_media_title1 = {
+    'ru': "👩🏽‍💻 2/2. <b>Введи</b> ключевые_слова для твоей media-заметки\n[изменить ключевые_слова нельзя]",
+    'en': "👩🏽‍💻 2/2. <b>Enter</b> ключевые_слова for your media note\n[ключевые_слова cannot be changed]",
+    'es': "👩🏽‍💻 2/2. <b>Ingrese</b> ключевые_слова para su nota de prensa\n[ключевые_слова no se pueden cambiar]",
+    'fr': "👩🏽‍💻 2/2. <b>Saisissez</b> ключевые_слова pour votre note média\n[ключевые_слова ne peuvent pas être modifiés]",
+    'zh': "👩🏽‍💻 2/2。为您的媒体说明<b>输入</b>ключевые_слова\n[无法更改ключевые_слова]",
+    'ar': "👩🏽‍💻 2/2. <b>أدخل</b> ключевые_слова لملاحظتك الإعلامية\n[لا يمكن تغيير ключевые_слова]",
 }
-l_promo_done = {
-    'ru': "👩🏽‍💻 <b>Готово!</b>\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n{0}\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n/promo 0",
-    'en': "👩🏽‍💻 <b>Done!</b>\n\n👩🏽‍💻 <i>Current /promo code</i> :\n{0}\n👩🏽‍💻 <i>Delete /promo code</i> :\n/promo 0",
-    'es': "👩🏽‍💻 <b>Listo!</b>\n\n👩🏽‍💻 <i>Código /promocional actual</i> :\n{0}\n👩🏽‍💻 <i>Eliminar código /promocional</i> :\n/promo 0",
-    'fr': "👩🏽‍💻 <b>C&#x27;est fait !</b>\n\n👩🏽‍💻 <i>Code /promo actuel</i> :\n{0}\n👩🏽‍💻 <i>Supprimer le code /promo</i> :\n/promo 0",
-    'zh': "👩🏽‍💻<b>完成！</b>\n\n👩🏽‍💻<i>当前/促销代码</i>：\n{0}\n👩🏽‍💻<i>删除/促销代码</i>：\n/promo 0",
-    'ar': "👩🏽‍💻 <b>انتهى!</b>\n\n👩🏽‍💻 <i>الرمز الحالي / الترويجي</i> :\n{0}\n👩🏽‍💻 <i>حذف / الرمز الترويجي</i> :\n/promo 0",
+l_media_title2 = {
+    'ru': "👩🏽‍💻 2/2. <b>Текущие</b> ключевые_слова для твоей media-заметки\n\n{0}\n\n[пришли новые или нажми {1}]",
+    'en': "👩🏽‍💻 2/2. <b>Current</b> ключевые_слова for your media note\n\n{0}\n\n[new ones come in or press {1}]",
+    'es': "👩🏽‍💻 2/2. ключевые_слова <b>actuales</b> para su nota de prensa\n\n{0}\n\n[nuevas ingrese o presione {1}]",
+    'fr': "👩🏽‍💻 2/2. ключевые_слова <b>actuels</b> pour votre note multimédia\n\n{0}\n\n[les nouveaux arrivent ou appuyez sur {1}]",
+    'zh': "👩🏽‍💻 2/2。您的媒体说明的<b>当前</b>ключевые_слова\n\n{0}\n\n[请输入新关键字或按 {1}]",
+    'ar': "👩🏽‍💻 2/2. ключевые_слова <b>الحالية</b> لملاحظة الوسائط الخاصة بك\n\n{0}\n\n[يتم إدخال كلمات رئيسية جديدة أو الضغط على {1}]",
 }
-l_promo_start = {
-    'ru': "👩🏽‍💻 <b>Введи</b> /promo-код для @{0}-бота:\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n{1}\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n/promo 0",
-    'en': "👩🏽‍💻 <b>Enter</b> /promo code for @{0}-bot:\n\n👩🏽‍💻 <i>Current /promo code</i> :\n{1}\n👩🏽‍💻 <i>Delete /promo code</i> :\n/promo 0",
-    'es': "👩🏽‍💻 <b>Ingresa el</b> /código de promoción para @{0}-bot:\n\n👩🏽‍💻 <i>Actual /código de promoción</i> :\n{1}\n👩🏽‍💻 <i>Eliminar /código de promoción</i> :\n/promo 0",
-    'fr': "👩🏽‍💻 <b>Entrez</b> /code promo pour @{0}-bot :\n\n👩🏽‍💻 <i>Code /code promo actuel</i> :\n{1}\n👩🏽‍💻 <i>Supprimer /code promo</i> :\n/promo 0",
-    'zh': "👩🏽‍💻<b>输入</b>@{0}-bot 的 /promo 代码：\n\n👩🏽‍💻<i>当前 /promo 代码</i>：\n{1}\n👩🏽‍💻<i>删除 /promo 代码</i>：\n/promo 0",
-    'ar': "👩🏽‍💻 <b>أدخل</b> / الرمز الترويجي لـ @ {0} -bot:\n\n👩🏽‍💻 <i>الرمز الحالي / الترويجي</i> :\n{1}\n👩🏽‍💻 <i>حذف / الرمز الترويجي</i> :\n/promo 0",
+l_media_confirm = {
+    'ru': "🏁 Завершить",
+    'en': "🏁 Complete",
+    'es': "🏁 Completa",
+    'fr': "🏁 Complet",
+    'zh': "🏁 完成",
+    'ar': "🏁 مكتمل",
 }
-# endregion
-
-
-# region cadmin_
-l_cadmin_text2 = {
-    'ru': "👮🏽 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> <i>доступ добавленных администраторов к функционалу <b>[💬 Оповещения]</b></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей",
-    'en': "👮🏽 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> <i>access of added administrators to functionality <b>[💬 Notifications]</b></i>\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/admin - add/remove administrator\n/parse - display all users",
-    'es': "👮🏽 <b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> <i>el acceso de los administradores agregados a la funcionalidad <b>[💬 Notificaciones]</b></i>\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/admin - agregar/eliminar administrador\n/ analizar - mostrar todos los usuarios",
-    'fr': "👮🏽 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>l&#x27;accès des administrateurs ajoutés à la fonctionnalité <b>[💬 Notifications]</b></i>\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/admin - ajouter/supprimer un administrateur\n/ parse - affiche tous les utilisateurs",
-    'zh': "👮🏽<b>单击</b>✅/☑️<b>启用/禁用</b><i>添加的管理员对功能的访问<b>[💬 通知]</b></i>\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/admin - 添加/删除管理员\n/ parse - 显示所有用户",
-    'ar': "👮🏽 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <i>وصول المسؤولين المضافين إلى الوظائف <b>[💬 إعلامات]</b></i>\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - كافة الأوامر\n/ admin - إضافة / إزالة المسؤول\n/ تحليل - عرض جميع المستخدمين",
+l_media_error = {
+    'ru': "👩🏽‍💻 <b>Ошибка</b> (попробуй позже или загрузи другое media)",
+    'en': "👩🏽‍💻 <b>Error</b> (try later or upload another media)",
+    'es': "👩🏽‍💻 <b>Error</b> (intenta más tarde o sube otro medio)",
+    'fr': "👩🏽‍💻 <b>Erreur</b> (essayez plus tard ou téléchargez un autre média)",
+    'zh': "👩🏽‍💻<b>错误</b>（稍后再试或上传其他媒体）",
+    'ar': "👩🏽‍💻 <b>خطأ</b> (حاول لاحقًا أو قم بتحميل وسائط أخرى)",
 }
-l_cadmin_done = {
-    'ru': "👮🏽 <b>Готово!</b>/admin-список @{0}-бота:\n\n{1}\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{2}/10</u>",
-    'en': "👮🏽 <b>Done!</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/admin - add/remove administrator\n/parse - display all users\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{2}/10</u>",
-    'es': "👮🏽 <b>Listo!</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/admin - agregar/eliminar administrador\n/parse - mostrar todos los usuarios\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{2}/10</u>",
-    'fr': "👮🏽 <b>C&#x27;est fait !</b> /admin-list @{0}-bot :\n\n{1}\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/admin - ajouter/supprimer un administrateur\n/parse - afficher tous les utilisateurs\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{2}/10</u>",
-    'zh': "👮🏽<b>完成！</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/admin - 添加/删除管理员\n/parse - 显示所有用户\n\n👩🏽‍💻<b>当前</b>管理员人数： <u>{2}/10</u>",
-    'ar': "👮🏽 <b>انتهى!</b> / admin-list @ {0} -bot:\n\n{1}\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - جميع الأوامر\n/ admin - إضافة / إزالة المسؤول\n/ parse - عرض جميع المستخدمين\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{2} / 10</u>",
+l_media_finish = {
+    'ru': "👩🏽‍💻 <b>Media</b>-заметка успешно создана",
+    'en': "👩🏽‍💻 <b>Media</b> - note created successfully",
+    'es': "👩🏽‍💻 <b>Medios</b> : nota creada con éxito",
+    'fr': "👩🏽‍💻 <b>Média</b> - note créée avec succès",
+    'zh': "👩🏽‍💻<b>媒体</b>- 笔记创建成功",
+    'ar': "👩🏽‍💻 <b>الوسائط</b> - تم إنشاء الملاحظة بنجاح",
 }
-l_cadmin_add = {
-    'ru': "👮🏽 <b>Введи</b> до 10 id-пользователей через пробельные символы или разделители, чтобы добавить их в /admin-список\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{0}</u>",
-    'en': "👮🏽 <b>Enter</b> user id separated by spaces or separators to add them to /admin-list\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{0}</u>",
-    'es': "👮🏽 <b>Ingrese</b> id de usuario separados por espacios o separadores para agregarlos a /admin-list\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{0}</u>",
-    'fr': "👮🏽 <b>Entrez</b> id des utilisateurs séparés par des espaces ou des séparateurs pour les ajouter à /admin-list\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{0}</u>",
-    'zh': "👮🏽<b>输入</b>以空格或分隔符分隔的用户id ，以将其添加到 /admin-list\n\n👩🏽‍💻<b>当前</b>管理员人数： <u>{0}</u>",
-    'ar': "👮🏽 <b>أدخل</b> id المستخدمين مفصولة بمسافات أو فواصل لإضافتها إلى / قائمة المشرف\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{0}</u>",
+l_media_publish = {
+    'ru': "🔗 Список",
+    'en': "🔗 List",
+    'es': "🔗 Lista",
+    'fr': "🔗 Liste",
+    'zh': "🔗 清单",
+    'ar': "🔗 قائمة",
 }
-l_cadmin_remove = {
-    'ru': "👮🏽 <b>Введи</b> id пользователей через пробельные символы или разделители, чтобы удалить их из /admin-список\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{0}</u>",
-    'en': "👮🏽 <b>Enter</b> user id separated by spaces or separators to remove them from /admin-list\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{0}</u>",
-    'es': "👮🏽 <b>Ingrese</b> id de usuario separados por espacios o separadores para eliminarlos de /admin-list\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{0}</u>",
-    'fr': "👮🏽 <b>Entrez</b> id d&#x27;utilisateur séparés par des espaces ou des séparateurs pour les supprimer de /admin-list\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{0}</u>",
-    'zh': "👮🏽<b>输入</b>以空格或分隔符分隔的用户id ，以将其从 /admin-list 中删除\n\n👩🏽‍💻<b>当前</b>管理员数量： <u>{0}</u>",
-    'ar': "👮🏽 <b>أدخل</b> id المستخدمين مفصولة بمسافات أو فواصل لإزالتها من / قائمة المشرف\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{0}</u>",
+l_media_check = {
+    'ru': "🔗 Проверка",
+    'en': "🔗 Check",
+    'es': "🔗 Comprobar",
+    'fr': "🔗 Vérifier",
+    'zh': "🔗 检查",
+    'ar': "🔗 تحقق",
 }
-l_parse_text = {
-    'ru': "👩🏽‍💻 <b>Готово!</b> Парсинг пользователей (<u>{0}</u>) @{1}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse - вывести всех пользователей\n/parse premium - вывести premium-пользователей\n/parse admin - вывести admin-пользователей\n/parse utm - вывести utm-рефералов\n",
-    'en': "👩🏽‍💻 <b>Done!</b> Parsing users ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/parse - print all users\n/parse premium - print premium users\n/parse admin - display admin users\n/parse utm - display utm referrals\n",
-    'es': "👩🏽‍💻 <b>Listo!</b> Analizando usuarios ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/parse - imprimir todos los usuarios\n/parse premium - imprimir usuarios premium\n/parse admin - mostrar usuarios administradores\n/parse utm - mostrar referencias utm\n",
-    'fr': "👩🏽‍💻 <b>C&#x27;est fait !</b> Analyse des utilisateurs ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/parse - imprimer tous les utilisateurs\n/parse premium - imprimer les utilisateurs premium\n/parse admin - affiche les utilisateurs administrateurs\n/parse utm - affiche les références utm\n",
-    'zh': "👩🏽‍💻<b>完成！</b>解析用户（ <u>{0}</u> ）@{1}-bot\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/parse - 打印所有用户\n/parse premium - 打印高级用户\n/parse admin - 显示管理员用户\n/parse utm - 显示 utm 引用\n",
-    'ar': "👩🏽‍💻 <b>انتهى!</b> تحليل المستخدمين ( <u>{0}</u> ) @ {1} -bot\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - جميع الأوامر\n/ تحليل - طباعة جميع المستخدمين\n/parse premium - طباعة المستخدمين المتميزين\n/parse admin - عرض المستخدمين المسؤولين\n/parse utm - عرض إحالات UTM\n",
+l_media_hasdeleted = {
+    'ru': "👩🏽‍💻 <b>Media</b>-заметка удалена",
+    'en': "👩🏽‍💻 <b>Media</b> - note deleted",
+    'es': "👩🏽‍💻 <b>Medios</b> - nota eliminada",
+    'fr': "👩🏽‍💻 <b>Médias</b> - note supprimée",
+    'zh': "👩🏽‍💻<b>媒体</b>- 注释已删除",
+    'ar': "👩🏽‍💻 <b>الوسائط</b> - تم حذف الملاحظة",
+}
+l_media_delprepare = {
+    'ru': "🔗 Выбрать",
+    'en': "🔗 Choose",
+    'es': "🔗 Elige",
+    'fr': "🔗 Choisissez",
+    'zh': "🔗选择",
+    'ar': "🔗 اختر",
 }
-# endregion
 # endregion
 
 
-# region client
-l_idea = {
-    'ru': "💡 Идея!",
-    'en': "💡 Idea!",
-    'es': "💡 Idea!",
-    'fr': "💡 Idée !",
-    'zh': "💡 想法！",
-    'ar': "💡 فكرة!",
+# region FereyPostBot
+l_post_btn1 = {
+    'ru': "⛰️ Посты",
+    'en': "⛰️ Posts",
+    'es': "⛰️ Publicaciones",
+    'fr': "⛰️ Messages",
+    'zh': "⛰️ 帖子",
+    'ar': "⛰️ المشاركات",
 }
-l_have_read = {
-    'ru': "👩🏽‍💻 {0} прочитал сообщение",
-    'en': "👩🏽‍💻 {0} read the message",
-    'es': "👩🏽‍💻 {0} lee el mensaje",
-    'fr': "👩🏽‍💻 {0} lire le message",
-    'zh': "👩🏽‍💻 {0}阅读消息",
-    'ar': "👩🏽‍💻 {0} اقرأ الرسالة",
+l_post_btn2 = {
+    'ru': "🌬 Подписка",
+    'en': "🌬 Subscription",
+    'es': "🌬 Suscripción",
+    'fr': "🌬 Abonnement",
+    'zh': "🌬订阅",
+    'ar': "🌬 الاشتراك",
 }
-l_telegraph_title = {
-    'ru': "📰 Telegraph блог",
-    'en': "📰 Telegraph Blog",
-    'es': "📰Blog de telégrafo",
-    'fr': "📰 Blog télégraphique",
-    'zh': "📰 电报博客",
-    'ar': "📰 مدونة التلغراف",
+l_post_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для создания креативных постов <b>Ferey</b>\n▪️инлайн-<b>телескопы</b>\n▪️<b>уведомления</b> о нажатиях\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <i>the landing bot</i> for creating creative постов <b>Ferey</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> para crear постов creativas <b>Ferey</b>\n\n❗️también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> pour créer постов créatifs <b>Ferey</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎使用<b>Ferey</b>创建创意постов的<i>登陆机器人</i>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> لإنشاء постов إبداعية <b>Ferey</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
-l_telegraph_blog = {
-    'ru': "<figure><img src='{0}'/><figcaption>Фото профиля: @{1}</figcaption></figure><blockquote>Лэндинг-блог для продвижения в <i>Telegram</i></blockquote>👩🏽‍💻 <b>бот:</b> {2}<br>[<b>id</b>={3}]<br><b>Био:</b> {4}<br><aside>Описание</aside>{5}",
-    'en': "Profile photo: @{1}Landing blog for promotion in <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = {3}] <b>Bio:</b> {4}Description{5}",
-    'es': "Foto de perfil: @{1}Blog de aterrizaje para promoción en <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = {3}] <b>Bio:</b> {4}Descripción{5}",
-    'fr': "Photo de profil : @{1}Blog d'atterrissage pour la promotion dans <i>Telegram</i> 👩🏽‍💻 <b>bot :</b> {2}[<b>id</b> = {3}] <b>Bio :</b> {4}Description{5}",
-    'zh': "个人资料照片：@{1}登陆博客以在<i>Telegram</i> 👩🏽‍💻<b>机器人中进行推广：</b> {2}[<b>id</b> = {3}]<b>简介：</b> {4}说明{5}",
-    'ar': "صورة الملف الشخصي: @ {1} مدونة الهبوط للترويج في <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2} [<b>id</b> = {3}] <b>السيرة الذاتية:</b> {4} الوصف {5}",
+l_subscribe_post = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>нотис</b>-уведомления о нажатиях\n(<i>ссылка на пользователя</i>)\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
+
+l_post_bot_button_push = {
+    'ru': "👩🏽‍💻 <b>Пользователь</b>: {0} нажал на: [{1}] (пост #<u>{2}</u>)",
+    'en': "👩🏽‍💻 <b>Пользователь</b>: {name} нажал на: [{button}] (пост #<u>{post_id}</u>)",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 # endregion
 
 
-# region extra bot
-l_show_admin_panel_md = {
-    'ru': "*👩🏽‍💻 Создание и редактирование блога*\n\n👩🏽‍💻 Вы зашли как *Администратор* и можете создавать и редактировать блоги, но не удалять их\n\n¹ Авторизация по ссылке в браузере:\n`{0}`\n\n² Перейди (в течение 10сек) по нужной ссылке для редактирования публикации (жми, чтобы скопировать):\n\n",
-    'en': "*👩🏽‍💻 Creating and editing a blog*\n\n👩🏽‍💻 You are logged in as *Administrator* and can create and edit blogs, but not delete them\n\n¹ Authorization via link in browser:\n`{0 }`\n\n² Go (within 10 seconds) to the desired link to edit the post (click to copy):\n\n",
-    'es': "*👩🏽‍💻 Crear y editar un blog*\n\n👩🏽‍💻 Ha iniciado sesión como *Administrador* y puede crear y editar blogs, pero no eliminarlos\n\n¹ Autorización a través de un enlace en el navegador:\n`{0 }`\n\n² Vaya (dentro de 10 segundos) al enlace deseado para editar la publicación (haga clic para copiar):\n\n",
-    'fr': "*👩🏽‍💻 Créer et modifier un blog*\n\n👩🏽‍💻 Vous êtes connecté en tant qu'*administrateur* et vous pouvez créer et modifier des blogs, mais pas les supprimer\n\n¹ Autorisation via un lien dans le navigateur :\n`{0 }`\n\n² Accédez (dans les 10 secondes) au lien souhaité pour modifier le message (cliquez pour copier) :\n\n",
-    'zh': "*👩🏽‍💻 创建和编辑博客*\n\n👩🏽‍💻 您以*管理员*身份登录，可以创建和编辑博客，但不能删除它们\n\n¹ 通过浏览器中的链接授权：\n`{0 }`\n\n²（在 10 秒内）转到所需的链接以编辑帖子（单击以复制）：\n\n",
-    'ar': "* 👩🏽‍💻 إنشاء مدونة وتحريرها *\n\n👩🏽‍💻 تم تسجيل دخولك بصفتك * المسؤول * ويمكنك إنشاء المدونات وتحريرها ، ولكن لا يمكنك حذفها\n\n¹ التفويض عبر الارتباط في المستعرض:\n'{0}`\n\n² انتقل (في غضون 10 ثوانٍ) إلى الرابط المطلوب لتعديل المشاركة (انقر للنسخ):\n\n",
+# region FereyToolsBot
+l_tools_btn1 = {
+    'ru': "⛰️ Инструменты",
+    'en': "⛰️ Tools",
+    'es': "⛰️ Herramientas",
+    'fr': "⛰️ Outils",
+    'zh': "⛰️ 工具",
+    'ar': "⛰️ أدوات",
 }
-l_show_admin_panel_html = {
-    'ru': "<b>👩🏽‍💻 Создание и редактирование блога</b>\n\n👩🏽‍💻 Вы зашли как <b>Администратор</b> и можете создавать и редактировать блоги, но не удалять их\n\n1. Авторизация по ссылке в браузере:\n{0}\n\n2. Перейди (в течение 10сек) по нужной ссылке для редактирования публикации (жми, чтобы скопировать):\n\n",
-    'en': "<b>👩🏽‍💻 Creating and editing a blog</b>\n\n👩🏽‍💻 You are logged in as <b>Administrator</b> and can create and edit blogs, but not delete them\n\n1. Authorization by link in browser:\n{0}\n\n2. Go (within 10 seconds) to the desired link to edit the publication (click to copy):\n\n",
-    'es': "<b>👩🏽‍💻 Crear y editar un blog</b>\n\n👩🏽‍💻 Ha iniciado sesión como <b>Administrador</b> y puede crear y editar blogs, pero no borrarlos\n\n1. Autorización por enlace en el navegador:\n{0}\n\n2. Vaya (dentro de 10 segundos) al enlace deseado para editar la publicación (haga clic para copiar):\n\n",
-    'fr': "<b>👩🏽‍💻 Créer et modifier un blog</b>\n\n👩🏽‍💻 Vous êtes connecté en tant <b>qu&#x27;administrateur</b> et pouvez créer et modifier des blogs, mais pas les supprimer\n\n1. Autorisation par lien dans le navigateur :\n{0}\n\n2. Accédez (dans les 10 secondes) au lien souhaité pour modifier la publication (cliquez pour copier) :\n\n",
-    'zh': "<b>👩🏽‍💻 创建和编辑博客</b>\n\n👩🏽‍💻 您以<b>管理员</b>身份登录，可以创建和编辑博客，但不能删除它们\n\n1.通过浏览器中的链接授权：\n{0}\n\n2.转到（在 10 秒内）所需的链接以编辑发布（单击以复制）：\n\n",
-    'ar': "<b>👩🏽‍💻 إنشاء مدونة وتحريرها</b>\n\n👩🏽‍💻 قمت بتسجيل الدخول <b>كمسؤول</b> ويمكنك إنشاء المدونات وتحريرها ، ولكن لا يمكنك حذفها\n\n1. التفويض بالارتباط في المتصفح:\n{0}\n\n2. انتقل (في غضون 10 ثوانٍ) إلى الارتباط المطلوب لتحرير المنشور (انقر للنسخ):\n\n",
+l_tools_btn2 = {
+    'ru': "🌬 Подписка",
+    'en': "🌬 Subscription",
+    'es': "🌬 Suscripción",
+    'fr': "🌬 Abonnement",
+    'zh': "🌬订阅",
+    'ar': "🌬 الاشتراك",
 }
-l_show_admin_panel_create = {
-    'ru': "🆕 Создать",
-    'en': "🆕 Create",
-    'es': "🆕 Crear",
-    'fr': "🆕 Créer",
-    'zh': "🆕 创建",
-    'ar': "🆕 خلق",
+l_tools_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> Telegram-инструментов:\n\n▪️<b>преобразование</b> контента\n▪️<b>получение</b> информации о сообщ\n▪️<b>удаление</b> фона\n▪️<b>конвертация</b> в телескопы\n▪️<b>сообщение</b> 0-длины\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <i>the landing bot</i> of Telegram инструментов :\n\n▪️ content <b>conversion</b>\n▪️ <b>getting</b> information about the message\n\n❗️you can also order the development of a chat bot in our studio Ferey",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> de инструментов de Telegram:\n\n▪️ <b>conversión</b> de contenido\n▪️ <b>obtener</b> información sobre el mensaje\n\n❗️también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue dans <i>le landing bot</i> des инструментов Telegram :\n\n▪️ <b>conversion</b> de contenu\n▪️ <b>obtenir</b> des informations sur le message\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎使用 Telegram инструментов的<i>登陆机器人</i>：\n\n▪️ 内容<b>转换</b>\n▪️<b>获取</b>有关消息的信息\n\n❗️您也可以在我们的工作室Ferey订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص инструментов Telegram:\n\n▪️ <b>تحويل</b> المحتوى\n▪️ <b>الحصول على</b> معلومات حول الرسالة\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
-l_show_admin_panel_auth = {
-    'ru': "👩🏽‍💻 Авторизация",
-    'en': "👩🏽‍💻 Authorization",
-    'es': "👩🏽‍💻 Autorización",
-    'fr': "👩🏽‍💻 Autorisation",
-    'zh': "👩🏽‍💻授权",
-    'ar': "👩🏽‍💻 إذن",
+l_subscribe_tools = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
-# endregion
 
-
-# region html
-l_burger_save = {
-    'ru': "Сохранить",
-    'en': "Save",
-    'es': "Ahorrar",
-    'fr': "Sauvegarder",
-    'zh': "节省",
-    'ar': "يحفظ",
+l_image_text = {
+    'ru': "👩🏽‍💻 <b>Выбери</b> инструменты для преобразования <i>изображения</i> в",
+    'en': "👩🏽‍💻 <b>Choose</b> tools to convert <i>your image</i> to",
+    'es': "👩🏽‍💻 <b>Elija</b> herramientas para convertir <i>su imagen</i> a",
+    'fr': "👩🏽‍💻 <b>Choisissez</b> des outils pour convertir <i>votre image</i> en",
+    'zh': "👩🏽‍💻<b>选择</b>将<i>图像</i>转换为的工具",
+    'ar': "👩🏽‍💻 <b>اختر</b> أدوات لتحويل <i>صورتك</i> إلى",
 }
-l_burger_gen = {
-    'ru': "Сгенерировать бота",
-    'en': "Generate bot",
-    'es': "Generar bot",
-    'fr': "Générer un robot",
-    'zh': "生成机器人",
-    'ar': "توليد بوت",
+l_image_sticker = {
+    'ru': "🌌 стикер",
+    'en': "🌌 sticker",
+    'es': "🌌 pegatina",
+    'fr': "🌌 autocollant",
+    'zh': "🌌 贴纸",
+    'ar': "🌌 ملصق",
 }
-l_burger_import = {
-    'ru': "Импортировать .bot",
-    'en': "Import .bot",
-    'es': "Importar .bot",
-    'fr': "Importer .bot",
-    'zh': "导入.bot",
-    'ar': "استيراد .bot",
+l_image_jpg = {
+    'ru': "🏞️ jpg",
+    'en': "🏞️ jpg",
+    'es': "🏞️ jpg",
+    'fr': "🏞️jpg",
+    'zh': "🏞️ jpg",
+    'ar': "🏞️ jpg",
 }
-l_burger_export = {
-    'ru': "Экспортировать как >",
-    'en': "Export as >",
-    'es': "Exportar como >",
-    'fr': "Exporter sous >",
-    'zh': "导出为 >",
-    'ar': "تصدير باسم>",
+l_image_png = {
+    'ru': "🌁 png",
+    'en': "🌁 png",
+    'es': "🌁 png",
+    'fr': "🌁 png",
+    'zh': "🌁 PNG",
+    'ar': "🌁 ينغ",
 }
-l_burger_clear = {
-    'ru': "Очистить",
-    'en': "Cleaning",
-    'es': "Limpieza",
-    'fr': "Nettoyage",
-    'zh': "打扫",
-    'ar': "تنظيف",
+l_image_rbg = {
+    'ru': "🙌🏽 удалить фон",
+    'en': "🙌🏽 remove background",
+    'es': "🙌🏽 eliminar fondo",
+    'fr': "🙌🏽 supprimer l'arrière-plan",
+    'zh': "🙌🏽 删除背景",
+    'ar': "🙌🏽 إزالة الخلفية",
 }
-l_burger_gen_alert = {
-    'ru': "Создать нового бота?",
-    'en': "Create a new bot?",
-    'es': "¿Crear un nuevo bot?",
-    'fr': "Créer un nouveau bot ?",
-    'zh': "创建一个新的机器人？",
-    'ar': "إنشاء روبوت جديد؟",
+l_image_mp4 = {
+    'ru': "🎥 mp4",
+    'en': "🎥 mp4",
+    'es': "🎥 mp4",
+    'fr': "🎥 mp4",
+    'zh': "🎥 mp4",
+    'ar': "🎥 mp4",
 }
-l_burger_import_alert = {
-    'ru': "Загрузка..",
-    'en': "Loading..",
-    'es': "Cargando..",
-    'fr': "Chargement..",
-    'zh': "加载中..",
-    'ar': "تحميل..",
+l_image_album = {
+    'ru': "9️⃣ album⁹",
+    'en': "9️⃣ album⁹",
+    'es': "9️⃣ álbum⁹",
+    'fr': "9️⃣album⁹",
+    'zh': "9️⃣专辑⁹",
+    'ar': "9️⃣ البوم⁹",
 }
-l_burger_clear_alert = {
-    'ru': "Очистить сцену?",
-    'en': "Clear the scene?",
-    'es': "Limpiar la escena?",
-    'fr': "Vider la scène ?",
-    'zh': "清理现场？",
-    'ar': "مسح المشهد؟",
+l_image_thumb = {
+    'ru': "🖼️ thumb",
+    'en': "🖼️ thumb",
+    'es': "🖼️ pulgar",
+    'fr': "🖼️ pouce",
+    'zh': "🖼️拇指",
+    'ar': "🖼️ إبهام",
 }
-
-l_ent_close = {
-    'ru': "Закрыть",
-    'en': "Close",
-    'es': "Cerca",
-    'fr': "Fermer",
-    'zh': "关闭",
-    'ar': "يغلق",
+l_image_descpic = {
+    'ru': "⿴ Bot Desc Pic",
+    'en': "⿴ Bot Desc Pic",
+    'es': "⿴ Foto de descripción del bot",
+    'fr': "⿴ Image de description du robot",
+    'zh': "⿴ 机器人描述图片",
+    'ar': "⿴ بوت ديسك بيك",
 }
-l_ent_save = {
-    'ru': "Сохранить",
-    'en': "Save",
-    'es': "Ahorrar",
-    'fr': "Sauvegarder",
-    'zh': "节省",
-    'ar': "يحفظ",
+l_image_sticker_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в стикер",
+    'en': "👩🏽‍💻 <b>Attach</b> a photo to convert into a sticker",
+    'es': "👩🏽‍💻 <b>Adjunta</b> una foto para convertirla en una pegatina",
+    'fr': "👩🏽‍💻 <b>Joignez</b> une photo à convertir en autocollant",
+    'zh': "👩🏽‍💻<b>附上</b>照片以转换为贴纸",
+    'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى ملصق",
 }
-l_ent_delete = {
-    'ru': "Удалить",
-    'en': "Delete",
-    'es': "Borrar",
-    'fr': "Supprimer",
-    'zh': "删除",
-    'ar': "يمسح",
+l_image_jpg_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в jpg",
+    'en': "👩🏽‍💻 <b>Attach</b> a photo to convert to jpg",
+    'es': "👩🏽‍💻 <b>Adjunta</b> una foto para convertir a jpg",
+    'fr': "👩🏽‍💻 <b>Joindre</b> une photo à convertir en jpg",
+    'zh': "👩🏽‍💻<b>附上</b>照片以转换为jpg",
+    'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى jpg",
 }
-l_copied = {
-    'ru': "Скопировано",
-    'en': "Copied",
-    'es': "Copiado",
-    'fr': "Copié",
-    'zh': "已复制",
-    'ar': "نسخ",
+l_image_png_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в png",
+    'en': "👩🏽‍💻 <b>Attach</b> a photo to convert to png",
+    'es': "👩🏽‍💻 <b>Adjunta</b> una foto para convertir a png",
+    'fr': "👩🏽‍💻 <b>Joindre</b> une photo à convertir en png",
+    'zh': "👩🏽‍💻<b>附上</b>要转换为png的照片",
+    'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى png",
 }
-l_web_gen_img = {
-    'ru': "Сгенерировать Образ",
-    'en': "Generate Image",
-    'es': "Generar imagen",
-    'fr': "Générer une image",
-    'zh': "生成图像",
-    'ar': "توليد الصورة",
+l_image_rbg_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для удаления фона",
+    'en': "👩🏽‍💻 <b>Attach</b> photo to remove background",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> foto para eliminar fondo",
+    'fr': "👩🏽‍💻 <b>Joindre</b> une photo pour supprimer l'arrière-plan",
+    'zh': "👩🏽‍💻<b>附加</b>照片以删除背景",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> صورة لإزالة الخلفية",
 }
-l_web_gen_txt = {
-    'ru': "Сгенерировать Текст",
-    'en': "Generate Text",
-    'es': "Generar Texto",
-    'fr': "Générer du texte",
-    'zh': "生成文本",
-    'ar': "توليد نص",
+l_image_mp4_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в mp4 (Telegram-аватарку)",
+    'en': "👩🏽‍💻 <b>Attach</b> a photo to convert to mp4 (Telegram avatar)",
+    'es': "👩🏽‍💻 <b>Adjunta</b> una foto para convertir a mp4 (Avatar de Telegram)",
+    'fr': "👩🏽‍💻 <b>Joindre</b> une photo à convertir en mp4 (avatar Telegram)",
+    'zh': "👩🏽‍💻<b>附上</b>照片以转换为mp4（电报头像）",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> صورة لتحويلها إلى mp4 (Telegram avatar)",
 }
-l_all_trg = {
-    'ru': ": все триггеры",
-    'en': ": all triggers",
-    'es': ": todos los disparadores",
-    'fr': ": tous les déclencheurs",
-    'zh': ": 所有触发器",
-    'ar': ": جميع المشغلات",
+l_image_album_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в альбом из 9 частей",
+    'en': "👩🏽‍💻 <b>Attach</b> a photo to transform into a 9-part album",
+    'es': "👩🏽‍💻 <b>Adjunta</b> una foto para transformarla en un álbum de 9 partes",
+    'fr': "👩🏽‍💻 <b>Joignez</b> une photo pour la transformer en un album en 9 parties",
+    'zh': "👩🏽‍💻<b>附上</b>照片，变身为9张相册",
+    'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى ألبوم مكون من 9 أجزاء",
 }
-l_one_trg = {
-    'ru': ": 1 триггер",
-    'en': ": 1 trigger",
-    'es': ": 1 gatillo",
-    'fr': ": 1 gâchette",
-    'zh': "：1个触发器",
-    'ar': ": 1 الزناد",
+l_image_thumb_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в thumb-nail-иконку (160x160)",
+    'en': "👩🏽‍💻 <b>Attach</b> a photo to convert to a thumb-nail icon (160x160)",
+    'es': "👩🏽‍💻 <b>Adjunte</b> una foto para convertirla en un icono de miniatura (160x160)",
+    'fr': "👩🏽‍💻 <b>Joignez</b> une photo à convertir en icône de vignette (160x160)",
+    'zh': "👩🏽‍💻<b>附加</b>照片以转换为缩略图图标 (160x160)",
+    'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى رمز مسمار الإبهام (160 × 160)",
 }
-l_actions = {
-    'ru': ": действия",
-    'en': ": actions",
-    'es': ": acciones",
-    'fr': ": Actions",
-    'zh': "：行动",
-    'ar': ": أجراءات",
+l_image_descpic_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> фото для преобразования в формат, необходимый для установки Description Picture для бота в @BotFather (640x360)",
+    'en': "👩🏽‍💻 <b>Attach</b> a photo to convert to the format required to set the Description Picture for the bot in @BotFather (640x360)",
+    'es': "👩🏽‍💻 <b>Adjunte</b> una foto para convertir al formato requerido para configurar la imagen de descripción para el bot en @BotFather (640x360)",
+    'fr': "👩🏽‍💻 <b>Joignez</b> une photo à convertir au format requis pour définir l'image de description du bot dans @BotFather (640x360)",
+    'zh': "👩🏽‍💻<b>附上</b>照片以转换为在@BotFather中为机器人设置描述图片所需的格式（640x360）",
+    'ar': "👩🏽‍💻 <b>أرفق</b> صورة لتحويلها إلى التنسيق المطلوب لتعيين وصف الصورة للروبوت في @BotFather (640x360)",
 }
-l_trigger = {
-    'ru': "Триггер",
-    'en': "Trigger",
-    'es': "Desencadenar",
-    'fr': "Déclencher",
-    'zh': "扳机",
-    'ar': "مشغل",
+
+l_gif_text = {
+    'ru': "👩🏽‍💻 <b>Выбери</b> инструменты для преобразования <i>гиф</i> в",
+    'en': "👩🏽‍💻 <b>Choose</b> tools to convert <i>GIF</i> to",
+    'es': "👩🏽‍💻 <b>Elija</b> herramientas para convertir <i>GIF</i> a",
+    'fr': "👩🏽‍💻 <b>Choisissez</b> des outils pour convertir <i>GIF</i> en",
+    'zh': "👩🏽‍💻<b>选择将</b><i>GIF</i>转换为的工具",
+    'ar': "👩🏽‍💻 <b>اختر</b> أدوات لتحويل <i>GIF</i> إلى",
 }
-l_action = {
-    'ru': "Действие",
-    'en': "Action",
-    'es': "Acción",
-    'fr': "Action",
-    'zh': "行动",
-    'ar': "فعل",
+l_gif_mp4 = {
+    'ru': "🎥 mp4",
+    'en': "🎥 mp4",
+    'es': "🎥 mp4",
+    'fr': "🎥 mp4",
+    'zh': "🎥 mp4",
+    'ar': "🎥 mp4",
 }
-l_message = {
-    'ru': "Сообщение",
-    'en': "Message",
-    'es': "Mensaje",
-    'fr': "Message",
-    'zh': "信息",
-    'ar': "رسالة",
+l_gif_thumb = {
+    'ru': "🖼️ thumb-nail",
+    'en': "🖼️ thumb-nail",
+    'es': "🖼️ miniatura",
+    'fr': "🖼️ ongle du pouce",
+    'zh': "🖼️ 缩略图",
+    'ar': "🖼️ الإبهام",
+}
+l_gif_descgif = {
+    'ru': "⿴ Bot Desc Gif",
+    'en': "⿴ Bottom Desc Gif",
+    'es': "⿴ Gif de descripción inferior",
+    'fr': "⿴ Bas Desc Gif",
+    'zh': "⿴ 底部描述 Gif",
+    'ar': "⿴ أسفل Desc Gif",
+}
+l_gif_mp4_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> гиф для преобразования в mp4",
+    'en': "👩🏽‍💻 <b>Attach</b> GIF to convert to mp4",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> GIF para convertir a mp4",
+    'fr': "👩🏽‍💻 <b>Joindre</b> GIF pour convertir en mp4",
+    'zh': "👩🏽‍💻<b>附加</b>GIF 以转换为 mp4",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> GIF للتحويل إلى mp4",
+}
+l_gif_thumb_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> гиф для преобразования в thumb-nail-иконку (160x160)",
+    'en': "👩🏽‍💻 <b>Attach</b> GIF to convert to thumb-nail icon (160x160)",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> GIF para convertir en icono de miniatura (160x160)",
+    'fr': "👩🏽‍💻 <b>Attachez</b> GIF pour convertir en icône de vignette (160x160)",
+    'zh': "👩🏽‍💻<b>附加</b>GIF 以转换为缩略图图标 (160x160)",
+    'ar': "👩🏽‍💻 <b>أرفق</b> ملف GIF للتحويل إلى أيقونة مسمار الإبهام (160 × 160)",
+}
+l_gif_descgif_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> гиф для преобразования в формат, необходимый для установки Description Gif для бота в @BotFather (640x360). После формирования GIF нажимаем на нее через <u>мобильное</u> приложение (ожидая загрузки), далее Поделиться - приложение Telegram - @BotFather",
+    'en': "👩🏽‍💻 <b>Attach</b> a gif to convert to the format needed to set the Description Gif for the bot to @BotFather (640x360). After generating a GIF, click on it through <u>the mobile</u> application (waiting for download), then Share - Telegram application - @BotFather",
+    'es': "👩🏽‍💻 <b>Adjunte</b> un gif para convertir al formato necesario para configurar el GIF de descripción para el bot en @BotFather (640x360). Después de generar un GIF, haga clic en él a través de <u>la aplicación móvil</u> (en espera de descarga), luego Compartir - Aplicación Telegram - @BotFather",
+    'fr': "👩🏽‍💻 <b>Joignez</b> un gif à convertir au format nécessaire pour définir le gif de description du bot sur @BotFather (640x360). Après avoir généré un GIF, cliquez dessus via <u>l&#x27;application mobile</u> (en attente de téléchargement), puis Partager - Application Telegram - @BotFather",
+    'zh': "👩🏽‍💻<b>附加</b>一个 gif 以转换为将机器人的描述 Gif 设置为@BotFather (640x360) 所需的格式。生成GIF后，通过<u>手机</u>应用点击（等待下载），然后Share - Telegram application - @BotFather",
+    'ar': "👩🏽‍💻 <b>أرفق</b> صورة gif للتحويل إلى التنسيق المطلوب لتعيين Description Gif للبوت إلى @BotFather (640x360). بعد إنشاء ملف GIF ، اضغط عليه من خلال تطبيق <u>الهاتف المحمول</u> (في انتظار التنزيل) ، ثم شارك - تطبيق Telegram @BotFather",
 }
 
-l_trg_add = {
-    'ru': "+ Добавить Триггер",
-    'en': "+ Add Trigger",
-    'es': "+ Agregar disparador",
-    'fr': "+ Ajouter un déclencheur",
-    'zh': "+ 添加触发器",
-    'ar': "+ إضافة مشغل",
+l_video_text = {
+    'ru': "👩🏽‍💻 <b>Выбери</b> инструменты для преобразования <i>видео</i> в",
+    'en': "👩🏽‍💻 <b>Choose</b> tools to convert <i>video</i> to",
+    'es': "👩🏽‍💻 <b>Elija</b> herramientas para convertir <i>videos</i> a",
+    'fr': "👩🏽‍💻 <b>Choisissez</b> des outils pour convertir <i>la vidéo</i> en",
+    'zh': "👩🏽‍💻<b>选择将</b><i>视频</i>转换为的工具",
+    'ar': "👩🏽‍💻 <b>اختر</b> أدوات لتحويل <i>الفيديو</i> إلى",
 }
-l_trg_cmd = {
-    'ru': "+ команда",
-    'en': "+ command",
-    'es': "+ comando",
-    'fr': "+ commande",
-    'zh': "+ 命令",
-    'ar': "+ الأمر",
+l_video_videonote = {
+    'ru': "⚫️ телескоп",
+    'en': "⚫️ telescope",
+    'es': "⚫️ telescopio",
+    'fr': "⚫️ télescope",
+    'zh': "⚫️望远镜",
+    'ar': "⚫️ تلسكوب",
 }
-l_trg_txt = {
-    'ru': "+ текст",
-    'en': "+ text",
-    'es': "+ texto",
-    'fr': "+ texte",
-    'zh': "+ 文字",
-    'ar': "+ نص",
+l_video_mp3 = {
+    'ru': "▶️ mp3",
+    'en': "▶️ mp3",
+    'es': "▶️ mp3",
+    'fr': "▶️ mp3",
+    'zh': "▶️ mp3",
+    'ar': "▶️ mp3",
 }
-l_trg_btn = {
-    'ru': "+ кнопка",
-    'en': "+ button",
-    'es': "+ botón",
-    'fr': "+ bouton",
-    'zh': "+ 按钮",
-    'ar': "+ زر",
+l_video_mp4 = {
+    'ru': "🎥 mp4",
+    'en': "🎥 mp4",
+    'es': "🎥 mp4",
+    'fr': "🎥 mp4",
+    'zh': "🎥 mp4",
+    'ar': "🎥 mp4",
 }
-l_trg_var = {
-    'ru': "+ переменная",
-    'en': "+ variable",
-    'es': "+ variables",
-    'fr': "+ variable",
-    'zh': "+ 变量",
-    'ar': "+ متغير",
+l_video_album = {
+    'ru': "9️⃣ album⁹",
+    'en': "9️⃣ album⁹",
+    'es': "9️⃣ álbum⁹",
+    'fr': "9️⃣album⁹",
+    'zh': "9️⃣专辑⁹",
+    'ar': "9️⃣ البوم⁹",
 }
-l_trg_lst = {
-    'ru': "+ список",
-    'en': "+ list",
-    'es': "+ lista",
-    'fr': "+ liste",
-    'zh': "+ 列表",
-    'ar': "+ قائمة",
+l_video_thumb = {
+    'ru': "🖼️ thumb-nail",
+    'en': "🖼️ thumb-nail",
+    'es': "🖼️ miniatura",
+    'fr': "🖼️ ongle du pouce",
+    'zh': "🖼️ 缩略图",
+    'ar': "🖼️ الإبهام",
+}
+l_video_gif = {
+    'ru': "📽️ gif",
+    'en': "📽️ gif",
+    'es': "📽️ gif",
+    'fr': "📽️ gif",
+    'zh': "📽️动图",
+    'ar': "📽️ gif",
+}
+l_video_transcribe = {
+    'ru': "🗣️ транскрибация",
+    'en': "🗣️ transcription",
+    'es': "🗣️ transcripción",
+    'fr': "🗣️ retranscription",
+    'zh': "🗣️ 转录",
+    'ar': "🗣️ النسخ",
+}
+l_video_videonote_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> видео для преобразования в телескоп (круглую видео-заметку)",
+    'en': "👩🏽‍💻 <b>Attach</b> a video to transform into a telescope (round video note)",
+    'es': "👩🏽‍💻 <b>Adjunta</b> un video para transformarte en telescopio (nota de video redonda)",
+    'fr': "👩🏽‍💻 <b>Joindre</b> une vidéo pour se transformer en télescope (note vidéo ronde)",
+    'zh': "👩🏽‍💻<b>附上</b>变身望远镜的视频（圆形视频笔记）",
+    'ar': "<b>أرفق</b> مقطع فيديو لتحويله إلى تلسكوب (ملاحظة فيديو مستديرة)",
+}
+l_video_mp3_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> видео для преобразования в mp3-аудио",
+    'en': "👩🏽‍💻 <b>Attach</b> video to convert to mp3 audio",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> video para convertir a audio mp3",
+    'fr': "👩🏽‍💻 <b>Joindre</b> une vidéo pour la convertir en audio mp3",
+    'zh': "👩🏽‍💻<b>附加</b>视频以转换为 mp3 音频",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> الفيديو لتحويله إلى صوت mp3",
+}
+l_video_mp4_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> видео для преобразования в mp4",
+    'en': "👩🏽‍💻 <b>Attach</b> video to convert to mp4",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> video para convertir a mp4",
+    'fr': "👩🏽‍💻 <b>Joindre</b> une vidéo à convertir en mp4",
+    'zh': "👩🏽‍💻<b>附上</b>视频以转换为mp4",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> الفيديو لتحويله إلى mp4",
+}
+l_video_album_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> видео для преобразования в альбом из 9 частей",
+    'en': "👩🏽‍💻 <b>Attach</b> video to convert into 9 part album",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> video para convertir en álbum de 9 partes",
+    'fr': "👩🏽‍💻 <b>Joindre</b> une vidéo à convertir en album en 9 parties",
+    'zh': "👩🏽‍💻<b>附上</b>视频以转换成 9 部分专辑",
+    'ar': "👩🏽‍💻 <b>أرفق مقطع</b> فيديو لتحويله إلى ألبوم مكون من 9 أجزاء",
+}
+l_video_thumb_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> видео для преобразования в thumb-nail-иконку (160x160)",
+    'en': "👩🏽‍💻 <b>Attach</b> video to convert to thumbnail (160x160)",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> video para convertirlo en miniatura (160x160)",
+    'fr': "👩🏽‍💻 <b>Joindre</b> une vidéo à convertir en vignette (160x160)",
+    'zh': "👩🏽‍💻<b>附加</b>视频以转换为缩略图 (160x160)",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> فيديو للتحويل إلى صورة مصغرة (160 × 160)",
+}
+l_video_gif_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> видео для преобразования в гиф",
+    'en': "👩🏽‍💻 <b>Attach</b> video to convert to GIF",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> video para convertir a GIF",
+    'fr': "👩🏽‍💻 <b>Joindre</b> une vidéo à convertir en GIF",
+    'zh': "👩🏽‍💻<b>附加</b>视频以转换为 GIF",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> الفيديو لتحويله إلى GIF",
+}
+l_video_transcribe_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> круглую видео для преобразования в текст",
+    'en': "👩🏽‍💻 <b>Attach</b> round video to convert to text",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> video redondo para convertir a texto",
+    'fr': "👩🏽‍💻 <b>Attachez</b> une vidéo ronde pour la convertir en texte",
+    'zh': "👩🏽‍💻<b>附上</b>圆形视频以转换为文本",
+    'ar': "👩🏽‍💻 <b>أرفق</b> مقطع فيديو مستديرًا للتحويل إلى نص",
 }
 
-l_act_add = {
-    'ru': "+ Добавить Действие",
-    'en': "+ Add Action",
-    'es': "+ Agregar acción",
-    'fr': "+ Ajouter une action",
-    'zh': "+ 添加动作",
-    'ar': "+ إضافة عمل",
+l_audio_text = {
+    'ru': "👩🏽‍💻 <b>Выбери</b> инструменты для преобразования <i>audio</i> в",
+    'en': "👩🏽‍💻 <b>Choose</b> tools to convert <i>audio</i> to",
+    'es': "👩🏽‍💻 <b>Elija</b> herramientas para convertir <i>audio</i> a",
+    'fr': "👩🏽‍💻 <b>Choisissez</b> des outils pour convertir <i>l&#x27;audio</i> en",
+    'zh': "👩🏽‍💻<b>选择</b>将<i>音频</i>转换为的工具",
+    'ar': "👩🏽‍💻 <b>اختر</b> أدوات لتحويل <i>الصوت</i> إلى",
 }
-l_act_dly = {
-    'ru': "+ задержка",
-    'en': "+ delay",
-    'es': "+ retraso",
-    'fr': "+ délai",
-    'zh': "+延迟",
-    'ar': "+ تأخير",
+l_audio_mp3 = {
+    'ru': "▶️ mp3-аудио",
+    'en': "▶️ mp3-audio",
+    'es': "▶️ audio mp3",
+    'fr': "▶️ audio mp3",
+    'zh': "▶️ mp3音频",
+    'ar': "▶ ️ mp3 الصوت",
 }
-l_act_wait = {
-    'ru': "+ ожидание",
-    'en': "+ waiting",
-    'es': "+ esperando",
-    'fr': "+ attente",
-    'zh': "+ 等待",
-    'ar': "+ الانتظار",
+l_audio_ogg = {
+    'ru': "🎤 ogg-голосовое",
+    'en': "🎤 ogg-voice",
+    'es': "🎤 voz ogg",
+    'fr': "🎤 ogg-voix",
+    'zh': "🎤 ogg 声音",
+    'ar': "🎤 ogg-voice",
 }
-l_act_req = {
-    'ru': "+ запрос",
-    'en': "+ request",
-    'es': "+ solicitud",
-    'fr': "+ demande",
-    'zh': "+ 要求",
-    'ar': "+ طلب",
+l_audio_transcribe = {
+    'ru': "🗣️ транскрибация",
+    'en': "🗣️ transcription",
+    'es': "🗣️ transcripción",
+    'fr': "🗣️ retranscription",
+    'zh': "🗣️ 转录",
+    'ar': "🗣️ النسخ",
+}
+l_audio_mp3_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> голосовое для преобразования в mp3",
+    'en': "👩🏽‍💻 <b>Attach</b> voice to convert to mp3",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> voz para convertir a mp3",
+    'fr': "👩🏽‍💻 <b>Joindre</b> la voix pour convertir en mp3",
+    'zh': "👩🏽‍💻<b>附上</b>语音转换成mp3",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> الصوت للتحويل إلى mp3",
+}
+l_audio_ogg_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> audio для преобразования в голосовое",
+    'en': "👩🏽‍💻 <b>Attach</b> audio to convert to voice",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> audio para convertir a voz",
+    'fr': "👩🏽‍💻 <b>Attachez</b> l'audio pour convertir en voix",
+    'zh': "👩🏽‍💻<b>附加</b>音频以转换为语音",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> الصوت لتحويله إلى صوت",
+}
+l_audio_transcribe_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> голосовое для преобразования в текст",
+    'en': "👩🏽‍💻 <b>Attach</b> voice to convert to text",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> voz para convertir a texto",
+    'fr': "👩🏽‍💻 <b>Attachez</b> la voix pour convertir en texte",
+    'zh': "👩🏽‍💻<b>附加</b>语音以转换为文本",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> صوت لتحويله إلى نص",
+}
+l_audio_recognize = {
+    'ru': "👩🏽‍💻 <b>Ошибка</b> распознавания речи",
+    'en': "👩🏽‍💻 Speech Recognition <b>Error</b>",
+    'es': "👩🏽‍💻 <b>Error</b> de reconocimiento de voz",
+    'fr': "👩🏽‍💻 <b>Erreur</b> de reconnaissance vocale",
+    'zh': "👩🏽‍💻语音识别<b>错误</b>",
+    'ar': "👩🏽‍💻 <b>خطأ</b> في التعرف على الكلام",
 }
 
-l_msg_text = {
-    'ru': ": text",
-    'en': ": text",
-    'es': ": texto",
-    'fr': ": texte",
-    'zh': "： 文本",
-    'ar': ": نص",
+l_text_text = {
+    'ru': "👩🏽‍💻 <b>Выбери</b> инструменты для преобразования <i>текста</i> в",
+    'en': "👩🏽‍💻 <b>Choose</b> tools to convert <i>text</i> to",
+    'es': "👩🏽‍💻 <b>Elija</b> herramientas para convertir <i>texto</i> a",
+    'fr': "👩🏽‍💻 <b>Choisissez</b> des outils pour convertir du <i>texte</i> en",
+    'zh': "👩🏽‍💻<b>选择</b>将<i>文本</i>转换为的工具",
+    'ar': "👩🏽‍💻 <b>اختر</b> أدوات لتحويل <i>النص</i> إلى",
 }
-l_msg_photo = {
-    'ru': ": фото",
-    'en': ": photo",
-    'es': ": foto",
-    'fr': ": photo",
-    'zh': "： 照片",
-    'ar': ": صورة",
+l_text_bin = {
+    'ru': "🔢 bin",
+    'en': "🔢 bin",
+    'es': "🔢 papelera",
+    'fr': "🔢 bin",
+    'zh': "🔢 垃圾桶",
+    'ar': "🔢 بن",
 }
-l_msg_gif = {
-    'ru': ": гиф",
-    'en': ": gif",
-    'es': ": gif",
-    'fr': ": gif",
-    'zh': ": 动图",
-    'ar': ": gif",
+l_text_hex = {
+    'ru': "🔠 hex",
+    'en': "🔠 hex",
+    'es': "🔠 maleficio",
+    'fr': "🔠 hexagone",
+    'zh': "🔠十六进制",
+    'ar': "🔠 عرافة",
 }
-l_msg_video = {
-    'ru': ": видео",
-    'en': ": video",
-    'es': ": video",
-    'fr': ": vidéo",
-    'zh': "： 视频",
-    'ar': ": فيديو",
+l_text_null = {
+    'ru': "0️⃣ null",
+    'en': "0️⃣ null",
+    'es': "0️⃣ nulo",
+    'fr': "0️⃣ nul",
+    'zh': "0️⃣ 无",
+    'ar': "0️⃣ لاغية",
 }
-l_msg_video_note = {
-    'ru': ": телескоп",
-    'en': ": telescope",
-    'es': ": telescopio",
-    'fr': ": télescope",
-    'zh': ": 望远镜",
-    'ar': ": تلسكوب",
+l_text_mp3 = {
+    'ru': "▶️ mp3-аудио",
+    'en': "▶️ mp3-audio",
+    'es': "▶️ audio mp3",
+    'fr': "▶️ audio mp3",
+    'zh': "▶️ mp3音频",
+    'ar': "▶ ️ mp3 الصوت",
 }
-l_msg_audio = {
-    'ru': ": аудио",
-    'en': ": audio",
-    'es': ": sonido",
-    'fr': ": l'audio",
-    'zh': "： 声音的",
-    'ar': ": صوتي",
+l_text_url = {
+    'ru': "️🧾 url-encode",
+    'en': "️🧾 url-encode",
+    'es': "️🧾 codificación de URL",
+    'fr': "️🧾 url-encoder",
+    'zh': "️🧾 网址编码",
+    'ar': "️🧾 عنوان url ترميز",
 }
-l_msg_voice = {
-    'ru': ": голосовое",
-    'en': ": voice",
-    'es': ": voz",
-    'fr': ": voix",
-    'zh': "： 嗓音",
-    'ar': ": صوت",
+l_text_bin_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> текст для преобразования в бинарный вид",
+    'en': "👩🏽‍💻 <b>Attach</b> text to convert to binary",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> texto para convertir a binario",
+    'fr': "👩🏽‍💻 <b>Joindre</b> du texte à convertir en binaire",
+    'zh': "👩🏽‍💻<b>附加</b>文本以转换为二进制",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> نص لتحويله إلى ثنائي",
 }
-l_msg_document = {
-    'ru': ": документ",
-    'en': ": document",
-    'es': ": documento",
-    'fr': ": document",
-    'zh': "： 文档",
-    'ar': ": وثيقة",
+l_text_hex_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> текст для преобразования в hex-символы",
+    'en': "👩🏽‍💻 <b>Attach</b> text to convert to hex characters",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> texto para convertir a caracteres hexadecimales",
+    'fr': "👩🏽‍💻 <b>Joindre</b> du texte à convertir en caractères hexadécimaux",
+    'zh': "👩🏽‍💻<b>附加</b>文本以转换为十六进制字符",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> نص لتحويله إلى أحرف سداسية عشرية",
 }
-l_msg_sticker = {
-    'ru': ": стикер",
-    'en': ": sticker",
-    'es': ": pegatina",
-    'fr': ": autocollant",
-    'zh': "： 贴纸",
-    'ar': ": ملصق",
+l_text_mp3_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> текст для преобразования в голосовое",
+    'en': "👩🏽‍💻 <b>Attach</b> text to convert to voice",
+    'es': "👩🏽‍💻 <b>Adjuntar</b> texto para convertir a voz",
+    'fr': "👩🏽‍💻 <b>Joindre</b> du texte à convertir en voix",
+    'zh': "👩🏽‍💻<b>附加</b>文本以转换为语音",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> نص لتحويله إلى صوت",
 }
-l_msg_quiz = {
-    'ru': ": опрос",
-    'en': ": survey",
-    'es': ": encuesta",
-    'fr': ": enquête",
-    'zh': "： 民意调查",
-    'ar': ": استطلاع",
+l_text_url_attach = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> текст для url-encode-преобразования",
+    'en': "👩🏽‍💻 <b>Attach</b> text for url-encode conversion",
+    'es': "👩🏽‍💻 <b>Adjunte</b> texto para la conversión de codificación URL",
+    'fr': "👩🏽‍💻 <b>Joindre</b> du texte pour la conversion en url-encode",
+    'zh': "👩🏽‍💻<b>附加</b>文本进行 url-encode 转换",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> نص لتحويل ترميز url",
 }
-l_msg_dice = {
-    'ru': ": игра",
-    'en': ": game",
-    'es': ": juego",
-    'fr': ": jeu",
-    'zh': "： 游戏",
-    'ar': ": لعبة",
+l_text_text1024 = {
+    'ru': "💭 Текст 1024 символа",
+    'en': "💭 Text 1024 characters",
+    'es': "💭 Texto 1024 caracteres",
+    'fr': "💭 Texte 1024 caractères",
+    'zh': "💭 文本 1024 个字符",
+    'ar': "💭 نص 1024 حرفًا",
+}
+l_text_text4096 = {
+    'ru': "🗯️ Текст 4096 символа",
+    'en': "🗯️ Text 4096 characters",
+    'es': "🗯️ Texto 4096 caracteres",
+    'fr': "🗯️ Texte 4096 caractères",
+    'zh': "🗯️ 文本 4096 个字符",
+    'ar': "🗯️ نص 4096 حرفًا",
 }
 
-l_btn_button_in = {
-    'ru': "✅ Кнопка ↑",
-    'en': "✅ Button ↑",
-    'es': "✅ Botón ↑",
-    'fr': "✅ Bouton ↑",
-    'zh': "✅按钮↑",
-    'ar': "✅ زر ↑",
+l_convert_error = {
+    'ru': "👩🏽‍💻 <b>Ошибка</b> преобразования контента (попробуй позже и загрузи другой файл)",
+    'en': "👩🏽‍💻 Content conversion <b>error</b> (try later and upload another file)",
+    'es': "👩🏽‍💻 <b>Error</b> de conversión de contenido (intente más tarde y cargue otro archivo)",
+    'fr': "👩🏽‍💻 <b>Erreur</b> de conversion de contenu (essayez plus tard et téléchargez un autre fichier)",
+    'zh': "👩🏽‍💻内容转换<b>错误</b>（稍后再试并上传另一个文件）",
+    'ar': "👩🏽‍💻 <b>خطأ</b> في تحويل المحتوى (حاول لاحقًا وقم بتحميل ملف آخر)",
 }
-l_btn_link = {
-    'ru': "🔗 Ссылка",
-    'en': "🔗 Link",
-    'es': "🔗 Enlace",
-    'fr': "🔗 Lien",
-    'zh': "🔗 链接",
-    'ar': "🔗 رابط",
+l_telegraph_text = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> .jpg/.png/.gif/.mp4 - контент, чтобы создать ссылку",
+    'en': "👩🏽‍💻 <b>Attach</b> .jpg/.png/.gif/.mp4 content to create a link",
+    'es': "👩🏽‍💻 <b>Adjunte</b> contenido .jpg/.png/.gif/.mp4 para crear un enlace",
+    'fr': "👩🏽‍💻 <b>Joignez</b> du contenu .jpg/.png/.gif/.mp4 pour créer un lien",
+    'zh': "👩🏽‍💻<b>附加</b>.jpg/.png/.gif/.mp4 内容以创建链接",
+    'ar': "👩🏽‍💻 <b>أرفق</b> محتوى .jpg / .png / .gif / .mp4 لإنشاء ارتباط",
 }
-l_btn_pay = {
-    'ru': "💳 Оплата",
-    'en': "💳 Payment",
-    'es': "💳 Pago",
-    'fr': "💳 Paiement",
-    'zh': "💳付款",
-    'ar': "💳 الدفع",
+l_telegraph_error = {
+    'ru': "👩🏽‍💻 <b>Ошибка</b> получения ссылки (попробуй позже или загрузи другой файл)",
+    'en': "👩🏽‍💻 <b>Failed</b> to get link (try later and upload another file)",
+    'es': "👩🏽‍💻 <b>No se pudo</b> obtener el enlace (intente más tarde y cargue otro archivo)",
+    'fr': "👩🏽‍💻 <b>Échec</b> de l'obtention du lien (essayez plus tard et téléchargez un autre fichier)",
+    'zh': "👩🏽‍💻 获取链接<b>失败</b>（稍后再试并上传另一个文件）",
+    'ar': "👩🏽‍💻 <b>فشل</b> الحصول على الرابط (حاول لاحقًا وقم بتحميل ملف آخر)",
 }
-l_btn_search = {
-    'ru': "🔎 Поиск",
-    'en': "🔎 Search",
-    'es': "🔎 Buscar",
-    'fr': "🔎 Rechercher",
-    'zh': "🔎 搜索",
-    'ar': "🔎 بحث",
+l_json_text = {
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> любое сообщение или сделай пересылку",
+    'en': "👩🏽‍💻 <b>Attach</b> any message or forward",
+    'es': "👩🏽‍💻 <b>Adjunte</b> cualquier mensaje o reenvíe",
+    'fr': "👩🏽‍💻 <b>Joindre</b> n'importe quel message ou transférer",
+    'zh': "👩🏽‍💻<b>附上</b>任何讯息或转发",
+    'ar': "👩🏽‍💻 <b>إرفاق</b> أي رسالة أو إعادة توجيهها",
 }
-l_btn_like = {
-    'ru': "❤️ Лайк",
-    'en': "❤️ Like",
-    'es': "❤️ Me gusta",
-    'fr': "❤️ J'aime",
-    'zh': "❤️喜欢",
-    'ar': "❤️ مثل",
+# endregion
+
+
+# region FereyTargetBot
+l_subscribe_target = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [<b>Донат</b> на баланс]:\n▪️рассылка/приглашения\n▪️редактирование чаевых\n(<i>чтобы указать точную сумму</i>)\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [<b>Донат</b> на баланс]:\n▪️возможность сделать рассылку по всем ботам\n▪️измените значение чаевых (<i>чтобы указать точную сумму</i>)\n\n👩🏽‍💻 /balance",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
-l_btn_button_kb = {
-    'ru': "✅ Кнопка ↓",
-    'en': "✅ Button ↓",
-    'es': "✅ Botón ↓",
-    'fr': "✅ Bouton ↓",
-    'zh': "✅按钮↓",
-    'ar': "✅ زر ↓",
+# endregion
+
+
+# region FereyAdsBot
+l_ads_btn1 = {
+    'ru': "⛰️ Посты",
+    'en': "⛰️ Posts",
+    'es': "⛰️ Publicaciones",
+    'fr': "⛰️ Messages",
+    'zh': "⛰️ 帖子",
+    'ar': "⛰️ المشاركات",
 }
-l_btn_phone = {
-    'ru': "📞 Сотовый",
-    'en': "📞 Cellular",
-    'es': "📞 Celular",
-    'fr': "📞 Cellulaire",
-    'zh': "📞 手机",
-    'ar': "📞 خلوي",
+l_ads_btn2 = {
+    'ru': "🌬 Подписка",
+    'en': "🌬 Subscription",
+    'es': "🌬 Suscripción",
+    'fr': "🌬 Abonnement",
+    'zh': "🌬订阅",
+    'ar': "🌬 الاشتراك",
 }
-l_btn_geo = {
-    'ru': "📍 Гео",
-    'en': "📍 Geo",
-    'es': "📍 Geo",
-    'fr': "📍 Géo",
-    'zh': "📍地理",
-    'ar': "📍 جيو",
+l_ads_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для создания креативных постов <b>Ferey</b>\n\n▪️️реклама во всех Ferey-ботах\n▪️️заказ рекламы на канале\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <i>the landing bot</i> for creating creative постов <b>Ferey</b>\n\n▪️️advertising in all Ferey bots\n▪️️ ordering advertising on the channel\n\n❗️you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido <i>al bot de aterrizaje</i> para crear постов creativas <b>Ferey</b>\n\n▪️️publicidad en todos los bots de Ferey\n▪️️solicitando publicidad en el canal\n\n❗️también puedes ordenar el desarrollo de un chatbot en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue dans <i>le bot de débarquement</i> pour la création постов créatives <b>Ferey</b>\n\n▪️️publicité dans tous les bots Ferey\n▪️️commande de publicité sur la chaîne\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎来到<b>Ferey</b>创建创意постов的<i>登陆机器人</i>\n\n▪️️在所有 Ferey 机器人中投放广告\n▪️️ 在频道订购广告\n\n❗️您也可以在以下订购聊天机器人的开发我们的Ferey工作室",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> لإنشاء постов إبداعية <b>Ferey</b>\n\nالإعلان في جميع برامج Ferey\n▪️️ طلب الإعلانات على القناة\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
-l_btn_blog = {
-    'ru': "📰 Блог",
-    'en': "📰 Blog",
-    'es': "📰Blog",
-    'fr': "📰 Blogue",
-    'zh': "📰 博客",
-    'ar': "📰 مدونة",
+l_subscribe_ads = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [<b>Донат</b> на баланс]:\n▪️рассылка по всем ботам\n▪️редактирование чаевых\n(<i>чтобы указать точную сумму</i>)\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [<b>Донат</b> на баланс]:\n▪️возможность сделать рассылку по всем ботам\n▪️измените значение чаевых (<i>чтобы указать точную сумму</i>)\n\n👩🏽‍💻 /balance",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
-l_btn_name = {
-    'ru': "Имя:",
-    'en': "Name:",
-    'es': "Nombre:",
-    'fr': "Nom:",
-    'zh': "姓名：",
-    'ar': "اسم:",
+
+l_post_media_ads = {
+    'ru': "✏️ 2. Прикрепи <b>медиа</b> контент: фото/гиф/видео до 5Mb\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'en': "✏️ 2. Attach <b>media</b> content: photo/gif/video up to 5Mb\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
+    'es': "✏️ 2. Adjunte contenido <b>multimedia</b> : foto/gif/video de hasta 5 Mb\n\n( <i>o presione &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
+    'fr': "✏️ 2. Joignez du contenu <b>multimédia</b> : photo/gif/vidéo jusqu&#x27;à 5 Mb\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
+    'zh': "✏️ 2.附加<b>媒体</b>内容：照片/gif/视频最大5Mb\n\n（<i>或按“➡️️/Next”跳过此步骤</i>）",
+    'ar': "✏️ 2. إرفاق محتوى <b>وسائط</b> : صورة / صورة / فيديو بحجم يصل إلى 5 ميغا بايت\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
 }
-l_btn_type = {
-    'ru': "Тип:",
-    'en': "Type:",
-    'es': "Tipo:",
-    'fr': "Taper:",
-    'zh': "类型：",
-    'ar': "يكتب:",
+# endregion
+
+
+# region FereyDemoBot
+l_demo_btn1 = {
+    'ru': "⛰️ Проекты",
+    'en': "⛰️ Projects",
+    'es': "⛰️ Proyectos",
+    'fr': "⛰️ Projets",
+    'zh': "⛰️ 项目",
+    'ar': "⛰️ المشاريع",
+}
+l_demo_btn2 = {
+    'ru': "🌬 Подписка",
+    'en': "🌬 Subscription",
+    'es': "🌬 Suscripción",
+    'fr': "🌬 Abonnement",
+    'zh': "🌬订阅",
+    'ar': "🌬 الاشتراك",
+}
+l_demo_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> проекта <b>Ferey</b>:\n\n▪️<b>информация</b> обо всех проектах\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <i>the landing bot</i> of the <b>Ferey</b> проекта :\n\n▪️ <b>information</b> about all projects\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del проекта <b>Ferey</b> :\n\n▪️ <b>información</b> sobre todos los proyectos\n\n❗️ también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du проекта <b>Ferey</b> :\n\n▪️ <b>informations</b> sur tous les projets\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎来到<b>Ferey</b> проекта的<i>落地机器人</i>：\n\n▪️ 所有项目的<b>信息</b>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص проекта <b>Ferey</b> :\n\n▪️ <b>معلومات</b> حول جميع المشاريع\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
+}
+l_subscribe_demo = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 
-l_check_box_pin_message = {
-    'ru': "Закреп сообщения",
-    'en': "Pin messages",
-    'es': "Anclar mensajes",
-    'fr': "Épingler les messages",
-    'zh': "固定消息",
-    'ar': "تثبيت الرسائل",
+l_kind_1 = {
+    'ru': "<b>👩🏽‍💻@FereyDemoBot</b>\n\n<b>Демо</b> бот всех проектов",
+    'en': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\nDemo bot of all projects",
+    'es': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\nBot de demostración de todos los proyectos",
+    'fr': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\nDemo bot de tous les projets",
+    'zh': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\n所有项目的演示机器人",
+    'ar': "<b>👩🏽‍💻FereyDemoBot</b>\n\nروبوت تجريبي <b>@FereyDemoBot</b> المشاريع",
 }
-l_check_box_protect_message = {
-    'ru': "Защита сообщения",
-    'en': "Message protection",
-    'es': "Protección de mensajes",
-    'fr': "Protection des messages",
-    'zh': "消息保护",
-    'ar': "حماية الرسائل",
+l_kind_2 = {
+    'ru': "<b>👩🏽‍💻@FereyBotBot</b>\n\n<b>Конструктор</b> ботов:\n▪️авто-генерация бота\n▪️авто-генерация контента (open-ai)\n▪️авто-бан/перевод/рассылка",
+    'en': "<b>👩🏽‍💻</b> <b>@FereyBotBot</b>\n\nBot Builder:\n▪️auto-generate bot\n▪️auto-generate content (open-ai)\n▪️auto-ban/auto-translate",
+    'es': "<b>👩🏽‍💻</b> <b>@FereyBotBot</b>\n\nGenerador de bots:\n▪️generación automática de bot\n▪️generación automática de contenido (open-ai)\n▪️prohibición automática/traducción automática",
+    'fr': "<b>👩🏽‍💻</b> <b>@FereyBotBot</b>\n\nBot Builder :\n▪️auto-génère le bot\n▪️auto-génère le contenu (open-ai)\n▪️auto-ban/auto-translate",
+    'zh': "<b>👩🏽‍💻</b> <b>@FereyBotBot</b>\n\nBot Builder：\n▪️自动生成机器人\n▪️自动生成内容（open-ai）\n▪️自动禁止/自动翻译",
+    'ar': "<b>👩🏽‍💻FereyBotBot</b>\n\nBot Builder:\n▪️ إنشاء روبوت تلقائيًا <b>@FereyBotBot</b> n▪️ إنشاء محتوى تلقائيًا (فتح ai)\n▪️ حظر تلقائي / ترجمة آلية",
 }
-l_check_box_edit_message = {
-    'ru': "Изменить текущее сообщение",
-    'en': "Edit current message",
-    'es': "Editar mensaje actual",
-    'fr': "Modifier le message actuel",
-    'zh': "编辑当前消息",
-    'ar': "تحرير الرسالة الحالية",
+l_kind_3 = {
+    'ru': "<b>👩🏽‍💻@FereyChannelBot</b>\n\n<b>Администрирование</b> каналов:\n▪️авто-постинг\n▪️авто-декор",
+    'en': "<b>👩🏽‍💻</b> <b>@FereyChannelBot</b>\n\nChannel admin:\n▪️auto-posting\n▪️auto-decor",
+    'es': "<b>👩🏽‍💻</b> <b>@FereyChannelBot</b>\n\nAdministrador del canal:\n▪️publicación automática\n▪️decoración automática",
+    'fr': "<b>👩🏽‍💻</b> <b>@FereyChannelBot</b>\n\nAdministrateur de la chaîne :\n▪️publication automatique\n▪️décoration automatique",
+    'zh': "<b>👩🏽‍💻</b> <b>@FereyChannelBot</b>\n\n频道管理员：\n▪️自动发布\n▪️自动装饰",
+    'ar': "<b>👩🏽‍💻FereyChannelBot</b>\n\nمسؤول القناة:\nنشر تلقائي <b>@FereyChannelBot</b> n ديكور تلقائي",
 }
-l_check_box_auto_format = {
-    'ru': "Авто формат сообщения",
-    'en': "Auto message format",
-    'es': "Formato de mensaje automático",
-    'fr': "Format de message automatique",
-    'zh': "自动消息格式",
-    'ar': "تنسيق الرسالة التلقائي",
+l_kind_4 = {
+    'ru': "<b>👩🏽‍💻@FereyGroupBot</b>\n\n<b>Модерация</b> групп:\n▪️авто-постинг\n▪️модерация",
+    'en': "<b>👩🏽‍💻</b> <b>@FereyGroupBot</b>\n\nGroup admin:\n▪️auto-posting\n▪️moderation",
+    'es': "<b>👩🏽‍💻</b> <b>@FereyGroupBot</b>\n\nAdministrador del grupo:\n▪️publicación automática\n▪️moderación",
+    'fr': "<b>👩🏽‍💻</b> <b>@FereyGroupBot</b>\n\nAdministrateur du groupe :\n▪️publication automatique\n▪️modération",
+    'zh': "<b>👩🏽‍💻</b> <b>@FereyGroupBot</b>\n\n群组管理员：\n▪️自动发布\n▪️审核",
+    'ar': "<b>👩🏽‍💻FereyGroupBot</b>\n\n<b>@FereyGroupBot</b> المجموعة:\nنشر تلقائي\n▪️ تعديل",
 }
-l_check_box_auto_typing = {
-    'ru': "Авто печатание сообщения",
-    'en': "Auto typing message",
-    'es': "Mensaje de escritura automática",
-    'fr': "Message de saisie automatique",
-    'zh': "自动输入信息",
-    'ar': "رسالة الكتابة التلقائية",
+l_kind_5 = {
+    'ru': "<b>👩🏽‍💻@FereyUserBot</b>\n\n<b>Автоматизация</b> пользователей:\n▪️авто-постинг\n▪️авто-декор",
+    'en': "<b>👩🏽‍💻</b> <b>@FereyUserBot</b>\n\nUser Admin:\n▪️auto-posting\n▪️auto-decor",
+    'es': "<b>👩🏽‍💻</b> <b>@FereyUserBot</b>\n\nAdministrador de usuarios:\n▪️publicación automática\n▪️decoración automática",
+    'fr': "<b>👩🏽‍💻</b> <b>@FereyUserBot</b>\n\nAdministrateur utilisateur :\n▪️publication automatique\n▪️décoration automatique",
+    'zh': "<b>👩🏽‍💻</b> <b>@FereyUserBot</b>\n\n用户管理员：\n▪️自动发布\n▪️自动装饰",
+    'ar': "<b>👩🏽‍💻FereyUserBot</b>\n\nمسؤول المستخدم:\nنشر <b>@FereyUserBot</b>\nديكور تلقائي",
 }
-l_check_box_preview = {
-    'ru': "Превью контент",
-    'en': "Preview content",
-    'es': "Vista previa del contenido",
-    'fr': "Prévisualiser le contenu",
-    'zh': "预览内容",
-    'ar': "معاينة المحتوى",
+l_kind_6 = {
+    'ru': "<b>👩🏽‍💻@FereyPostBot</b>\n\n<b>Приватные посты</b>:\n▪️превью\n▪️галерея",
+    'en': "<b>👩🏽‍💻</b> <b>@FereyPostBot</b>\n\nQuick post creation and publishing:\n▪️preview\n▪️gallery",
+    'es': "<b>👩🏽‍💻</b> <b>@FereyPostBot</b>\n\nCreación y publicación rápidas de publicaciones:\n▪️vista previa\n▪️galería",
+    'fr': "<b>👩🏽‍💻</b> <b>@FereyPostBot</b>\n\nCréation et publication rapides d'articles :\n▪️aperçu\n▪️galerie",
+    'zh': "<b>👩🏽‍💻</b> <b>@FereyPostBot</b>\n\n快速创建和发布帖子：\n▪️预览\n▪️图库",
+    'ar': "<b>👩🏽‍💻FereyPostBot</b>\n\nإنشاء منشور سريع <b>@FereyPostBot</b> :\nمعاينة\n▪️ معرض",
 }
-l_check_box_spoiler = {
-    'ru': "Гиф/фото/видео спойлер",
-    'en': "GIF/photo/video spoiler",
-    'es': "Spoiler de GIF/foto/video",
-    'fr': "Spoiler GIF/photo/vidéo",
-    'zh': "GIF/照片/视频剧透",
-    'ar': "مفسد GIF / صور / فيديو",
+l_kind_7 = {
+    'ru': "<b>👩🏽‍💻@FereyFindBot</b>\n\n<b>Поиск</b> по каналам/группам/пользователям/ботам:\n▪️отслеживание постов\n▪️гео-поиск",
+    'en': "<b>👩🏽‍💻</b> <b>@FereyFindBot</b>\n\nSearch by channels/groups/users/bots:\n▪️post tracking\n▪️geo-search",
+    'es': "<b>👩🏽‍💻</b> <b>@FereyFindBot</b>\n\nBuscar por canales/grupos/usuarios/bots:\n▪️seguimiento de publicaciones\n▪️búsqueda geográfica",
+    'fr': "<b>👩🏽‍💻</b> <b>@FereyFindBot</b>\n\nRecherche par canaux/groupes/utilisateurs/bots :\n▪️suivi des publications\n▪️géo-recherche",
+    'zh': "<b>👩🏽‍💻</b> <b>@FereyFindBot</b>\n\n按频道/群组/用户/机器人搜索：\n▪️post tracking\n▪️geo-search",
+    'ar': "<b>👩🏽‍💻FereyFindBot</b>\n\nالبحث عن طريق القنوات / المجموعات <b>@FereyFindBot</b> المستخدمين / الروبوتات:\n▪️ تتبع المنشور\n▪️ البحث الجيو",
 }
-l_check_box_silence = {
-    'ru': "Тихое сообщение",
-    'en': "Quiet message",
-    'es': "Mensaje tranquilo",
-    'fr': "Message silencieux",
-    'zh': "悄悄话",
-    'ar': "رسالة هادئة",
+l_kind_8 = {
+    'ru': "<b>👩🏽‍💻@FereyMediaBot</b>\n\n<b>Медиа-заметки</b>:\n▪️аудио/️видео-заметки\n▪️текст/фото-стикеры",
+    'en': "<b>👩🏽‍💻</b> <b>@FereyMediaBot</b>\n\nBot with popular creatives:\n▪️audio notes\n▪️video notes",
+    'es': "<b>👩🏽‍💻</b> <b>@FereyMediaBot</b>\n\nBot con creatividades populares:\n▪️notas de audio\n▪️notas de video",
+    'fr': "<b>👩🏽‍💻</b> <b>@FereyMediaBot</b>\n\nBot avec des créations populaires :\n▪️notes audio\n▪️notes vidéo",
+    'zh': "<b>👩🏽‍💻</b> <b>@FereyMediaBot</b>\n\n具有流行创意的机器人：\n▪️音频笔记\n▪️视频笔记",
+    'ar': "<b>👩🏽‍💻FereyMediaBot</b>\n\nاستخدام التصميمات المشهورة:\n▪️ ملاحظات <b>@FereyMediaBot</b>\n▪️ ملاحظات الفيديو",
+}
+l_kind_9 = {
+    'ru': "<b>👩🏽‍💻@FereyVPNBot</b>\n\n<b>Настройка</b>VPN",
+    'en': "<b>👩🏽‍💻</b> <b>@FereyVpnBot</b>\n\nAll about VPN",
+    'es': "<b>👩🏽‍💻</b> <b>@FereyVpnBot</b>\n\nTodo sobre VPN",
+    'fr': "<b>👩🏽‍💻</b> <b>@FereyVpnBot</b>\n\nTout sur le VPN",
+    'zh': "<b>👩🏽‍💻</b> <b>@FereyVpnBot</b>\n\n关于 VPN",
+    'ar': "<b>👩🏽‍💻FereyVpnBot</b> <b>@FereyVpnBot</b> n\nكل شيء عن VPN",
+}
+l_kind_10 = {
+    'ru': "<b>👩🏽‍💻@FereyTargetBot</b>\n\n<b>Таргет</b> сообщений/пользователей",
+    'en': "<b>👩🏽‍💻</b> <b>@FereyTargetBot</b>\n\nTargeted email",
+    'es': "<b>👩🏽‍💻</b> <b>@FereyTargetBot</b>\n\nCorreo electrónico dirigido",
+    'fr': "<b>👩🏽‍💻</b> <b>@FereyTargetBot</b>\n\nE-mail ciblé",
+    'zh': "<b>👩🏽‍💻</b> <b>@FereyTargetBot</b>\n\n目标电子邮件",
+    'ar': "<b>👩🏽‍💻FereyTargetBot</b> \ <b>@FereyTargetBot</b>\nالبريد الإلكتروني المستهدف",
+}
+l_kind_11 = {
+    'ru': "<b>👩🏽‍💻@FereyToolsBot</b>\n\n<b>Телеграм инструменты</b>:\n▪️конвертация файлов\n▪️шаблоны",
+    'en': "<b>👩🏽‍💻</b> <b>@FereyToolsBot</b>\n\nTool bot:\n▪️convert\n▪️download",
+    'es': "<b>👩🏽‍💻</b> <b>@FereyToolsBot</b>\n\nHerramienta bot:\n▪️convertir\n▪️descargar",
+    'fr': "<b>👩🏽‍💻</b> <b>@FereyToolsBot</b>\n\nBot outil :\n▪️convertir\n▪️télécharger",
+    'zh': "<b>👩🏽‍💻</b> <b>@FereyToolsBot</b>\n\n工具机器人：\n▪️转换\n▪️下载",
+    'ar': "<b>👩🏽‍💻FereyToolsBot</b>\n\ <b>@FereyToolsBot</b> بوت الأداة:\n▪️ تحويل\n▪️ تحميل",
+}
+l_kind_12 = {
+    'ru': "<b>👩🏽‍💻@FereyAIBot</b>\n\n<b>Нейросеть</b> генерации контента (open-ai):\n▪️chat-gpt\n▪️dalli·e",
+    'en': "<b>👩🏽‍💻</b> <b>@FereyAIBot</b>\n\nContent generation bot (open-ai):\n▪️chat-gpt\n▪️dalli e",
+    'es': "<b>👩🏽‍💻</b> <b>@FereyAIBot</b>\n\nBot de generación de contenido (open-ai):\n▪️chat-gpt\n▪️dalli e",
+    'fr': "<b>👩🏽‍💻</b> <b>@FereyAIBot</b>\n\nBot de génération de contenu (open-ai) :\n▪️chat-gpt\n▪️dalli e",
+    'zh': "<b>👩🏽‍💻</b> <b>@FereyAIBot</b>\n\n内容生成机器人（open-ai）：\n▪️chat-gpt\n▪️dalli e",
+    'ar': "<b>👩🏽‍💻FereyAIBot</b>\n\nروبوت إنشاء المحتوى (open <b>@FereyAIBot</b> ai):\n▪️chat-gpt\n▪️dalli e",
+}
+l_kind_13 = {
+    'ru': "<b>👩🏽‍💻@FereyAdsBot</b>\n\n<b>Реклама</b> в:\n▪️ботах",
+    'en': "<b>👩🏽‍💻</b> <b>@FereyAdsBot</b>\n\nBot ads in:\n▪️bots\n▪️channels",
+    'es': "<b>👩🏽‍💻</b> <b>@FereyAdsBot</b>\n\nAnuncios de bot en:\n▪️bots\n▪️canales",
+    'fr': "<b>👩🏽‍💻</b> <b>@FereyAdsBot</b>\n\nAnnonces de robots dans :\n▪️bots\n▪️chaînes",
+    'zh': "<b>👩🏽‍💻</b> <b>@FereyAdsBot</b>\n\n机器人广告在：\n▪️bots\n▪️channels",
+    'ar': "<b>👩🏽‍💻FereyAdsBot</b>\n\n<b>@FereyAdsBot</b> الإعلانات في:\n▪️ الروبوتات\n▪️ القنوات",
+}
+l_kind_14 = {
+    'ru': "<b>👩🏽‍💻@FereyWorkBot</b>\n\n<b>Рабочий</b> бот информации о:\n▪️вакансиях\n▪️соревнованиях",
+    'en': "<b>👩🏽‍💻</b> <b>@FereyWorkBot</b>\n\nBot of information about:\n▪️vacancies\n▪️competitions",
+    'es': "<b>👩🏽‍💻</b> <b>@FereyWorkBot</b>\n\nBot de información sobre:\n▪️vacantes\n▪️concursos",
+    'fr': "<b>👩🏽‍💻</b> <b>@FereyWorkBot</b>\n\nBot d'informations sur :\n▪️offres d'emploi\n▪️concours",
+    'zh': "<b>👩🏽‍💻</b> <b>@FereyWorkBot</b>\n\n有关以下信息的机器人：\n▪️职位空缺\n▪️比赛",
+    'ar': "<b>👩🏽‍💻FereyWorkBot</b>\n\nبعض <b>@FereyWorkBot</b> حول:\n▪️ وظائف شاغرة\n▪️ مسابقات",
 }
-# endregion
 # endregion
 
 
-# region FereyUserBot
-l_subscribe_user = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>рассылка</b> пользователям\n▪️<b>экстра</b> бот\n\n👩🏽‍💻 /balance",
+# region FereyVPNBot
+l_vpn_btn1 = {
+    'ru': "⛰️ VPN",
+    'en': "⛰️ VPN",
+    'es': "⛰️VPN",
+    'fr': "⛰️VPN",
+    'zh': "⛰️ VPN",
+    'ar': "⛰️ VPN",
+}
+l_vpn_btn2 = {
+    'ru': "🌬 Подписка",
+    'en': "🌬 Subscription",
+    'es': "🌬 Suscripción",
+    'fr': "🌬 Abonnement",
+    'zh': "🌬订阅",
+    'ar': "🌬 الاشتراك",
+}
+l_vpn_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> проекта Ferey:\n\n▪️<b>openvpn</b>\n▪️<b>wireguard</b>\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <i>the landing bot</i> of the Ferey project:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del proyecto Ferey:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du projet Ferey :\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎来到 Ferey 项目的<i>落地机器人</i>：\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص بمشروع Ferey:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey",
+}
+l_subscribe_vpn = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
     'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
+
+l_vpn_1 = {
+    'ru': "👩🏽‍💻 <b>Open VPN</b>\n\n{0}",
+    'en': "👩🏽‍💻 <b>Open VPN</b>\n\n{0}",
+    'es': "👩🏽‍💻 <b>Abrir VPN</b>\n\n{0}",
+    'fr': "👩🏽‍💻 <b>Ouvrez le VPN</b>\n\n{0}",
+    'zh': "👩🏽‍💻<b>打开 VPN</b>\n\n{0}",
+    'ar': "👩🏽‍💻 <b>افتح VPN</b>\n\n{0}",
+}
+l_vpn_2 = {
+    'ru': "👩🏽‍💻 <b>Wire Guard</b>\n\n{0}",
+    'en': "👩🏽‍💻 <b>Wire Guard</b>\n\n{0}",
+    'es': "👩🏽‍💻 <b>Protector de alambre</b>\n\n{0}",
+    'fr': "👩🏽‍💻 <b>Fil de protection</b>\n\n{0}",
+    'zh': "👩🏽‍💻<b>线卫士</b>\n\n{0}",
+    'ar': "👩🏽‍💻 <b>واقي الأسلاك</b>\n\n{0}",
+}
 # endregion
 
 
-# region FereyTargetBot
-l_subscribe_target = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [<b>Донат</b> на баланс]:\n▪️рассылка/приглашения\n▪️редактирование чаевых\n(<i>чтобы указать точную сумму</i>)\n\n👩🏽‍💻 /balance",
-    'en': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [<b>Донат</b> на баланс]:\n▪️возможность сделать рассылку по всем ботам\n▪️измените значение чаевых (<i>чтобы указать точную сумму</i>)\n\n👩🏽‍💻 /balance",
+# region FereyWorkBot
+l_work_btn1 = {
+    'ru': "⛰️ Вакансии",
+    'en': "⛰️ Jobs",
+    'es': "⛰️ Empleos",
+    'fr': "⛰️ Emplois",
+    'zh': "⛰️ 工作",
+    'ar': "⛰️ وظائف",
+}
+l_work_btn2 = {
+    'ru': "🌬 Подписка",
+    'en': "🌬 Subscription",
+    'es': "🌬 Suscripción",
+    'fr': "🌬 Abonnement",
+    'zh': "🌬订阅",
+    'ar': "🌬 الاشتراك",
+}
+l_work_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> проекта <b>Ferey</b>:\n\n▪️<b>вакансии</b> нашего стартапа\n▪️конкурсы и <b>мероприятия</b>\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <i>the landing bot</i> of the <b>Ferey</b> проекта :\n\n▪️ <b>vacancies</b> of our startup\n▪️ contests and <b>events</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del проекта <b>Ferey</b> :\n\n▪️ <b>vacantes</b> de nuestra startup\n▪️ concursos y <b>eventos</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du проекта <b>Ferey</b> :\n\n▪️ <b>offres d&#x27;emploi</b> de notre startup\n▪️ concours et <b>événements</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎来到<b>Ferey</b> проекта的<i>登陆机器人</i>：\n\n▪️ 我们初创公司的<b>职位空缺</b>\n▪️ 竞赛和<b>活动</b>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> проекта <b>Ferey</b> :\n\n▪️ <b>الشواغر</b> في بدء التشغيل\n▪️ المسابقات <b>والأحداث</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey",
+}
+l_subscribe_work = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
     'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
-# endregion
+
+l_vacancy_1 = {
+    'ru': "👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company",
+    'en': "👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company",
+    'es': "👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTareas: crear máscaras ferey (video realista) para cualquier humano\nGénero: niña\nEdad: menos de 30\nPago: parte de la empresa",
+    'fr': "👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTâches : créer des masques de ferey (vidéo réaliste) pour tout humain\nSexe : fille\nÂge : moins de 30 ans\nPaiement : part de l'entreprise",
+    'zh': "👩🏽‍💻<b>文本到视频 ai-designer</b>\n\n任务：为任何人创建 ferey-mask（逼真的视频）\n性别：女孩\n年龄：30 岁以下\n薪酬：公司股份",
+    'ar': "👩🏽‍💻 <b>نص إلى فيديو مصمم ai</b>\n\nالمهام: إنشاء أقنعة ضيقة (فيديو واقعي) لأي إنسان\nالجنس: فتاة\nالعمر: أقل من 30\nالدفع: حصة الشركة",
+}
+l_vacancy_2 = {
+    'ru': "👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials",
+    'en': "👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials",
+    'es': "👩🏽‍💻 <b>Creador de contenido/video</b>\n\nTareas: generar creatividades para todas las redes sociales\nGénero: niña\nEdad: menos de 30\nPago: 1 TON por 1 publicación para todas las redes sociales",
+    'fr': "👩🏽‍💻 <b>Créateur de contenu/vidéo</b>\n\nTâches : générer des créations pour tous les réseaux sociaux\nSexe : fille\nÂge : moins de 30 ans\nPaiement : 1 TON pour 1 post pour tous les réseaux sociaux",
+    'zh': "👩🏽‍💻<b>内容/视频制作者</b>\n\n任务：为所有社交生成创意\n性别：女孩\n年龄：小于 30\n报酬：所有社交每 1 个帖子 1 吨",
+    'ar': "👩🏽‍💻 <b>صانع المحتوى / الفيديو</b>\n\nالمهام: إنشاء تصميمات لجميع وسائل التواصل الاجتماعي\nالجنس: فتاة\nالعمر: أقل من 30\nالدفع: 1 طن لكل مشاركة واحدة لجميع الشبكات الاجتماعية",
+}
+l_vacancy_3 = {
+    'ru': "👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company",
+    'en': "👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company",
+    'es': "👩🏽‍💻 <b>Desarrollador Aio/pyro-gram</b>\n\nTareas: desarrollar y apoyar todos los proyectos\nGénero: niña\nEdad: menos de 30\nPago: parte de la empresa",
+    'fr': "👩🏽‍💻 <b>Développeur Aio/pyro-gram</b>\n\nTâches : développement et support de tous les projets\nSexe : fille\nÂge : moins de 30 ans\nRémunération : part de l'entreprise",
+    'zh': "👩🏽‍💻 <b>Aio/pyro-gram 开发者</b>\n\n任务：开发和支持所有项目\n性别：女孩\n年龄：30岁以下\n薪酬：公司股份",
+    'ar': "👩🏽‍💻 <b>مطور Aio / pyro-gram</b>\n\nالمهام: تطوير ودعم جميع المشاريع\nالجنس: فتاة\nالعمر: أقل من 30\nالدفع: حصة الشركة",
+}
+# endregion
```

### Comparing `yeref-0.1.96/yeref/yeref.py` & `yeref-0.1.98/yeref/yeref.py`

 * *Files identical despite different names*

