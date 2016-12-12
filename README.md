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

	cambrian-balance <member-number> -s

You will be prompted to enter your password and answer one of your "secret
questions". It'll remember the password, and store the cookies so it won't need
any more answers either!

### After that

	cambrian-balance

If you change you're password just add `-s` and it'll prompt you for a new one.
If you want to check a different account, just type `cambrian-balance
<different-member-number>` and it'll show you that one instead. add `-s` to
replace the old member number in the pasword file.
