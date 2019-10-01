#################
FLInboxChat_ctl
#################

getIsClassic()
---------------

Assinatura
    @AuraEnabled
    public static Boolean getIsClassic()
Ação
    Retorna se a organização é classic ou não.
Valor retornado
    Tipo: Boolean    
Exemplo

   .. code-block:: apex

      FLInboxChat_ctl.getIsClassic();

getRefreshValue()
---------------

Assinatura
    @AuraEnabled
    public static Decimal getRefreshValue() 
Ação
    Retorna o tempo oara atualização do componente em milisegundos.
Valor retornado
    Tipo: Decimal
Exemplo

   .. code-block:: apex

      FLInboxChat_ctl.getRefreshValue();

getConversaFalae()
---------------

Assinatura
    @AuraEnabled
    public static List<ParametroInboxEntity> getConversaFalae(String pSoqlFilter)
Ação
    Retorna uma lista de uma classe contendo os parametros e suas conversas relacionadas.
Valor Retornado
    Tipo: List<**ParametroInboxEntity**>
Exemplo

   .. code-block:: apex

      FLInboxChat_ctl.getConversaFalae('');

setSeenConversa()
---------------

Assinatura
    @AuraEnabled
    public static void setSeenConversa(String pConversaFalaeId)
Ação
    Atualiza o campo Status__c das mensagens para "lido"
Exemplo

   .. code-block:: apex

      List<ConversaFalae__c> lstChanged = new List<ConversaFalae__c> lstChanged([
                                                                                SELECT 
                                                                                        Id
                                                                                FROM 
                                                                                        ConversaFalae__c
                                                                                ]);
      FLInboxChat_ctl.setSeenConversa(lstChanged[0].Id);


getFLActions()
---------------

Assinatura
    @AuraEnabled
    public static List<AcaoInbox> getFLActions(ParametroFalae__c pParametroFalae)
Ação
    Retorna uma lista com as informações de AcaoFalae__mdt do tipo Inbox
Exemplo

   .. code-block:: apex

      List<ParametroFalae__c> lstChanged = new List<ParametroFalae__c>([
                                                                        SELECT 
                                                                                Id,
                                                                                Celular__c,
                                                                                RecordTypeId,
                                                                                Operadora__c,
                                                                                SenhaSalesforce__c,
                                                                                UsuarioSalesforce__c
                                                                        FROM 
                                                                                ParametroFalae__c
                                                                        ]);
      FLInboxChat_ctl.getFLActions(lstChanged[0]);

doExecuteAction()
---------------

Assinatura
    @AuraEnabled
    public static void doExecuteAction(AcaoFalae__mdt pAcaoFalae, ParametroFalae__c pParametroFalae)
Ação
    Executa a ação determinado no pelo metadado AcaoFalae__mdt enviado por parâmetro
Exemplo

   .. code-block:: apex
   
      List<ParametroFalae__c> lstChanged = new List<ParametroFalae__c>([
                                                                        SELECT 
                                                                                Id,
                                                                                Celular__c,
                                                                                RecordTypeId,
                                                                                Operadora__c,
                                                                                SenhaSalesforce__c,
                                                                                UsuarioSalesforce__c
                                                                        FROM 
                                                                                ParametroFalae__c
                                                                        ]);
      AcaoFalae__mdt pAcaoFalae = new AcaoFalae__mdt();
      FLInboxChat_ctl.doExecuteAction(pAcaoFalae, lstChanged[0]);
