##########################
FLCoreActionRelacionamento
##########################

Funcionamento:
~~~~~~~~~~~~~~~~
Utilizado para abrir o modal correspondente a uma das ações, a de relacionar contato ou lead.

Atributos:
~~~~~~~~~~~~

+------------------------+-----------------------+-------------+
|  name                  | Tipo                  | Obrigatório |
+========================+=======================+=============+
| conversaFalae          | String                | false       | 
+------------------------+-----------------------+-------------+
| acaoChat               | Object                | false       | 
+------------------------+-----------------------+-------------+
| tipoRelacao            | Map[]                 | false       | 
+------------------------+-----------------------+-------------+


Exemplo:
~~~~~~~~
   .. code-block:: html

      openModal : function(component, event, helper, acaoChat) {
         var componentName = "" + acaoChat.action.NamespacePrefix + ":" + acaoChat.action.flcore__ComponenteLightning__c;
        $A.createComponent( componentName, {
                'actionId' : (component.get("v.mapNavigation") ? acaoChat.action.Id : ""),
                'conversaFalae' : component.get("v.conversaFalae"),
                'isVisualforceView' : component.get("v.isVisualforceView"),
                'isClassic' : component.get("v.isClassic")
            }
         );
      }
