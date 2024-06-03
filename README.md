1. create requirements.txt , put Django in

2. 
ALLOWED_HOSTS = [os.environ['WEBSITE_HOSTNAME']] if 'WEBSITE_HOSTNAME' in os.environ else []
CSRF_TRUSTED_ORIGINS = ['https://'+ os.environ['WEBSITE_HOSTNAME']] if 'WEBSITE_HOSTNAME' in os.environ else []

3.
    # Enables whitenoise for serving static files
    'whitenoise.middleware.WhiteNoiseMiddleware',

https://learn.microsoft.com/en-us/training/modules/django-get-started/5-exercise-first-project