#####################
FLCoreExecutionBefore
#####################

onInicioConversa()
~~~~~~~~~~~~~~~~~~~~
  Implementação da FLActionInterface, não está sendo utilizado.
Assinatura
  public void onInicioConversa(List<ConversaFalae__c> pListConversaFalae)
Valor retornado
  Sem retorno.
Exemplo

   .. code-block:: apex

      Map<Id, ConversaFalae__c> mapResult = new Map<Id, ConversaFalae__c>([SELECT Id, Name, ContatoFalae__r.Name, ContatoFalae__r.Numero__c, Status__c FROM ConversaFalae__c]);
      Map<Id, MensagemFalae__c> mapResultMensagem = new Map<Id, MensagemFalae__c>([SELECT Id, Name, Corpo__c, Destino__c, Direcao__c, NomeOrigem__c, Origem__c, Status__c FROM MensagemFalae__c]);
      List<ConversaFalae__c> lstChanged = mapResult.values().deepClone(true, true, true);
      List<MensagemFalae__c> lstChangedMensagem = mapResultMensagem.values().deepClone(true, true, true);
      lstChangedMensagem[0].ConversaFalae__c = null;
      lstChangedMensagem[0].Destino__c = '22222222';
      lstChangedMensagem[0].Origem__c = '22222222';
      new FLCoreExecutionBefore().onInicioConversa(lstChanged);

onFimConversa()
~~~~~~~~~~~~~~~~~~~~
  Implementação da FLActionInterface, não está sendo utilizado.
Assinatura
  public void onFimConversa(List<ConversaFalae__c> pListConversaFalae)
Valor retornado
  Sem retorno.
Exemplo

   .. code-block:: apex

      Map<Id, ConversaFalae__c> mapResult = new Map<Id, ConversaFalae__c>([SELECT Id, Name, ContatoFalae__r.Name, ContatoFalae__r.Numero__c, Status__c FROM ConversaFalae__c]);
      Map<Id, MensagemFalae__c> mapResultMensagem = new Map<Id, MensagemFalae__c>([SELECT Id, Name, Corpo__c, Destino__c, Direcao__c, NomeOrigem__c, Origem__c, Status__c FROM MensagemFalae__c]);
      List<ConversaFalae__c> lstChanged = mapResult.values().deepClone(true, true, true);
      List<MensagemFalae__c> lstChangedMensagem = mapResultMensagem.values().deepClone(true, true, true);
      lstChangedMensagem[0].ConversaFalae__c = null;
      lstChangedMensagem[0].Destino__c = '22222222';
      lstChangedMensagem[0].Origem__c = '22222222';
      new FLCoreExecutionBefore().onFimConversa(lstChanged);
  
onEntradaMensagem()
~~~~~~~~~~~~~~~~~~~~
  Implementação da FLActionInterface, executa outros métodos privados da classe.
Assinatura
  public void onEntradaMensagem(List<MensagemFalae__c> pListMensagemFalae)
Valor retornado
  Sem retorno.
Exemplo

   .. code-block:: apex

      Map<Id, ConversaFalae__c> mapResult = new Map<Id, ConversaFalae__c>([SELECT Id, Name, ContatoFalae__r.Name, ContatoFalae__r.Numero__c, Status__c FROM ConversaFalae__c]);
      Map<Id, MensagemFalae__c> mapResultMensagem = new Map<Id, MensagemFalae__c>([SELECT Id, Name, Corpo__c, Destino__c, Direcao__c, NomeOrigem__c, Origem__c, Status__c FROM MensagemFalae__c]);
      List<ConversaFalae__c> lstChanged = mapResult.values().deepClone(true, true, true);
      List<MensagemFalae__c> lstChangedMensagem = mapResultMensagem.values().deepClone(true, true, true);
      lstChangedMensagem[0].ConversaFalae__c = null;
      lstChangedMensagem[0].Destino__c = '22222222';
      lstChangedMensagem[0].Origem__c = '22222222';
      new FLCoreExecutionBefore().onEntradaMensagem(lstChangedMensagem);
   
onEntradaMensagem()
~~~~~~~~~~~~~~~~~~~~
  Implementação da FLActionInterface, executa outros métodos privados da classe.
Assinatura
  public void onEntradaMensagem(List<MensagemFalae__c> pListMensagemFalae)
Valor retornado
  Sem retorno.
Exemplo

   .. code-block:: apex

      Map<Id, ConversaFalae__c> 
