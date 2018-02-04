# wallet_definitiva
Wallet Blockchain in PHP

Contiene 2 wallets: 

1. Wallet: Es la wallet en PHP con llamadas cURL a la API

2. master_nodejs: Es la wallet como su nombre lo indica, hecha con nodejs y jade en vez de HTML. Utiliza request y bootstrap.

3. wallet: Es la base de datos creada para almacenar datos importantes para la corrida de las wallets.
  
  3.1 Tablas: a) crear_billetera: Esta es la tabla para manejar las sesiones. Tiene 5 campos: -guid que viene de la api
                                                                                              
                                                                                              -email con el que se inicia la sesión
                                                                                              
                                                                                              -address que es la dirección principal
                                                                                              
                                                                                              -label que viene de la API
                                                                                              
                                                                                              -password que es la clave para acceder
              
              b) direcciones: Esta es la tabla que almacena todas las direcciones de la cuenta, sobre todo las secundarias.
              tiene 3 campos: -id_direccion: Que es el id de la dirección almacenada.
                              
                              -guid que viene de la API
                              
                              -new_address que es la dirección, bien sea principal(para tener también un respaldo de la misma en la tabla)                               o nueva creada.
