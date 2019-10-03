#######################
FLCoreExecutionFecharConversa
#######################

onInicioConversa()
~~~~~~~~~~~~~~
Assinatura
  public void onInicioConversa(List<ConversaFalae__c> pListConversaFalae)
Ação
  Implementa FLActionInterface

onFimConversa()
~~~~~~~~~~~~~~
Assinatura
  public void onFimConversa(List<ConversaFalae__c> pListConversaFalae) 
Ação
  Implementa FLActionInterface

onEntradaMensagem()
~~~~~~~~~~~~~~
Assinatura
  public void onEntradaMensagem(List<ConversaFalae__c> pListConversaFalae)
Ação
  Implementa FLActionInterface

onClick()
~~~~~~~~~~~~~~
Assinatura
  public void onClick(Object pConversaFalae) 
Ação
  Executa o método fecharConversa
Exemplo

   .. code-block:: apex

      FLCoreExecutionFecharConversa.onClick('a023i000004qAnEAAU');
      
onEntradaMensagem()
~~~~~~~~~~~~~~
Assinatura
  public void onAtualizarMensagem(Map<Id, MensagemFalae__c> pOldMapMensagemFalae, List<MensagemFalae__c> pNewListMensagemFalae)
Ação
  Implementa FLActionInterface
      
isDisabled()
~~~~~~~~~~~~~~
Assinatura
  public Boolean isDisabled(Object pConversaFalae)
Ação
  Retorna false
Exemplo

   .. code-block:: apex

      FLCoreExecutionFecharConversa.isDisabled('a023i000004qAnEAAU');
      
      
      
      
      
