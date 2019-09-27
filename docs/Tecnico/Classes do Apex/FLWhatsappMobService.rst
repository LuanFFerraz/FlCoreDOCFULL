#################
FLWhatsappMobService
#################
Classe responsável por gerenciar e enviar mensagens pela API Whatsapp Mobile

doEnviarMensagem()
---------------

Assinatura
    public static void doEnviarMensagem(String pOrigem, String pDestino, String pChave, String pMensagem, String pIdChat)
Retorno
    Método responsável pelo envio de mensagem na API Mob
Exemplo

   .. code-block:: apex

      SendWhatsappMessage.doEnviarMensagem('551399999999', '5513997733761', '', 'teste', 'a011U00000Occ0WQAR');    
 

doEnviarMensagens()
---------------

Assinatura
    public static void doEnviarMensagens(String pOrigem, String pDestino, String pChave, String pMensagem, String pIdChat)
Retorno
    Método responsável pelo envio de múltiplas mensagens, enfileirando-as. 
Exemplo

   .. code-block:: apex

      Map<Id, MensagemWhatsapp__c> exemploresult = new Map<Id, MensagemWhatsapp__c>([SELECT Id, Name FROM MensagemWhatsapp__c]);
      doEnviarMensagens.doEnviarMensagens(exemploresult.keySet());    
 
doEnviarContentMedia()
-----------------------

Retorno
    Envia mensagens com conteúdo de mídia, vide imagens.
Assinatura
    public static void doEnviarContentMedia(String pOrigem, String pDestino, String pChave, String pContentMedia, String pContentSize)
Exemplo

   .. code-block:: apex

      
       
doRegistrarNovoNumero()
-----------------------

Retorno
    Registra o número que envia mensagens
Assinatura
    public static void doRegistrarNovoNumero(RegisterNumberEntity pRegisterNumberEntity) 
Exemplo
       
   .. code-block:: apex

      

doAtualizarNovoNumero()
-----------------------
    
Retorno   
    Atualiza o número que envia mensagens.
Assinatura
    doAtualizarNovoNumero(RegisterNumberEntity pRegisterNumberEntity) 
Exemplo
       
   .. code-block:: apex
      
      SendWhatsappMessage.doAutenticarNumero('13', '55999999999', '');
             
registerNewNumber()
-----------------------

Retorno
    
Assinatura
    private static void registerNewNumber(String pJsonRegisterNumber) {
Exemplo
 

   .. code-block:: apex

      SendWhatsappMessage.doRegistrarNovoNumero('55999999999', '55988888888', 'operadora', 'xxxx_xx@xxxx.com', 'xxx51465xx', '', '1');
           
