# My Custom theme for openstack horizon

## Installation:

    cd horizon/openstack_dashboard/themes/
    git clone <paste this repo url>

- Open horizon/openstack_dashboard/local/local_settings.py
    and add theme to AVAILABLE_THEMES:

      ('custom-theme', 'Custom', 'themes/custom'),

- Prepare static:

        python manage.py collectstatic
        python manage.py compress

- Restart horizon server
