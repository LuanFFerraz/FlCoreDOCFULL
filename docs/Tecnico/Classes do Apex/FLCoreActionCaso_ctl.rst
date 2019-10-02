#######################
FLCoreActionCaso_ctl
#######################

deleteRecord()
Assinatura
  public static Void deleteRecord(String recordId)
Ação
  Deleta os registros de Caso retornados através da query feita pelo recordId.
Exemplo

   .. code-block:: apex

      FLCoreActionCaso.deleteRecord('5003i000002RlBRAA0');
      
getRecords2()
Assinatura
  public static List<Case> getRecords2(String recordId)
Ação
  Retorna uma lista de registros de Caso através da query feita pelo recordId.
Exemplo

   .. code-block:: apex

      FLCoreActionCaso.getRecords2('5003i000002RlBRAA0');
            
getObjectUrlNew()
Assinatura
  public static String getObjectUrlNew(String pObjectName)
Ação
  Retorna a URL para criação de um novo registro do objeto passado por parâmetro.
Exemplo

   .. code-block:: apex

      FLCoreActionCaso.getObjectUrlNew('Case');
      
