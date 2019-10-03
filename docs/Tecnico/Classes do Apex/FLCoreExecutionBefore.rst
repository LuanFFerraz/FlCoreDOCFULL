#####################
FLCoreExecutionBefore
#####################

onInicioConversa()
~~~~~~~~~~~~~~~~~~~~ 
Assinatura
  public void onInicioConversa(List<ConversaFalae__c> pListConversaFalae)
Ação
  Implementação da FLActionInterface, não está sendo utilizado.    

onFimConversa()
~~~~~~~~~~~~~~~~~~~~
Assinatura
  public void onFimConversa(List<ConversaFalae__c> pListConversaFalae)
Ação
  Implementação da FLActionInterface, não está sendo utilizado.   
  
onEntradaMensagem()
~~~~~~~~~~~~~~~~~~~~
Assinatura
  public void onEntradaMensagem(List<MensagemFalae__c> pListMensagemFalae)
Ação
  Cria uma lista das mensagens em que o canal seja Whatsapp e manda-as como parâmetro para o método doRelacionarConversaByNumero.
Exemplo

   .. code-block:: apex
        List<MensagemFalae__c> lstChangedMensagem = mapResultMensagem.values().deepClone(true, true, true);
        new FLCoreExecutionBefore().onEntradaMensagem(lstChangedMensagem);
        
onAtualizarMensagem()
~~~~~~~~~~~~~~~~~~~~
Assinatura
  public void onEntradaMensagem(List<MensagemFalae__c> pListMensagemFalae)
Ação
  Implementação da FLActionInterface, não está sendo utilizado.

   
onClick()
~~~~~~~~~~~~~~~~~~~~
Assinatura
  public void onClick(Object pRecordValue)
Ação
  Implementação da FLActionInterface, não está sendo utilizado.
Exemplo

   .. code-block:: apex

      FLCoreExecutionBefore().onClick(lstChangedMensagem[0]); 
   
isDisabled()
~~~~~~~~~~~~~~~~~~~~
Assinatura
  public Boolean isDisabled(Object pConversaFalae) 
Ação
  Retorna false.
Exemplo

   .. code-block:: apex

      FLCoreExecutionBefore().onClick(lstChangedMensagem[0]);





