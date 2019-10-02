#######################
FLCoreExecutionAfter
#######################

onAtualizarMensagem()
Assinatura
  public void onAtualizarMensagem(Map<Id, MensagemFalae__c> pOldMapMensagemFalae, List<MensagemFalae__c> pNewListMensagemFalae) 
Ação
  Ao receber nova mensagem, insere-a no chat.
Exemplo

   .. code-block:: apex

      FLCoreExecutionAfter().onAtualizarMensagem(mapResultMensagem, lstChangedMensagem);
      Map<Id, MensagemFalae__c> mapResultMensagem = new Map<Id, MensagemFalae__c>([SELECT Id, Name, ConversaFalae__c, Corpo__c, Destino__c, Direcao__c, Origem__c, Status__c, APIComunicacao__c, CanalComunicacao__c FROM MensagemFalae__c]);
      List<MensagemFalae__c> lstChangedMensagem = mapResultMensagem.values().deepClone(true, true, true);
