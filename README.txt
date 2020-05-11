Formatting matters in this script. I recommend you use the example CSV "User_List.csv" as a template and enter your own data
into it to avoid having to change to code. In case you don't feel like restructuring your csv it should be enough to change
the headers as shown below.

Emails should be stored in a column named "E-Mail".

Usernames are constructed by combining the columns "First name" and "User Number".

In case you have multiple people sharing an e-mail address/account, you can set a conjunction that the code will format out
of usernames. The conjunction is set to " and " by default.

The list of groups a user is in should be stored in a column named "Groups".

Each item in the list of groups should be separate by a comma and a space, or ", ". The character case matters here, so be 
sure to double check whether the spelling is consistent across all users.

The formatting for the e-mail body is not very pretty. The actual message is bilingual (German/English) and will look like
this by default:

Ein Nextcloud Account wurde für dich erstellt! Du kannst dich unter {example.url.com} mit den folgenden Daten einloggen:
Username: {Username}
Kennwort: {Password}
Das Kennwort wurde nur für die erste Benutzung generiert. Bitte log dich ein und ändere das Passwort.

---

A Nextcloud account has been created for you. You can log in at {example.url.com} using the following credentials:
Username: {Username}
Password: {Password}
The password is meant to be used only once, the first time you log in. Please change it as soon as possible.

I am not sure whether HTML can be formatted the same way as an fstring in Python and was satisfied with what I already had,
but it shouldn't be difficult to make the text prettier and easier to edit.
