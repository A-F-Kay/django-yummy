### Usage:
1. Rename .env.example to .env and fill up with your data
1. Add executable rigts for ./compose: `chmod +x ./compose`
1. Launch application: `./compose up --build -d` (`--build` and `-d` are optional)
1. Create superuser: `./compose exec app ./manage.py createsuperuser`
1. You are ready to enter to the [admin part of site](http://127.0.0.1:8000/admin)

