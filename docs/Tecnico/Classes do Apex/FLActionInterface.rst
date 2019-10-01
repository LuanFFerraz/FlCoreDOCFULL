#################
FLActionInterface
#################

onInicioConversa()
~~~~~~~~~~~~~~~~~~~~
  Método para ser executado no início de uma conversa nas classes que a implementam.
Assinatura
  void onInicioConversa(List<ConversaFalae__c> pListConversaFalae)
Valor retornado
  Sem retorno.
Exemplo

   .. code-block:: apex

      Map<Id, ConversaFalae__c> mapResult = new Map<Id, ConversaFalae__c>([SELECT Id, Name, ContatoFalae__r.Name, ContatoFalae__r.Numero__c, Status__c FROM ConversaFalae__c]);
      Map<Id, MensagemFalae__c> mapResultMensagem = new Map<Id, MensagemFalae__c>([SELECT Id, Name, ConversaFalae__c, Corpo__c, Destino__c, Direcao__c, Origem__c, Status__c FROM MensagemFalae__c]);
      List<ConversaFalae__c> lstChanged = mapResult.values().deepClone(true, true, true);
      List<MensagemFalae__c> lstChangedMensagem = mapResultMensagem.values().deepClone(true, true, true);
      new WACoreExecutionAfter().onInicioConversa(lstChanged);
      
onFimConversa()
~~~~~~~~~~~~~~~~~~~~
  Método para ser executado no fim de uma conversa nas classes que a implementam.
Assinatura
  void onFimConversa(List<ConversaFalae__c> pListConversaFalae)
Valor retornado
  Sem retorno.
Exemplo

   .. code-block:: apex

      Map<Id, ConversaFalae__c> mapResult = new Map<Id, ConversaFalae__c>([SELECT Id, Name, ContatoFalae__r.Name, ContatoFalae__r.Numero__c, Status__c FROM ConversaFalae__c]);
      Map<Id, MensagemFalae__c> mapResultMensagem = new Map<Id, MensagemFalae__c>([SELECT Id, Name, ConversaFalae__c, Corpo__c, Destino__c, Direcao__c, Origem__c, Status__c FROM MensagemFalae__c]);
      List<ConversaFalae__c> lstChanged = mapResult.values().deepClone(true, true, true);
      List<MensagemFalae__c> lstChangedMensagem = mapResultMensagem.values().deepClone(true, true, true);
      new WACoreExecutionAfter().onFimConversa(lstChanged);
        
onEntradaMensagem()
~~~~~~~~~~~~~~~~~~~~
  Método para ser executado ao chegar uma nova mensagem nas classes que a implementam.
Assinatura
  void onEntradaMensagem(List<MensagemFalae__c> pListMensagemFalae)
Valor retornado
  Sem retorno.
Exemplo

   .. code-block:: apex

      Map<Id, ConversaFalae__c> mapResult = new Map<Id, ConversaFalae__c>([SELECT Id, Name, ContatoFalae__r.Name, ContatoFalae__r.Numero__c, Status__c FROM ConversaFalae__c]);
      Map<Id, MensagemFalae__c> mapResultMensagem = new Map<Id, MensagemFalae__c>([SELECT Id, Name, ConversaFalae__c, Corpo__c, Destino__c, Direcao__c, Origem__c, Status__c FROM MensagemFalae__c]);
      List<ConversaFalae__c> lstChanged = mapResult.values().deepClone(true, true, true);
      List<MensagemFalae__c> lstChangedMensagem = mapResultMensagem.values().deepClone(true, true, true);
      new WACoreExecutionAfter().onEntradaMensagem(lstChangedMensagem);      
        
onAtualizarMensagem()
~~~~~~~~~~~~~~~~~~~~
  Método para ser executado ao chegar uma nova mensagem nas classes que a implementam.
Assinatura
  void onAtualizarMensagem(Map<Id, MensagemFalae__c> pOldMapMensagemFalae, List<MensagemFalae__c> pNewListMensagemFalae);
Valor retornado
  Sem retorno.
Exemplo

   .. code-block:: apex

      Map<Id, ConversaFalae__c> mapResult = new Map<Id, ConversaFalae__c>([SELECT Id, Name, ContatoFalae__r.Name, ContatoFalae__r.Numero__c, Status__c FROM ConversaFalae__c]);
      Map<Id, MensagemFalae__c> mapResultMensagem = new Map<Id, MensagemFalae__c>([SELECT Id, Name, ConversaFalae__c, Corpo__c, Destino__c, Direcao__c, Origem__c, Status__c FROM MensagemFalae__c]);
      List<ConversaFalae__c> lstChanged = mapResult.values().deepClone(true, true, true);
      List<MensagemFalae__c> lstChangedMensagem = mapResultMensagem.values().deepClone(true, true, true);
      new WACoreExecutionAfter().onEntradaMensagem(lstChangedMensagem);      
        
isDisabled()
~~~~~~~~~~~~~~~~~~~~
  Método para ser executado ao chegar uma nova mensagem nas classes que a implementam.
Assinatura
  Boolean isDisabled(Object pRecordValue);
Valor retornado
  Sem retorno.
Exemplo

   .. code-block:: apex

      Map<Id, ConversaFalae__c> mapResult = new Map<Id, ConversaFalae__c>([SELECT Id, Name, ContatoFalae__r.Name, ContatoFalae__r.Numero__c, Status__c FROM ConversaFalae__c]);
      Map<Id, MensagemFalae__c> mapResultMensagem = new Map<Id, MensagemFalae__c>([SELECT Id, Name, ConversaFalae__c, Corpo__c, Destino__c, Direcao__c, Origem__c, Status__c FROM MensagemFalae__c]);
      List<ConversaFalae__c> lstChanged = mapResult.values().deepClone(true, true, true);
      List<MensagemFalae__c> lstChangedMensagem = mapResultMensagem.values().deepClone(true, true, true);
      new WACoreExecutionAfter().onEntradaMensagem(lstChangedMensagem);    
