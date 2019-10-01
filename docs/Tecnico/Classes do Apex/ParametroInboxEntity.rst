##########      
ParametroInboxEntity
##########

Inner Class da classe FLInboxChat_ctl

Assinatura
    public class ParametroInboxEntity
Expecificação
    Possui as variáveis paramFl e listConversaFl e os métodos ParametroInboxEntity e add
      
paramFl
---------------

Assinatura
    @AuraEnabled
    public ParametroFalae__c paramFl;
Acao
    Cria uma variável do tipo ParametroFalae__c
      
listConversaFl
---------------

Assinatura
    @AuraEnabled
    public List<ConversaFalae__c> listConversaFl;
Acao
    Cria uma lista do tipo ConversaFalae__c
      
ParametroInboxEntity()
---------------

Assinatura
   public ParametroInboxEntity()
Acao
   Instancia a lista listConversaFl
Exemplo

   .. code-block:: apex

      ParametroInboxEntity.ParametroInboxEntity()
      
add()
---------------

Assinatura
   public void add(ConversaFalae__c pConversaFalae)
Acao
   Atribui o parâmetro paramFl e adiciona as conversas desse parâmetro a lista listConversaFl
Exemplo

   .. code-block:: apex
      
      List<ConversaFalae__c> lstChanged = new List<ConversaFalae__c>([
                                                                      SELECT
                                                                            Id,
                                                                            Name,
                                                                            Status__c
                                                                      FROM
                                                                            ConversaFalae__c
                                                                    ]);
      ParametroInboxEntity.add(lstChanged[0]);
