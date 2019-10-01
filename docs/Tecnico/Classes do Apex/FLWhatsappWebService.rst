#################
FLWhatsappWebService
#################    
      
doEnviarMensagens()
-----------------------

Assinatura
    public static void doEnviarMensagens(Set<Id> pSetMensagem)
Ação
    Responsável pelo enfileiramento das mensagem com origem Empresa > Cliente 
Exemplo
      
   .. code-block:: apex
  
      Map<Id, MensagemFalae__c> exemploresult = new Map<Id, MensagemFalae__c>([
                                                                SELECT 
                                                                        Id, 
                                                                        Name 
                                                                FROM 
                                                                        MensagemFalae__c
                                                                ]);
      FLWhatsappWebService.doEnviarMensagens(exemploresult.keySet());
       
doEnviarContentMedia()
-----------------------
**NÃO ESTÁ EM USO**

Assinatura
    public static void doEnviarContentMedia(String pOrigem, String pDestino, String pChave, String pContentMedia, String           pContentSize)
Ação
    As mensagens com imagens são montadas através deste método
Exemplo

   .. code-block:: apex

      FLWhatsappWebService.doEnviarContentMedia('551399999999', '5513997733761', '', 'teste', '60000');
       
doRegistrarNovoNumero()
-----------------------

Assinatura
    public static void doRegistrarNovoNumero(RegisterNumberEntity pRegisterNumberEntity)
Ação
    Faz a integração do novo número no servidor.
Exemplo
       
   .. code-block:: apex
   
      FLWhatsappWebService.RegisterNumberEntity registerEntity = new FLWhatsappWebService.RegisterNumberEntity();
      FLWhatsappWebService.doAutenticarNumero(registerEntity);             

doVerificaNovoNumero()
-----------------------

Assinatura
    public static void doVerificaNovoNumero()
Ação
    Faz a autenticação do código no Whatsapp.
Exemplo
       
   .. code-block:: apex
   
      FLWhatsappWebService.doVerificaNovoNumero();

doRegitrarNovoGrupo()
-----------------------
**NÃO ESTÁ EM USO**

Assinatura
   public static void doRegitrarNovoGrupo()
Ação
   Faz a integração de um novo grupo do Whatsapp no servidor.
Exemplo
       
   .. code-block:: apex
   
      FLWhatsappWebService.doRegitrarNovoGrupo();

getQr()
-----------------------

Assinatura
    public static String getQr(String pNumero)
Ação
    Pega o Qr Code do número enviado por parametro.
Retorno
    Retorna uma váriavel do tipo String.
Exemplo
       
   .. code-block:: apex
       
      FLWhatsappWebService.getQr('5513999999999');


.. _WAQrView : 
             
requestQr()
-----------------------

Assinatura
    public static String requestQr(String pNumero)
Ação
    Faz a requicição de um Qr Code para registro de um número.
Retorno
    Retorna uma váriavel do tipo String.
Exemplo

   .. code-block:: apex

      FLWhatsappWebService.requestQr('55999999999');


.. _WAQrRequest :  
             
getMensagemWaJson()
-----------------------

Assinatura
    public static String getMensagemWaJson(Set<Id> pSetId)
Ação
    Cria o Json para envio de mensagens.
Retorno
    Retorna uma váriavel do tipo String.
Exemplo

   .. code-block:: apex
   
      Map<Id, MensagemFalae__c> mapResult = new Map<Id, MensagemFalae__c>([
                                                                            SELECT 
                                                                                    Id, 
                                                                                    Name 
                                                                            FROM 
                                                                            MensagemFalae__c
                                                                         ]);
      FLWhatsappWebService.getMensagemWaJson(mapResult.keySet());
