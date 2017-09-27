# Server RADIUS
1. nainstalovat
2. info

1.1. Instalace Virtual Box#
1.2. Instalace Linuxu ve Virtual Boxu#
1.3. Instalace+Konfigurace firewallu Radius#
    apt-get install freeradius#
    iptables -A INPUT -p tcp --dport 1812 -j ACCEPT#
    iptables -A INPUT -p tcp --dport 1813 -j ACCEPT#
    


















RADIUS je AAA protokol používaný pro přístup k síti nebo pro IP mobilitu. Může pracovat jak lokálně tak i v roamingu.

Mezi nejdůležitější vlastnosti patří jeho vysoká síťová bezpečnost, neboť transakce mezi klientem a RADIUS serverem je autentizována pomocí sdíleného tajemství, které není nikdy posíláno přes síť. Pouze uživatelská hesla jsou přes síť zasílána šifrovaně. Uživatelská jména, účtování apod. můžou byt odposlechnuta třetí osobou, protože tyto data nejsou přenášena šifrovaně.
