# GoLDen SoFT ERP

This repository currently contains a Django project scaffold with an HRM app. The
accounting, inventory, and API modules described as future ERP functionality are
not implemented yet.

## Security configuration

Set these environment variables before starting Django:

- `DJANGO_SECRET_KEY`: a newly generated, private key. Generate one with
  `python -c "from django.core.management.utils import get_random_secret_key; print(get_random_secret_key())"`.
- `DJANGO_ALLOWED_HOSTS`: comma-separated hostnames, for example
  `localhost,127.0.0.1` for local development or your deployed domain.
- `DJANGO_DEBUG`: optional; defaults to `False`. Set to `True` only for local
  development.

The key previously committed in `gserp/settings.py` was public and must not be
used for any deployment. If it was used by a running deployment, replace it
there and invalidate sessions signed with that key.
