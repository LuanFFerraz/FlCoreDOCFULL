#######################
ChatContent
#######################

ChatContent()
~~~~~~~~~~~~~~
Assinatura
  public ChatContent(List<MensagemFalae__c> pListMensagemFl) 
Ação
  Adiciona a mensagem no chat, verificando se há ou não sessão prévia para agrupar mensagens pela data.
Exemplo

   .. code-block:: apex

      ChatContent.ChatContent();
      
      
isSameSection()
~~~~~~~~~~~~~~
Assinatura
  public Boolean isSameSection(SectionConversa pSectionConversa, MensagemFalae__c pMensagemFl)
Ação
  Verifica se a mensagem deve ser mostrada na mesma sessão ou não, dado a data de criação.
Exemplo

   .. code-block:: apex

      ChatContent.isSameSection();
            
getLastMensagemFl()
~~~~~~~~~~~~~~
Assinatura
  public MensagemFalae__c getLastMensagemFl(SectionConversa pSectionConversa)
Ação
  Retorna a ultima mensagem da sessão.
Exemplo

   .. code-block:: apex

      ChatContent.getLastMensagemFl();
      
      
      
      
