criar banco mysql com nome desejado

rodar as querys abaixo

```

CREATE TABLE `tbl_messages` (
  `id` int(11) NOT NULL,
  `username` text NOT NULL,
  `message` text NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;


ALTER TABLE `tbl_messages`
  ADD PRIMARY KEY (`id`);

ALTER TABLE `tbl_messages`
  MODIFY `id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=17;
COMMIT;

```

```
cd qwst-server
npm i
node server.js
Caso prefira deixar em daemon basta instalar o nodemon com npm i nodemon e rodar com nodemon server.js 
```

```
cd qwst-client
npm i
quasar dev
```

app basico com socket.io e insert no mysql.
