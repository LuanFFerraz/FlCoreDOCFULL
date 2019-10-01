###############
FLInboxConversa_ctl
###############

getIconUrl()
~~~~~~~~~~~~~~~~~~~~
  
Assinatura
    @AuraEnabled
    public static String getIconUrl(String pContatoId)
Ação
    Retorna a URL do ícone do Contato do Whatsapp caso o mesmo tenha um ícone, caso contrário retorna uma string vazia.
Valor retornado
    Retorna uma variável do tipo String
Exemplo

   .. code-block:: apex

      FLInboxConversa_ctl.getIcon('IdDoContato');

getHostUrl()
~~~~~~~~~~~~~~~~~~~~

Assinatura
    public static String getHostUrl()
Valor retornado
    Retorna uma variável do tipo String
Exemplo

   .. code-block:: apex

      String host = FLInboxConversa_ctl.getHostUrl();
