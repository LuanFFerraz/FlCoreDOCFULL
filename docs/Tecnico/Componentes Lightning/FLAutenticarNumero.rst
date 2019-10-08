##########################
FLAutenticarNumero
##########################

Funcionamento:
~~~~~~~~~~~~~~~~
Utilizado para abrir o modal de autentificar o número.

Atributos:
~~~~~~~~~~~~

+------------------------+-----------------------+
|  name                  | Tipo                  |
+========================+=======================+
| parametroFalae         | String                |
+------------------------+-----------------------+
| isVisualforceViewsic   | Boolean               |
+------------------------+-----------------------+


Exemplo:
~~~~~~~~
   .. code-block:: html
      <script>
        $Lightning.use("flcore:Falae", function() {
            $Lightning.createComponent(
                "flcore:FLAutenticarNumero", 
                { 
                    parametroFalae : "{!ParametroFalae__c.Id}",
                    isVisualforceView : true
                },
                "FLAutenticarNumero",
                function(cmp) {
                    
                }
            );
        });
      </script>
      
