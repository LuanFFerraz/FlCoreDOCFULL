#################
Acionadores do Apex
#################

ParametroFalae_aiu
-----------------------

O ParametroFalae_aiu é um acionador executado depois da inserção e depois da atualização do objeto Parâmetro Falae.

Nele apenas é chamado o método executeTrigger da classe ParametroFalaeHandler.

.. Important::
   Referências:
    Objeto Personalizado:
    `ParametroFalae`_

ConversaFalae_aiu
-----------------------
O ConversaFalae_aiu é um acionador executado depois da inserção e depois da atualização do objeto Conversa do Falae.

Nele apenas é chamado o método executeTrigger da classe ConversaFalaeHandler.

.. Important::
   Referências:
    Objeto Personalizado:
    `Conversa do Falae`_

ConversaFalae_biu
-----------------------

O ConversaFalae_biu é um acionador executado antes da inserção e antes da atualização do objeto Conversa do Falae.

Nele apenas é chamado o método executeTrigger da classe ConversaFalaeHandler.

.. Important::
   Referências:
    Objeto Personalizado:
    `ConversaFalae`_



MensagemFalae_aiu
-----------------------

O MensagemFalae_aiu é um acionador executado depois da inserção e depois da atualização do objeto Mensagem do Falae.

Nele apenas é chamado o método executeTrigger da classe MensagemFalaeHandler.

.. Important::
   Referências:
    Objeto Personalizado:
    `Mensagem do Falae`_



MensagemFalae_biu
-----------------------

O MensagemFalae_biu é um acionador executado antes da inserção e antes da atualização do objeto Mensagem do Falae.

Nele apenas é chamado o método executeTrigger da classe MensagemFalaeHandler.

.. Important::
   Referências:
    Objeto Personalizado:
    `Mensagem do Falae`_

Lead_aiud
-----------------------

O Lead_aiud é um acionador executado após inserção, alteração e exclusão de um Lead, este acionador executa o método executeTrigger da classe LeadHandler, passando o oldmap do Lead excluido.


.. Important::
   Referências:
    Objeto Personalizado:
    

ContatoFalae_biu
-----------------------

O Lead_aiud é um acionador executado após inserção, alteração e exclusão de um Lead, este acionador executa o método executeTrigger da classe ContatoFalaeHandler, passando o oldmap do ContatoFalae excluido.

.. Important::
   Referências:
    Objeto Personalizado:
    `Mensagem do Falae`_

.. _Conversa do Falae : https://whatsapp-teste.readthedocs.io/en/latest/Tecnico/Objetos.html
.. _Mensagem do Falae : https://whatsapp-teste.readthedocs.io/en/latest/Tecnico/Objetos.html
.. _ContatoFalae : https://whatsapp-teste.readthedocs.io/en/latest/Tecnico/Objetos.html
.. _ConversaFalae : https://whatsapp-teste.readthedocs.io/en/latest/Tecnico/Objetos.html
.. _ParametroFalae : https://whatsapp-teste.readthedocs.io/en/latest/Tecnico/Objetos.html
.. _MensagemFalae : https://whatsapp-teste.readthedocs.io/en/latest/Tecnico/Objetos.html
