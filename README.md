# first_site
Первый сайт на FastAPI


Создать виртуальное окружение с нужной версией python

uv venv --python 3.12

Создать проект в нем

uv init

Добавить зависимость в проект

uv add requests
pip install "fastapi[standard]"
или
uv pip install -r requirements.txt

- `my_lib` - установка абсолютно последней версии
- `my_lib>=1.0.0` - установка последней минорной версии
- `my_lib~=1.0.0` - установка последней патч версии
- `my_lib==1.0.0` - установка конкретной версии

Указать версию
uv add "pandas>=2.0.0"

Указать версию библиотеки из github

uv pip install "git+https://github.com/psf/requests
uv add "git+https://github.com/psf/requests(для фиксации в pyproject.toml)

Проверить установленные пакеты
uv pip list

Точная информация в uv.lock

Удаление ненужной бибилиотеки

uv remove requests

если пакет был установлен вручную

uv pip uninstall package-name

Создать окружение с текущей версией python

uv venv
source .venv/bin/activate

Запустить скрипт в окружении и с зависимостями

uv run main.py

конкретно этот

uv run fastapi dev main.py

Синхронизация с вируальным окружением

uv sync
