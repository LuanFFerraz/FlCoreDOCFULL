#################
FLModalTemplate
#################

Atributos:
~~~~~~~~~~~~

+------------------------+-----------------------+-------------+
|  Name                  | Type                  | Default     |
+========================+=======================+=============+
| recordValue            | Object                | -           | 
+------------------------+-----------------------+-------------+
| isVisualforceView      | Boolean               | false       | 
+------------------------+-----------------------+-------------+
| isClassic              | Boolean               | -           | 
+------------------------+-----------------------+-------------+
| title                  | String                | -           | 
+------------------------+-----------------------+-------------+
| footer                 | Aura.Component[]      | -           | 
+------------------------+-----------------------+-------------+

Function
~~~~~~~~~~
close()

Método utilizado para fechamento da modal.


Exemplo:
~~~~~~~~
   .. code-block:: html

      <aura:component extends="flcore:FLModalTemplate" >
         <!-- Header -->
         <aura:set attribute="title" value="Teste Modal" />
         <!-- Footer -->
         <aura:set attribute="footer">
             <lightning:button variant="Neutral" label="Cancelar" title="Cancelar" onclick="{! c.close }" />
         </aura:set>

         <!-- Content -->
         <lightning:layout>         
            <ui:outputText value="Hello World!!"/>
         </lightning:layout>
      </aura:component>


