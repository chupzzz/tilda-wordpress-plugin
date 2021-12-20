# Плагин Tilda для WordPress
Интегрирует контент, который был создан на Tilda, с вашим сайтом на WordPress.  
https://help-ru.tilda.ws/wordpress-plug-in


## Подключение плагина для WordPress

Подробная инструкция установки плагина  
https://help-ru.tilda.ws/wordpress

## Краткая инструкция

* Скачать плагин https://wordpress.org/plugins/tilda-publishing/
* Загрузите в папку `/wp-content/plugins` папку с плагином (`tilda-wordpress-plugin`)
* Зайдите в панель администрирования сайтом
* Перейдите в раздел управления плагинами (Плагины/Установленные)
* Найдите плагин Tilda Publishing API и нажмите «Активировать»
* Получите публичный и секретный ключ. Для этого в вашем аккаунте откройте вкладку API в настройках проекта в разделе "Действия"
* Перейдите в раздел Настроек плагина (Настройки/Tilda Publishing)
* Нажмите `Добавить API ключ`
* Введите публичный и секретный ключи, сгенерированные на Тильде. Нажмите `Сохранить`.

## Обновление плагина с версии 0.1 на версию 0.2
После обновления, нужно активировать новую версию плагина и удалить старую версию. Сделать это можно в разделе управления плагинами (Плагины/Установленные).
У новой версии изменилась папка размещения плагина с tilda на tilda-wordpress-plugin

## Использование плагина

Перед подключением плагина создайте в Тильде как минимум один проект и одну страницу.

* Нажмите `Добавить новую` (страницу или запись)
* Введите заголовок страницы или записи (иначе Тильда не подключится)
* Если список проектов и страниц не отображается, нажмите `Обновить список`
* В списке слева выберите нужный проект, в котором находится страница, которую вы хотите подключить.
* В списке справа выберете страницу.
* После выбора страницы нажмите `Сохранить`. Готово, все данные страницы находятся теперь на вашем сервере.

При изменении страницы на Тильде вам необходимо нажать на вашем сайте у страницы кнопку `Синхронизировать`.

## FAQ

В: Можно ли автоматически обновлять страницу на вордпрессе, после публикации страницы на Тильде?
О: Да, можно. Для этого нужно указать в настройках API Тильды, следующий урл для callback-вызова http://your-wordpress-site.ru/wp-admin/admin-ajax.php?action=tilda_sync_event

В: Можно ли скачать плагин из GIT-репозитория
О: Да, плагин доступен по адресу https://github.com/greensun7/tilda-wordpress-plugin