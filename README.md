Welcome to the mandrill_logger wiki!

# Installation


    pip install mandrill-logger

*Add to INSTALLED_APPS*

    'mandrill_logger',

*Migrate*

    python manage.py migrate mandrill_logger

*Implement Mandrill Logger*
After you have sent your email, simply send the email to log_email:

    from mandrill_logger.utils import MandrillLogger
    mandrill_logger = MandrillLogger()
    mandrill_logger.log_email(email)

