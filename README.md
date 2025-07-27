# SnapDish

SnapDish is a Django web application that allows restaurants to generate QR codes for their digital menus. 
Users can enter their restaurant name and menu URL, and the app will create a downloadable QR code image.

## Features
- Generate QR codes for restaurant menus
- Download QR code images
- Simple and modern Bootstrap UI

## Requirements
- Python 3.13+
- Django 5.2.4
- Bootstrap (via CDN)

## Setup Instructions

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd qr-code-django
   ```

2. **Create and activate a virtual environment**
   ```bash
   python3 -m venv env
   source env/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install django
   pip install qrcode
   pip install pillow
   ```

4. **Run migrations**
   ```bash
   python manage.py migrate
   ```

5. **Start the development server**
   ```bash
   python manage.py runserver
   ```

6. **Access the app**
   Open your browser and go to `http://127.0.0.1:8000/`

## Project Structure
```
qr-code-django/
├── SnapDish/
│   ├── __init__.py
│   ├── asgi.py
│   ├── forms.py
│   ├── settings.py
│   ├── urls.py
│   ├── views.py
│   └── wsgi.py
├── templates/
│   ├── generate_qr_code.html
│   └── qr_result.html
├── db.sqlite3
├── manage.py
└── env/
```

## Usage
1. Fill in the restaurant name and menu URL on the homepage.
2. Click "Generate QR Code".
3. Download the generated QR code image.

## License
This project is licensed under the MIT License.
