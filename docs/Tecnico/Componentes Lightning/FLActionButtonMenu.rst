##########################
FLActionButtonMenu
##########################

Funcionamento:
~~~~~~~~~~~~~~~~
Utilizado para abrir o modal correspondente a uma das ações, a de relacionar contato ou lead.

Atributos:
~~~~~~~~~~~~

+----------------------------+-----------------------+
|  name                      | Tipo                  |
+============================+=======================+
| recordValue                | Object                |
+----------------------------+-----------------------+
| acoes                      | Object[]              |
+----------------------------+-----------------------+
| isClassic                  | Boolean               |
+----------------------------+-----------------------+
| isClasisVisualforceViewsic | Boolean               |
+----------------------------+-----------------------+

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
