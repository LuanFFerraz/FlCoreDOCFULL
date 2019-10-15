#################
FLInboxChat
#################

Funcionalidade
~~~~~~~~~~

O componente FLInboxChat serve para mostrar a o inbox das conversas do chat.


Atributos:
~~~~~~~~~~~~

+------------------------+-----------------------+
|  name                  | Tipo                  |
+========================+=======================+
| soql-filter-conversa   | String                |
+------------------------+-----------------------+
| IsVisualForceView      | Boolean               |
+------------------------+-----------------------+
| mapNavigation          | Boolean               |
+------------------------+-----------------------+

Chamada
~~~~~~~~~~
<c:FLInboxChat soql-filter-conversa="WHERE flcore__Status__c = 'Exemplo'" isVisualforceView="false" mapNavigation="false"/>
