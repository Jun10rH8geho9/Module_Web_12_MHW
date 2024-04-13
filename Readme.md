Запуск uvicorn
uvicorn main:app --host localhost --port 8000 --reload

запуск html
http://127.0.0.1:8000/docs

poetry shell

ініціалізування оточення alembic
alembic init migrations

Створюємо міграцію наступною консольною командою в корені проекту.
alembic revision --autogenerate -m 'Init'

застосуємо створену міграцію:
alembic upgrade head

poetry export --without-hashes --format=requirements.txt > requirements.txt
poetry export -f requirements.txt --output requirements.txt
