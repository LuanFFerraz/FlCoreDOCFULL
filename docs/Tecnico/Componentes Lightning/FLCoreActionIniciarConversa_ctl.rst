################################
FLCoreActionIniciarConversa_ctl
################################
Funcionalidade:
~~~~~~~~~~~~~~~~
Abre o modal para iniciar uma conversa criada através de um ContatoFalae, Lead ou Contato.

Atributos:
~~~~~~~~~~~~

+------------------------+-----------------------+-------------+
|  name                  | Tipo                  | Obrigatório |
+========================+=======================+=============+
| Footer                 | Aura.Component[]      | false       | 
+------------------------+-----------------------+-------------+
| title                  | String                | false       | 
+------------------------+-----------------------+-------------+
| conversaWhatsapp       | conversaWhatsapp__c   | false       | 
+------------------------+-----------------------+-------------+

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
