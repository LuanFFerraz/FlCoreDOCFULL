##########################
FLCoreActionCaso
##########################

Funcionamento:
~~~~~~~~~~~~~~~~
Utilizado para abrir o modal correspondente a criação de Caso na conversa.

Atributos:
~~~~~~~~~~~~

+------------------------+-----------------------+
|  name                  | Tipo                  |
+========================+=======================+
| conversaFalae          | String                | 
+------------------------+-----------------------+
| acaoChat               | Object                |
+------------------------+-----------------------+
| tipoRelacao            | Map[]                 | 
+------------------------+-----------------------+
| tipoRelacao            | Map[]                 | 
+------------------------+-----------------------+


Exemplo:
~~~~~~~~
   .. code-block:: html

      openModal : function(component, event, helper, acaoChat) {
         var componentName = "" + acaoChat.action.NamespacePrefix + ":" + acaoChat.action.flcore__ComponenteLightning__c;
        $A.createComponent( componentName, {
                'actionId' : (component.get("v.mapNavigation") ? acaoChat.action.Id : ""),
                'recordValue' : helper.getParametroSelecionado(component).paramFl,
                'isVisualforceView' : component.get("v.isVisualforceView"),
                'isClassic' : component.get("v.isClassic")
            }
         );
      }
      
