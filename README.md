<img src="https://raw.githubusercontent.com/eduardostuart/paperboy/main/.github/resources/paperboy.png" alt="Paperboy" width="160" align="right">

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
SMTP_HOST="smtp.mailtrap.io" # Which service are you using? fastmail? gmail? sendgrid? ...
SMTP_PORT=2525 # 25 is the default port
SMTP_USERNAME="username"
SMTP_PASSWORD="password"
SMTP_FROM="Paperboy <rss@your-domain.com>" # Who will send new posts by email?
MAIL_TO="email@domain.com"
```

4. Update `template.hbs` if you want to customize the email template.
5. Update `.github/workflows/cron.yml` if you want to change the frequency or time that you want to receive the email.
6. If you just want to test, trigger the `.github/workflows/manual.yml` GitHub Action.

**Example**: https://github.com/eduardostuart/paperboy-eduardo

## License

This code is distributed under the terms of MIT license.
See [LICENSE-MIT](LICENSE-MIT) for details.
