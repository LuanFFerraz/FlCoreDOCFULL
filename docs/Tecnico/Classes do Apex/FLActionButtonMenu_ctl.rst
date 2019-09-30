#######################
FLActionButtonMenu_ctl
#######################

getIsClassic()
~~~~~~~~~~~~~~~~~~
Assinatura
  public static Boolean getIsClassic() 
Ação
  Retorna true ou false caso o modo do SalesForce seja o Classic ou não.
Exemplo

   .. code-block:: apex

      FLActionButtonMenu_ctl.getIsClassic();
      
getFLActions()
~~~~~~~~~~~~~~~~~~
Assinatura
  public static List<AcaoInbox> getFLActions(Object pRecordValue, String pTipoAcao) 
Ação
  Retorna informações dos registros do metadado AcaoFalae.
Exemplo

   .. code-block:: apex

      FLActionButtonMenu_ctl.getFLActions(new ConversaFalae__c(), 'Chat');
      
      
doExecuteAction()
~~~~~~~~~~~~~~~~~~
Assinatura
  public static void doExecuteAction(AcaoFalae__mdt pAcaoFalae, Object pRecordValue) 
Ação
  Executa o método doExecuteFlActionda classe FLActionHandler.
Exemplo

   .. code-block:: apex

      FLActionButtonMenu_ctl.doExecuteAction(lstResult[0].action, new ConversaFalae__c());
      
