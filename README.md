# Mutt Configuration Files

## Overview

I still love using command line based tools.  I especially like using
  [_Mutt_](http://www.mutt.org/) for reading mail.  I am use a
  [_Vim_](http://www.vim.org) user and the integration of
  [_Mutt_](http://www.mutt.org/) and [_Vim_](http://www.vim.org) works
  well for me.

## Customization

I have a top level _muttrc_ file usually named _muttrc-personal_.  This
  contains the configuration for my home e-mail setup.  I typically also
  create a second _muttrc-work_ file which I use for work related email.

Depending upon the site that I am working at I use a simple symbolic link
  from *~/.mutt/muttrc* to the file that I am primarily use instead of
  utilizing mutt's -F flag.  I keep all of my configuration file in
  *~.mutt/* which mutt searches by default on startup for a _muttrc_ file.

All of the top level _muttrc_ files that I have include generic Mutt
  configuration files which I use to setup the look and feel that I
  like.  This allows me to flip in different configurations easily,
  especially if I want different environment for home or work.

* **_.mutt/muttrc-personal_**

  This file is the startup file for _Mutt_.  I use this to set the mail
  account specific settings such as the user name and _IMAP_ server, etc.
  This file then includes the files below for customization of _Mutt_ for
  the specific environment in which I am working.

* **_.mutt/mutt-colors_**

  This file contains the color settings to be used in different parts of
  _Mutt_ such as the message index and the message viewer, etc.  For
  instance different fields of an email header can be colored differently.

* **_.mutt/mutt-customization_**

  This file contains different macros and key bindings that I typically
  use.

* **_.mutt/mutt-settings_**

  This file contains the generic settings that _Mutt_ provides such as the
  editor to use for writing email as well as the sort order for indexing
  emails in various folders, etc.

* **_.mutt/mutt-settings-crypto_**

  This file contains the settings to be used for signed and encrypted
  emails.  These are integrated with [_GnuPG_](https://gnupg.org/).  These
  are split out from the general _mutt-settings_ file simply because there
  are quite a few configurables here.
