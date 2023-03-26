## Introdution

This is an ItIsAllMail driver used to convert local Viber sqlite database to Maildir. You need Viber being installed, or at least have Viber profile dir.

## Installation:

1) Install ItIsAllMail.
2) Install the driver.

    cd lib/ItIsAllMail/Driver/
    git clone https://github.com/yalexwander/iam-driver-viber.local viber.local

3) Add driver to ItIsAllMail `conf/config.yml`:

```
drivers :
  - "viber.local"
```

2) Add source in `conf/sources.yml`:

```
- url: viber.local:/home/user/.ViberPC/12312321125
  mailbox_base_dir: /tmp
  mailbox: mailbox_viber
```

12312321125 - is basically your number without leading plus. Or any ID Viber use to create directory.
