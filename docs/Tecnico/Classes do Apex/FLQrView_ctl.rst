#############
FLQrView_ctl
#############

param
~~~~~~~~~~~~~~~~~~~~
  Get e Set da variável pública do tipo ParametroFalae__c.
Assinatura
  public ParametroFalae__c param {get;set;}
Valor retornado
  Tipo de retorno do get:		ParametroFalae__c.
  Tipo do retorno do set:		sem retorno.


keepPolling
~~~~~~~~~~~~~~~~~~~~
  Get e Set da variável pública do tipo Boolean.
Assinatura
  public Boolean keepPolling {get;set;}
Valor retornado
  Tipo de retorno do get:		Boolean.
  Tipo do retorno do set:		sem retorno.


FLQrView_ctl()
~~~~~~~~~~~~~~~~~~~~
  Atribui um Parâmetro Falae a variável local param.
Assinatura
  public FLQrView_ctl(ApexPages.StandardController std)
Valor retornado
  Sem retorno.
Exemplo

   .. code-block:: apex

      ParametroFalae__c pw = [
      SELECT 
            Id, 
            Celular__c 
      FROM 
            ParametroWhatsapp__c 
      Where 
            Celular__c = '13986751234' 
      LIMIT 
            1
      ];
      FLQrView_ctl ctlExemplo = new FLQrView_ctl(new ApexPages.StandardController(pw));    
      
      
init()
~~~~~~~~~~~~~~~~~~~~
  Executa outros métodos privados da classe.
Assinatura
  public void init()
Valor retornado
  Sem retorno.
Exemplo

   .. code-block:: apex

      ParametroFalae__c pw = [
      SELECT 
            Id, 
            Celular__c 
      FROM 
            ParametroFalae__c 
      Where 
            Celular__c = '13986751234' 
      LIMIT 
            1
      ];
      FLQrView_ctl ctlExemplo = new FLQrView_ctl(new ApexPages.StandardController(pw));  
      ctlExemplo.inibt();
      
loadQr() 
~~~~~~~~~~~~~~~~~~~~
  Carrega a imagem do QR Code do Parâmetro Falae da variável local param.
Assinatura
  public void loadQr()
Valor retornado
  Sem retorno.
Exemplo

   .. code-block:: apex

      FLQrView_ctl mCtl = new FLQrView_ctl();
      mCtl.loadQr();
      
getCurrentQrId()
~~~~~~~~~~~~~~~~~~~~
  Retorna o Id da imagem do QR Code do Parâmetro Falae da variável local param.
Assinatura
  public Id getCurrentQrId()
Valor retornado
  Tipo: 	Id.
Exemplo

   .. code-block:: apex

      Attachment existingAttach = new Attachment(Id = getCurrentQrId());     
      
getDisplayMessage()
~~~~~~~~~~~~~~~~~~~~
  Retorna a mensagem “Aguardando QR Code...” caso esteja aguardando o QR Code e retorna a mensagem “Nenhum código disponível” caso a organização não esteja ativada no servidor ou se o Parâmetro Falae já esteja conectado.
Assinatura
  public String getDisplayMessage()
Valor retornado
  Tipo: 	String.
Exemplo

   .. code-block:: apex

      ParametroFalae__c pw = [
      SELECT 
            Id, 
            Celular__c 
      FROM 
            ParametroFalae__c 
      Where 
            Celular__c = '13986751234' 
      LIMIT 
            1
      ];
      FLQrView_ctl ctlExemplo = new FLQrView_ctl(new ApexPages.StandardController(pw));  
      ctlExemplo.getDisplayMessage();
