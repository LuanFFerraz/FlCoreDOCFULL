#################
Process Builder
#################

Para acessar o Process Builder:

Entre em Configuração.

.. figure:: processbuilder1.png	
    :width: 270px
    :alt: Solidity logo
    :align: center
    
    Acessando as Configurações
    
Escreva process na busca rápida e clique em Process Builder.

Nele constará o seguinte fluxo ligado ao pacote

.. figure:: processbuilder2.png	
    :width: 550px
    :alt: Solidity logo
    :align: center
    
    Página de Process Builders

FL - Notificar Inbox (Conversa)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

O fluxo FL - Notificar Inbox (Conversa) é ligado ao objeto Conversa do Falae, nele é criado um registro do evento Whatsapp Inbox quando o campo Status da Conversa do Whatsapp sofre alguma alteração.

FL - Verificar DDI
~~~~~~~~~~~~~~~~~~~

O fluxo FL - Verificar DDI é ligado ao objeto Conversa do Falae, ele verifica se o Número possui ou não DDI, caso não possua, insere o DDI do Brasil.
 
FL - Mudar Relacionamento ao Converter
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

O fluxo FL - Mudar Relacionamento ao Converter é ligado ao objeto Lead, caso um Lead seja convertido um Contato é criado com o ID
