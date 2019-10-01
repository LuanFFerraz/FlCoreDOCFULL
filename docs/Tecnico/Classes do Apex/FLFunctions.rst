############
FLFunctions
############

emptyIfNull()
------------
  
Assinatura
    public static String emptyIfNull(String pValue)
Ação
    Retorna a String em branco caso seja nula, caso contrário retorna a própria string passado por parâmetro
Valor retornado
    Tipo:	String
Exemplo

    .. code-block:: apex

      FLFunctions.getVfHost();

getVfHost()
------------
  
Assinatura
    public static String getVfHost()
Ação
    Retorna a URL da organização.
Valor retornado
    Tipo:	String
Exemplo

    .. code-block:: apex

      FLFunctions.getVfHost();

getSfdcActionUrlNew()
------------
  
Assinatura
    public static String getSfdcActionUrlNew(String pObjectApi)
Ação
    Retorna a URL para criação de um novo registro do objeto passado por parâmetro.
Valor retornado
    Tipo:	String
Exemplo

    .. code-block:: apex

      FLFunctions.getSfdcActionUrlNew('Case');

runningInASandbox()
------------
  
Assinatura
    public static Boolean runningInASandbox()
Ação
    Retorna se está rodando em sandbox
Valor retornado
    Tipo:	Boolean
Exemplo

    .. code-block:: apex

      FLFunctions.runningInASandbox();
      
getHostName()
------------
  
Assinatura
    public static String getHostName()
Ação
    Retorna o host da organização.
Valor retornado
    Tipo:	String
Exemplo

    .. code-block:: apex

      FLFunctions.getHostName();

isClassic()
------------
  
Assinatura
    public static Boolean isClassic() 
Ação
    Retorna se o tema da organização é classic.
Valor retornado
    Tipo:	String
Exemplo

    .. code-block:: apex

      FLFunctions.isClassic();
