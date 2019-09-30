########################
MensagemFalaeHandler
########################

executeTrigger()
----------------
Assinatura
  public static void executeTrigger(Map<Id, MensagemFalae__c> pMapOldRecord, List<MensagemFalae__c> pListRecord, 
                                    Boolean pBeforeInsert, Boolean pBeforeUpdate, Boolean pAfterInsert, Boolean pAfterUpdate)
Ação
  Integra as mensagens com o Salesforce/Servidor e dispara eventos de atualizações do Inbox do Falae e do Chat do Falae, cria,
  atualiza e relaciona as mensagens à Conversa do Falae
Exemplo

   .. code-block:: apex

      Map<Id, MensagemFalae__c> mapResult = new Map<Id, MensagemFalae__c>([
      SELECT 
            Id, 
            Name, 
            Corpo__c, 
            Direcao__c, 
            Destino__c, 
            Origem__c, 
            Status__c 
            FROM 
            MensagemFalae__c]);
      List<MensagemFalae__c> lstChanged = mapResult.values().deepClone(true, true, true);
      
      ``Antes da insercao``
      MensagemFalaeHandler.executeTrigger(mapResult, lstChanged, true, true, false, false);
      
      ``Depois da insercao``
      MensagemFalaeHandler.executeTrigger(mapResult, lstChanged, false, false, true, true);
