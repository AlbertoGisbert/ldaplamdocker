 ldapsearch -x  -b "dc=example,dc=org" -D "cn=admin,dc=example,dc=org" -W
ldapadd -c -x -w "admin" -D "cn=admin,dc=example,dc=org"  -f bootstrap.ldif
docker-compose up -d
docker-compose down
nano bootstrap.ldif






