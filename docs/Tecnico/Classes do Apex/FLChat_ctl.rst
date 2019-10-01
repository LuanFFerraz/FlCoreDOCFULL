###############
FLChat_ctl
###############

getIsClassic()
~~~~~~~~~~~~
Assinatura
  public static Boolean getIsClassic()
Ação
  Retorna true caso o modo do SalesForce seja Classic e false caso seja Lightning.
Exemplo

   .. code-block:: apex

      FLChat.getIsClassic();
      
getConversaFl()
~~~~~~~~~~~~~~

Assinatura
  public static ConversaFalae__c getConversaFl(String pConversaFlId)
Ação
  Retorna um registro de ConversaFalae buscando pelo ID da conversa.
Exemplo

   .. code-block:: apex

      FLChat.getConversaFl('a023i000004qAnEAAU');
          
getMensagemFl()
~~~~~~~~~~~~~~

Assinatura
  global static List<MensagemFalae__c> getMensagemFl(String pConversaFlId)
Ação
  Retorna um registro de MensagemFalae buscando pelo ID da conversa.
Exemplo

   .. code-block:: apex

      FLChat.getConversaFl('a023i000004qAnEAAU');
              
getChatContent()
~~~~~~~~~~~~~~

Assinatura
  public static ChatContent getChatContent(String pConversaFlId)
Ação
  Retorna ChatContent passando como parâmetro o ID da conversa.
Exemplo

   .. code-block:: apex

      FLChat.getChatContent('a023i000004qAnEAAU');
                  
doSaveMessage()
~~~~~~~~~~~~~~

Assinatura
  public static ChatContent getChatContent(String pConversaFlId)
Ação
  Insere a mensagem de origem Empresa no objeto MensagemFalae.
Exemplo

   .. code-block:: apex

      FLChat.getChatContent('a023i000004qAnEAAU');
                      
getIconUrl()
~~~~~~~~~~~~~~

Assinatura
  public static ChatContent getChatContent(String pConversaFlId)
Ação
  Retorna o url do ícone do ContatoFalae.
Exemplo

   .. code-block:: apex

      FLChat.getIconUrl('a013i000006rKdwAAE');
                          
getHostUrl()
~~~~~~~~~~~~~~

Assinatura
  public static String getHostUrl() 
Ação
  Retorna a URL da organização.
Exemplo

   .. code-block:: apex

      FLChat.getHostUrl();
                              
getRefreshValue()
~~~~~~~~~~~~~~

Assinatura
  public static String getHostUrl() 
Ação
  Retorna a Periodicidade da Atualização.
Exemplo

   .. code-block:: apex

      FLChat.getRefreshValue();
    
    
    
