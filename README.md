# password-manager

A GnuPG-based password manager. Two commands are provided, one to generate
random passwords and one for managing passwords.

`random-password` will generate a random password.

`password --key <gpg-key> -s <name>` will prompt for a password, encrypt
using the supplied gpg-key and save under the specified name (in
`~/.password_manager`).

`password <text>` will search for a previously added password file matching the
string, prompt for the gpg password and display the password.
