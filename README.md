# newsbeuter_dotfiles
my newsletter CONFIG~! enjoy

features an awesome script for `GetPocket.com` integration, check `/scripts` and authorise your email to send to `add@getpocket.com` in your `GetPocket` account

run `leader + p` think "macro-pocket-this"

prerequisite: `ssmtp` to run a successful `$ sendmail -s "subject" "recipient@server.com" < /path/to/txt_to_send`

## install smmpt
`$ sudo apt-get install ssmtp`

`$ sudo nano /etc/ssmtp/ssmtp.conf`

contents of ssmtp.conf to:
```
root=username@gmail.com
mailhub=smtp.gmail.com:465
rewriteDomain=gmail.com
AuthUser=usernameNoGmailSuffix
AuthPass=supersecretpassword
FromLineOverride=YES
UseTLS=YES
```

`$ sudo cat /var/log/mail.log`
