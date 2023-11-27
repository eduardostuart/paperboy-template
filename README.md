<img src="https://raw.githubusercontent.com/eduardostuart/paperboy/main/.github/resources/paperboy.png" alt="Paperboy" width="240" align="right">

# Paperboy template

A GitHub template that [delivers](.github/workflows/cron.yml) new posts from all your favorite sites by email.

## Usage

1. Click on `use this template`
2. Update the `subs.txt` file. Include your list of websites.

Example:

```
https://blog.laravel.com/feed
# https://news.mit.edu/rss/feed (this will be ignored)
https://blog.mozilla.org/feed
```

3. Set these environment variable values (`GitHub Secrets`):

```bash
SMTP_HOST="smtp.mailtrap.io"               # SMTP host
SMTP_PORT=2525                             # SMTP port
SMTP_USERNAME="username"                   # SMTP username
SMTP_PASSWORD="password"                   # SMTP password
SMTP_FROM="Paperboy <rss@domain.com>"      # the sender
MAIL_TO="email@domain.com"                 # the recipient
EMAIL_SUBJECT="Subject"                    # Email subject (optional)
```

4. Update `template.hbs` & `template_text.hbs` if you want to customize the email template.
5. Update `.github/workflows/cron.yml` if you want to change the frequency or time that you want to receive the email.
6. If you just want to test, trigger the `.github/workflows/manual.yml` GitHub Action.

## License

This code is distributed under the terms of MIT license.
See [LICENSE-MIT](LICENSE-MIT) for details.
