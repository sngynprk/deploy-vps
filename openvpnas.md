### OPENVPN ACCESS SERVER
```
apt update && apt -y install ca-certificates wget net-tools gnupg
wget https://as-repository.openvpn.net/as-repo-public.asc -qO /etc/apt/trusted.gpg.d/as-repository.asc
echo "deb [arch=amd64 signed-by=/etc/apt/trusted.gpg.d/as-repository.asc] http://as-repository.openvpn.net/as/debian bullseye main">/etc/apt/sources.list.d/openvpn-as-repo.list
apt update && apt -y install openvpn-as
```
> or Install Manually
```
apt update
apt install -y bridge-utils dmidecode iptables iproute2 libc6 libffi7 libgcc-s1 liblz4-1 liblzo2-2 libmariadb3 libpcap0.8 libssl1.1 libstdc++6 zlib1g libsasl2-2 libsqlite3-0 net-tools python3-pkg-resources python3-migrate python3-sqlalchemy python3-mysqldb python3-ldap3 sqlite3 python3-netaddr python3-arrow python3-lxml python3-openssl python3-incremental libxmlsec1 libxmlsec1-openssl python3-constantly python3-hyperlink python3-automat python3-service-identity python3-cffi python3-defusedxml
dpkg -i openvpn-as-bundled-clients-27.deb openvpn-as_2.11.3-af31575c-Debian11_amd64.deb
```
