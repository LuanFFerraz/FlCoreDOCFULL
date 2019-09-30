############
FLQrRequest_ctl
############

param
~~~~~~~~~~~~~~~~~~~~
  Get e Set da variável pública do tipo ParametroFalae__c.
Assinatura
  public ParametroFalae__c param {get;set;}
Valor retornado
  Tipo de retorno do get:		ParametroFalae__c.
  Tipo do retorno do set:		sem retorno.
  
  
response
~~~~~~~~~~~~~~~~~~~~
  Get e Set da variável pública do tipo String.
Assinatura
  public String response {get;set;}
Valor retornado
  Tipo de retorno do get:		String.
  Tipo do retorno do set:		sem retorno.
  
  
FLQrRequest_ctl()
~~~~~~~~~~~~~~~~~~~~
  Atribui um Parâmetro Falae a variável local param.
Assinatura
  public FLQrRequest_ctl(ApexPages.StandardController std)
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
      FLQrRequest_ctl ctlexemplo = new FLQrRequest_ctl(new ApexPages.StandardController(pw))
  
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
      FLQrRequest_ctl ctlexemplo = new FLQrRequest_ctl(new ApexPages.StandardController(pw));
      ctlexemplo.init();
  
getResponseMessage()
~~~~~~~~~~~~~~~~~~~~
  Retorna a mensagem do json feito com o servidor ou Erro inesperado, caso a mensagem esteja vazia.
Assinatura
  public String getResponseMessage()
Valor retornado
  Tipo:	String.
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
      FLQrRequest_ctl ctlexemplo = new FLQrRequest_ctl(new ApexPages.StandardController(pw))
      ctlexemplo.getResponseMessage();  
  
requestQr() 
~~~~~~~~~~~~~~~~~~~~
  Faz o json de requisição de um QR Code para o ParametroFalae__c da variável local param.
Assinatura
  public void requestQr()
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
      FLQrRequest_ctl ctlexemplo = new FLQrRequest_ctl(new ApexPages.StandardController(pw))
      ctlexemplo.requestQr();  
