#######################
FLCoreActionCaso_ctl
#######################

deleteRecord()
--------------

Assinatura
  @AuraEnabled
  public static Void deleteRecord(String recordId)
Ação
  Deleta os registros de Caso retornados através da query feita pelo recordId.
Exemplo

   .. code-block:: apex

      FLCoreActionCaso.deleteRecord('5003i000002RlBRAA0');
      
getRecords2()
--------------

Assinatura
  @AuraEnabled
  public static List<Case> getRecords2(String recordId)
Ação
  Retorna uma lista de registros de Caso através da query feita pelo recordId.
Valor retornado
  Tipo: List<Case>
Exemplo

   .. code-block:: apex

      FLCoreActionCaso.getRecords2('5003i000002RlBRAA0');
            
getObjectUrlNew()
--------------

Assinatura
  @AuraEnabled
  public static String getObjectUrlNew(String pObjectName)
Ação
  Retorna a URL para criação de um novo registro do objeto passado por parâmetro.
Valor retornado
  Tipo: String
Exemplo

   .. code-block:: apex

      FLCoreActionCaso.getObjectUrlNew('Case');
      
doGetRLID()
--------------

Assinatura
  @AuraEnabled
  public static String doGetRLID()
Ação
  Retorna o Id da relação entre o objeto pai ConversaFalae e o objeto filho Caso.
Valor retornado
  Tipo: String
Exemplo

   .. code-block:: apex

      FLCoreActionCaso.doGetRLID();
