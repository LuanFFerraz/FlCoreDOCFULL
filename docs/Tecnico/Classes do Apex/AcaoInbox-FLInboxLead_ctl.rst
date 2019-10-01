##########      
AcaoInbox
##########
Inner Class da classe FLInboxLead_ctl

Assinatura
    public class AcaoInbox
Expecificação
    Possui as variáveis AcaoFalae__mdt e isDisabled e o método AcaoInbox
      
AcaoFalae__mdt
---------------
Assinatura
    public AcaoFalae__mdt action;
Acao
    Cria uma variável tipo metadado AcaoFalae__mdt
      
isDisabled
---------------
Assinatura
    public Boolean isDisabled;
Acao
    Cria uma variável tipo booleano isDisabled
      
AcaoInbox()
---------------
Assinatura
    public AcaoInbox(AcaoFalae__mdt pAcaoFalae, ConversaFalae__c pConversaFalae
Acao
    Atribui valores a isDisabled e action
Exemplo

   .. code-block:: apex

      AcaoInbox.AcaoInbox(new AcaoFalae__mdt[]{new AcaoFalae__mdt(
                                                                    TipoAcao__c = 'Entrada de Mensagem', 
                                                                    ClasseApex__c = 'FLCoreExecutionAfter', 
                                                                    Assincrono__c = true
                                                                )}, 
                                                                'a021U000007pg2FQAQ'
                                                                );
