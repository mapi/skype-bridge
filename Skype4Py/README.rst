========
Skype4Py
========

Skype Lingr Gateway
===================

VNC�����Ф�Skype�ε�ư
----------------------

::

  sudo su - www-data
  LANG=C XAUTHORITY=/var/www/.Xauthority /usr/bin/dbus-launch tightvncserver :32
  LANG=C XAUTHORITY=/var/www/.Xauthority DISPLAY=:32 nohup /usr/bin/skype

�ǡ�����ư��³����
----------------------

::

  sudo su - 
  while :; do date;sudo -u www-data sh -c 'XAUTHORITY=/var/www/.Xauthority DISPLAY=:32 python skype-lingr.py';date; done

����åȥ롼��μ��̻Ҥ�Ĵ�٤�
------------------------------

::

  sudo -u www-data  XAUTHORITY=/var/www/.Xauthority DISPLAY=:32 python chat_list.py


