# README

openssl req -x509 -sha256 -nodes -newkey rsa:2048 -days 365 -keyout localhost.key -out localhost.crt
 
rails s -b 'ssl://0.0.0.0:3000?key=./localhost.key&cert=./localhost.crt'
