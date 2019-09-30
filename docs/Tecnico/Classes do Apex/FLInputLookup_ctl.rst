##########      
FLInputLookup_ctl
##########

getLookUpValues()
---------------
Assinatura
    public static List<sObject> getLookUpValues(String pSearchKeyWord, String pObjectName)
Ação
    Retorna uma lista com objetos que contenha a string passada por parâmetro. 
Retorno
    Retorna um objeto do tipo **List<sObject>**
Exemplo
      
   .. code-block:: apex
  
      FLInputLookup_ctl.getLookUpValues('Elia', 'Contact');

getObjectUrlNew()
---------------
Assinatura
    public static String getObjectUrlNew(String pObjectName)
Ação
    Retorna a Url para criação de um novo objeto do tipo enviado por parâmetro.
Retorno
    Retorna um valor do tipo String
Exemplo
      
   .. code-block:: apex
   
      FLInputLookup_ctl.getObjectUrlNew('teste');
