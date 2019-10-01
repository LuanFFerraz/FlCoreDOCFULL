#######################
FLActionHandler
#######################

Clásse responsável por gerenciar as ações relacionadas a Conversa Falae

doExecuteFlAction()
~~~~~~~~~~~~~~~~~~~~
Assinatura
  public static void doExecuteFlAction(AcaoFalae__mdt pAcaoFalae, Object pObjectParam) 
Ação
  Executa o método doExecuteFlAction.
Exemplo

   .. code-block:: apex

      FLActionHandler.doExecuteFlAction(AcaoFalae__mdt, lstChangedMensagem);
      
doExecuteFlAction()
~~~~~~~~~~~~~~~~~~~~
Assinatura
  public static void doExecuteFlAction(AcaoFalae__mdt pAcaoFalae, Object pObjectParam, Object pObjectParam2)
Ação
  Verifica se o registro do metadado AcaoFalae é assincrono ou não. Caso seja, executa-os, caso não, enfileira as ações e executa.
Exemplo

   .. code-block:: apex

      FLActionHandler.doExecuteFlAction(AcaoFalae__mdt, lstChanged);
          
getFlAction()
~~~~~~~~~~~~~~~~~~~~
Assinatura
  public static FLActionInterface getFlAction(AcaoFalae__mdt pAcaoFalae) 
Ação
  Retorna FLActionInterface.
Exemplo

   .. code-block:: apex

      FLActionHandler.getFlAction(AcaoFalae__mdt, lstChanged);
      
