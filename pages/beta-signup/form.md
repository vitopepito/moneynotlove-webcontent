---
title: Sign up

form:
    name: signup

    fields:
        - name: vorname
          label: Vorname
          type: text
          validate:
            required: true

        - name: name
          label: Name
          type: text
          validate:
            required: true

        - name: email
          label: Email
          placeholder: Enter your email address
          type: email
          validate:
            required: true

        - name: job
          label: Was machst du so?
          placeholder: Enter your message
          type: text
          validate:
            required: true


    buttons:
        - type: submit
          value: Submit

    process:
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

Wir nutzen Slack für die interne Kommunikation. Es ist ein einfacher Weg, mit allen im Kontakt zu bleiben und gibt die Möglichkeit, die ganze Gruppe über etwas zu informieren. Wir freuen uns, falls du daran teilhaben möchtest. Jede Anmeldung wird von uns geprüft – am Liebsten wäre uns sogar, dich einmal persönlich kennenzulernen.
