# Saleor Admin Email Templates

A set of [MJML](https://mjml.io/) templates you can use to customize Saleor's admin emails.

NOTE: Saleor uses [Handlebars](https://handlebarsjs.com/) as a templating language, so both MJML templates and resulting HTML will be in that format.

## Saleor Admin Emails
* Set Password Email [Current Preview](https://htmlpreview.github.io/?https://github.com/saleor/saleor-admin-email-templates/blob/main/build/set_password.html)
* Reset Password Email [Current Preview](https://htmlpreview.github.io/?https://github.com/saleor/saleor-admin-email-templates/blob/main/build/password_reset.html)
* Staff Order Confirmation Email [Current Preview](https://htmlpreview.github.io/?https://github.com/saleor/saleor-admin-email-templates/blob/main/build/staff_confirm_order.html)
* Export Successful Email [Current Preview](https://htmlpreview.github.io/?https://github.com/saleor/saleor-admin-email-templates/blob/main/build/export_success.html)
* Export Failed Email [Current Preview](https://htmlpreview.github.io/?https://github.com/saleor/saleor-admin-email-templates/blob/main/build/export_failed.html)


## (MJML) installation and usage

```shell
npm install
```

To compile the emails run:

```shell
npm run build-emails
```


## Updating Saleor admin templates via Dashboard

1. You can compile the required MJML template(s) to HTML using our `build-emails` formula as described in Installation section or by using `mjml` tool directly:
```shell
mjml source/staff_confirm_order.mjml -o compiled/
```
2. Paste the resulting HTML to the relevant field in `Configuration → Plugins → Admin emails` section of Saleor Dashboard.
