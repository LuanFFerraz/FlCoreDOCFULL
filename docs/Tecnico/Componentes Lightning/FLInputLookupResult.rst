#################
FLInputLookupResult
#################
Funcionalidade
~~~~~~~~~~

O componente FLInboxUser serve para mostrar a barra de pesquisa que reside dentro do modal para o modo de exibição Classic.


Atributos:
~~~~~~~~~~~~

+------------------------+-----------------------+
|  Name                  | Type                  |
+========================+=======================+
| oRecord                | sObject               |
+------------------------+-----------------------+
| IconName               | string                |
+------------------------+-----------------------+

Chamada
~~~~~~~~~~

<aura:attribute name="caso" type="Case"/>

<flcore:FLInputLookupResult oRecord="{!v.caso}" IconName="utility:case"/>

