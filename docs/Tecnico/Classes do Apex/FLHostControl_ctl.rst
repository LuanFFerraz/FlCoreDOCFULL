#################
FLHostControl_ctl
#################

getHost()
------------

Assinatura
    public String getHost()
Ação
    Retorna a URL da organização.
Valor retornado
    Tipo:	String
Exemplo

    .. code-block:: apex

      FLHostControl_ctl wahost = new FLHostControl_ctl();
      String s = wahost.getHost();
      system.assertEquals(s, 'exemplo-dev-ed.my.salesforce.com');
