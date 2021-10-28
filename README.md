### Usage:
1. Rename .env.example to .env and fill up with your data
1. Launch application `docker-compose -f stack.yml up --build`
1. Create superuser: `docker-compose -f stack.yml exec app ./manage.py create superuser`
1. You are ready to enter to the [admin part of site](http://127.0.0.1:8000/admin)
