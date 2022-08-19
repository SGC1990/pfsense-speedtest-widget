# Speedtest dashboard widget for pfSense

## Install Manual Mode

To use this widget you will need to install the speedtest package

PFSense 2.4 or Older
```
pkg update ; pkg install -y py37-speedtest-cli
```
PFSense 2.5 or Newer
```
pkg update ; pkg install -y py38-speedtest-cli-2.1.3
```

Copy the widget file **speedtest.widget.php** to **/usr/local/www/widgets/widgets/** on your pfSense machine.

Install the widget on your dashboard.

## Install Automatic mode

Diagnostics - Command prompt

Run this command

```
fetch -q -o - https://raw.githubusercontent.com/aln-1/pfsense-speedtest-widget/master/autoconfigure.sh | sh
```
