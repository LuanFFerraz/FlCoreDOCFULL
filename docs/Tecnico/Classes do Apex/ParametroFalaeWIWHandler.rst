#################
ParametroFalaeWIWHandler
#################


executeTrigger()
---------------

Assinatura
    public static void executeTrigger(Map<Id, ParametroFalae__c> pMapOldRecord, List<ParametroFalae__c> pListRecord, 
                                      Boolean pBeforeInsert, Boolean pBeforeUpdate, Boolean pAfterInsert, Boolean pAfterUpdate)
Ação
    É responável por registrar um novo número de Parâmetro Falae do tipo **Whatsapp InpulsoWeb** 
Exemplo

   .. code-block:: apex

      insert new Parametro__c(
            Ativo__c = true,
            Celular__c = pNumero,
            RecordTypeId = '0123i000000UGAuAAO',
            SenhaSalesforce__c = '123123123',
            UsuarioSalesforce__c = 'teste@teste.com'
      );
