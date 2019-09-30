#################
ContatoFalaeHandler
#################
Clásse responsável por gerenciar as ações relacionadas ao Contato Falae

executeTrigger()
---------------

Assinatura
    public static void executeTrigger(Map<Id, ContatoFalae__c> pMapOldRecord, List<ContatoFalae__c> pListRecord, 
                                        Boolean pBeforeInsert, Boolean pBeforeUpdate, Boolean pAfterInsert, Boolean pAfterUpdate) 
Retorno
    Método responsável por iniciar os métodos privados da classe. 
Exemplo

   .. code-block:: apex

      ContatoFalaeHandler.executeTrigger(mapResult, lstChanged, true, true, true, true);      
      
   
