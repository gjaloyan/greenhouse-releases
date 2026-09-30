# Теплица — пакеты установки для Arduino UNO Q

Здесь только готовые пакеты системы «Теплица»: программа для платы и служба восстановления. Без
истории разработки. Репозиторий закрыт; открывайте его только на время установки.

## Установка или обновление с GitHub

1. Откройте репозиторий: Settings → Danger Zone → Change visibility → **Public**.
2. На плате, под пользователем `arduino`:

   ```
   cd /tmp && curl -fsSL -o greenhouse.tar.gz https://github.com/gjaloyan/greenhouse-releases/releases/latest/download/greenhouse.tar.gz && tar xzf greenhouse.tar.gz && ./greenhouse/install.sh
   ```

3. Закройте репозиторий: Change visibility → **Private**.

Та же команда ставит систему на новую плату и обновляет уже установленную (настройки остаются).
Сброс к заводским: `./greenhouse/install.sh --factory-reset`.

Подробная инструкция — `INSTALL.md` внутри пакета. Каждый выпуск лежит в Releases двумя
одинаковыми файлами: `greenhouse-<версия>.tar.gz` и `greenhouse.tar.gz` (для ссылки «последний»).
