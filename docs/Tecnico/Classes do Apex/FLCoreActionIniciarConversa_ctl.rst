#######################
FLCoreActionIniciarConversa_ctl
#######################

saveData()
Assinatura
  public static String saveData(String pRecordId, String pParametroId, String pObjectLabel) 
Ação
  Salve o Contato ou Lead no ContatoFalae relacionado a um Parâmetro.
Exemplo

   .. code-block:: apex

      FLCoreActionIniciarConversa_ctl.saveData([SELECT Id FROM ContatoFalae__c][0].Id, [SELECT Id FROM ParametroFalae__c][0].Id, 'Contato do Falae');> 
