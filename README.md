<img src="https://raw.githubusercontent.com/eduardostuart/paperboy/main/.github/resources/paperboy.png" alt="Paperboy" width="160" align="right">

# Paperboy template

A GitHub template that [delivers](.github/workflows/cron.yml) new posts from all your favorite sites by email.

## Usage

Set these environment variable values:

```bash
SMTP_HOST="smtp.mailtrap.io" # Which service are you using? fastmail? gmail? sendgrid? ...
SMTP_PORT=2525 # 25 is the default port
SMTP_USERNAME="username"
SMTP_PASSWORD="password"
SMTP_FROM="Paperboy <rss@your-domain.com>" # Who will send new posts by email?
MAIL_TO="email@domain.com"
```

## License

This code is distributed under the terms of MIT license.
See [LICENSE-MIT](LICENSE-MIT) for details.
