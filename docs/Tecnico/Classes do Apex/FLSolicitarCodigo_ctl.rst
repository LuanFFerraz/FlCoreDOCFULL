##########      
FLSolicitarCodigo_ctl
##########

getParametro()
---------------
Assinatura
    public static ParametroFalae__c getParametro(String pParamId)
Ação
    Retorna um **ParametroFalae__c** relacionado ao Id passado por parâmetro.
Retorno
    Retorna um objeto do tipo **ParametroFalae__c**
Exemplo
      
   .. code-block:: apex
  
      ParametroFalae__c param = new ParametroFalae__c([SELECT Id, Name FROM MensagemWhatsapp__c LIMIT 1]);
      param = FLSolicitarCodigo_ctl.getParametro(param.Id);

verificarTempoEnvio()
---------------
Assinatura
    public static ResponseEntity verificarTempoEnvio(ParametroFalae__c pParam)
Ação
    Retorna uma classe **ResponseEntity** contento o uma mensagem de resposta e um booleano contento se pode ou não enviar um novo código.
Retorno
    Retorna uma classe do tipo **ResponseEntity**
Exemplo
      
   .. code-block:: apex
      
      ParametroFalae__c param = new ParametroFalae__c([SELECT Id, Name FROM MensagemWhatsapp__c LIMIT 1]);
      param = FLSolicitarCodigo_ctl.getParametro(param.Id);
      Boolean aux = FLSolicitarCodigo_ctl.verificarTempoEnvio(param);

requestCodigo()
---------------
Assinatura
    public static void requestCodigo(ParametroFalae__c pParam)
Ação
    Faz a requicição de um novo código pa ao **Parametro Falae** do tipo **Inpulso - Mob Service**.
Exemplo
      
   .. code-block:: apex
      
      ParametroFalae__c param = new ParametroFalae__c([SELECT Id, Name FROM MensagemWhatsapp__c LIMIT 1]);
      param = FLSolicitarCodigo_ctl.getParametro(param.Id);
      FLSolicitarCodigo_ctl.requestCodigo(param);
