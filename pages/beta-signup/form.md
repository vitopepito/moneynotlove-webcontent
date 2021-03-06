---
title: Sign up

form:
    name: signup

    fields:
        - name: vorname
          label: Vorname
          type: text
          autofocus: true
          validate:
            required: true

        - name: name
          label: Name
          type: text
          validate:
            required: true

        - name: email
          label: Email
          type: email
          validate:
            required: true

        - name: job
          label: Was machst du so?
          type: text
          validate:
            required: true

        - name: honeypot
          type: honeypot

        -
          name: g-recaptcha-response
          label: Zur Sicherheit
          type: captcha
          recaptcha_site_key: 6Le8HDwUAAAAAPbOaxTsRQe3GunNnTWQLu4veXTs
          recaptcha_not_validated: 'Captcha not valid!'
          validate:
            required: true


    buttons:
        - type: submit
          value: Submit
          classes: button button-large block--color-hard

    process:
        - captcha:
            recatpcha_secret: 6Le8HDwUAAAAAHdDz0qYMTslDcU3XBnzxBybvmBQ
        - email:
            from: "{{ form.value.email }}"
            subject: "[moneynotlove signup] {{ form.value.vorname|e }} {{ form.value.name|e }}"
            body: "{% include 'forms/data.html.twig' %}"
        - save:
            fileprefix: signup-
            dateformat: Ymd-His-u
            extension: txt
            body: "{% include 'forms/data.txt.twig' %}"
        - message: Merci! Wir werden uns bald bei dir melden.
        - display: thankyou
---

# Sign up

Wir nutzen Slack für die interne Kommunikation. Es ist ein einfacher Weg, mit allen im Kontakt zu bleiben und gibt die Möglichkeit, das ganze Netzwerk über etwas zu informieren. Wir freuen uns, falls du daran teilhaben möchtest. Jede Anmeldung wird von uns geprüft – wir sind aber offen für alle Kreativen, die sich austauschen möchten.

Für alle die es noch nicht kennen: [Slack](https://slack.com) ist eine kostenlose App auf mobile und desktop. Für lose Gruppen wie Unsere eignet Slack sich sehr gut, es wird aber auch von vielen Firmen genutzt.

---
