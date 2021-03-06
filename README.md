# m17n-db-ipa-x-sampa

## ipa-x-sampa input method for IPA phonetic symbols for m17n-db

## Information about the IPA X-SAMPA

See: https://en.wikipedia.org/wiki/X-SAMPA

## Mapping

See the contents of the ipa-x-sampa.mim file, it is a rather simple table

## Dependencies

You will need to install

* ibus-m17n
* Any Unicode font supporting the IPA symbols

## Installation

``` bash
$ mkdir -p ~/.m17n.d/
$ cp ipa-x-sampa.mim ~/.m17n.d/
$ mkdir -p ~/.m17n.d/icons/
$ cp icons/ipa-x-sampa.png ~/.m17n.d/icons/
$ ibus restart
```

Now ibus should list the newly added input method:

``` bash
$ ibus list-engine | grep sampa
  m17n:t:ipa-x-sampa - ipa-x-sampa (m17n)
```

## Adding the input method to your desktop:

### If you are  using Gnome3:

Open the input method settings in the gnome-control-center. Either from
the gnome panel by clicking on the icon showing a wrench and a
screwdriver. Then the gnome-control-center opens. Click on the flag
to go to the regional settings. Or in newer versions of Gnome you will
find it in the keyboard settings.

In the input method settings dialog, click on the “+” button at the lower
left corner of the dialog to add an input method. In the search dialog
which opens, click on the three vertical dots at the bottom.  Enter
"sampa" into the search field. Click on “Other”.  Select
“Other (ipa-x-sampa (m17n))” and click on the “Add” button.

### If you are not using Gnome3:

Start ibus-setup and add the “sipa-x-sampa (m17n)” input method (Search
for “other”). Don’t use ibus-setup if you are using Gnome3, it
does not work for Gnome3!
