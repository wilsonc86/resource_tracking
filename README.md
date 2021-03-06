# Resource Tracking application

Django and Leaflet application that collects tracking information using IMAP
from a mailbox and displays it on a collection of layers provided by
Geoserver. The application also downloads observation data from
automatic weather stations.

# Environment variables

This project uses confy to set environment variables (in a `.env` file).
The following variables are required for the project to run:

    DATABASE_URL="postgis://USER:PASSWORD@HOST:PORT/DATABASE_NAME"
    SECRET_KEY="ThisIsASecretKey"

Variables below may also need to be defined (context-dependent):

    DEBUG=True
    CSRF_COOKIE_SECURE=False
    SESSION_COOKIE_SECURE=False
    EMAIL_HOST="email.host"
    EMAIL_PORT=25
    EMAIL_PASSWORD="password"
    TRACPLUS_URL="https://your-trackplus-gateway-url/parameters"
