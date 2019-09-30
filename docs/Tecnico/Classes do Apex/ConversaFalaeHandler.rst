#######################
ConversaFalaeHandler
#######################

Clásse responsável por gerenciar as ações relacionadas a Conversa Falae

executeTrigger()
Assinatura
  public static void executeTrigger(Map<Id, MensagemFalae__c> pMapOldRecord, List<MensagemFalae__c> pListRecord, Boolean pBeforeInsert, Boolean pBeforeUpdate, Boolean pAfterInsert, Boolean pAfterUpdate) 
Ação
  Atribui os parâmetro passados à variáveis da classe e executa o método que inicia os demais.
Exemplo

   .. code-block:: apex

      Map<Id, ConversaFalae__c> mapResult = new Map<Id, ConversaFalae__c>([SELECT Id, Name, ContatoFalae__r.Name, ContatoFalae__r.Numero__c, Status__c FROM ConversaFalae__c]);
      List<ConversaFalae__c> lstChanged = mapResult.values().deepClone(true, true, true);
      lstChanged[0].Status__c = 'Fechado';
      ConversaFalaeHandler.executeTrigger(mapResult, lstChanged, true, true, true, true); 

