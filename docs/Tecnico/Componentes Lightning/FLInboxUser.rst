#################
FLInboxUser
#################
Funcionalidade
~~~~~~~~~~

O componente FLInboxUser serve pra pegar a instancia do usuario.

Atributos:
~~~~~~~~~~~~

+------------------------+-----------------------+
|  Name                  | Type                  |
+========================+=======================+
| usuario                | User                  |
+------------------------+-----------------------+
| isVisualforceView      | Boolean               |
+------------------------+-----------------------+

Chamada
~~~~~~~~~~

<aura:attribute name="usuarioExemplo" type="User" />

<flcore:FLInboxUser usuario="usuarioExemplo" 
                    isVisualforceView="false"/>
