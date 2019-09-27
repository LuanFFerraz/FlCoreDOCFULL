#################
ParametroFalaeWIMHandler
#################


executeTrigger()
---------------

Assinatura
    public static void executeTrigger(Map<Id, ParametroFalae__c> pMapOldRecord, List<ParametroFalae__c> pListRecord, 
                                        Boolean pBeforeInsert, Boolean pBeforeUpdate, Boolean pAfterInsert, Boolean pAfterUpdate) 
Retorno
    Método Void, responsável por passar os parâmetros da assinatura e iniciar a classe
Exemplo

   .. code-block:: apex

      SendWhatsappMessage.doEnviarMensagem('551399999999', '5513997733761', '', 'teste', 'a011U00000Occ0WQAR');      
      
   
