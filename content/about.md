---
Title: About
Description: Lists all techniques used.
---

About
==========================

I kmom02 har jag lekt lite med stylingen. Jag skapade ett färgtema som är tänkt att användas och byggas på längre in i kursen.

![color theme](image/color-theme.png "Color Theme")

Jag har hämtat fina fonter ifrån Google Fonts och i min SASS-kod har jag lekt med tekniker som variabler:

    $links-color: #A7B3DE;
    $links-alternative-color: #EC8970;
    $titles: 'Gabarito', sans-serif;
    $text: 'Space Mono', monospace;

Och nästalade regler:

    .footer {
        a {
            text-decoration: none;
            color: $font-color;
        }

        p {
            text-transform: uppercase;
        }
    }

I footern har jag även lekt lite med css-grid och flex, men stannade på flex än så länge.
