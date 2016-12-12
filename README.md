# cambrian-balance

Get your balance on your Cambrian Credit Union Online Banking account, because
their website is just so terrible.

## Installation

You need `Python 3.x` with the `Requests` and `CSSSelect` libraries. You almost
certainly have Python already, so just:

- Generic: `pip install requests cssselect`.
- Arch: `sudo pacman -S python-requests python-cssselect`
- Ubuntu: `sudo apt install python3-requests python3-cssselect`

And put it somewhere in your `$PATH`:

	sudo cp cambrian-balance /usr/local/bin

## Usage

### First time

	cambrian-balance <username> -s

### After that

	cambrian-balance

It'll prompt you for your password and a secret question the first time. Type
it in. Then it'll tell you your balance on your accounts(s). It saves the
password, and cookies so it won't have to prompt for the security question
every time either.

You can add in `-s` and it'll remember your username pasword for you for next
time (stored in `~/.cambrian_auth`), or overwrite an existing one if you change
your password.
