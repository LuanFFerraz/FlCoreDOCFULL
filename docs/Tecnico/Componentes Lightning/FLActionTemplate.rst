#################
FLActionTemplate
#################
Funcionamento:
~~~~~~~~~~~~~~~~~~~~~~~~

Template das ações do Falae

Atributos:
~~~~~~~~~~~~

+------------------------+-----------------------+-------------+
|  name                  | Tipo                  | Obrigatório |
+========================+=======================+=============+
| Footer                 | Aura.Component[]      | false       | 
+------------------------+-----------------------+-------------+
| title                  | String                | false       | 
+------------------------+-----------------------+-------------+
| conversafalae          |    conversafalae__c   | false       | 
+------------------------+-----------------------+-------------+


Exemplo:
~~~~~~~~
   .. code-block:: html

      <aura:component extends="LActionTemplate" >
         <!-- Header -->
         <aura:set attribute="title" value="Relacionar Lead/Contato " />
         <!-- Footer -->
         <aura:set attribute="footer">
             <lightning:button variant="Neutral" label="Cancelar" title="Cancelar" onclick="{! c.close }" />
         </aura:set>

         <!-- Content -->
         <lightning:layout>         
             <!-- LookupField -->
             <lightning:layoutItem flexibility="auto" size="6" >
                 <lightning:recordEditForm aura:id="recordViewForm"
                     onsubmit="{!c.close}"
                     recordId="{!v.conversafalae.whats__Contatofalae__c}"
                     objectApiName="whats__Contatofalae__c">
                     <lightning:inputField aura:id="lead"
                         fieldName="whats__Lead__c"/>
                 </lightning:recordEditForm>
             </lightning:layoutItem>
         </lightning:layout>
      </aura:component>


