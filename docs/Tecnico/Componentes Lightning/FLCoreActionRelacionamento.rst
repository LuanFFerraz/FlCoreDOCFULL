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

Function
~~~~~~~~~~
close()

Método utilizado para fechamento da modal.


Exemplo:
~~~~~~~~
   .. code-block:: html

      <aura:component extends="FLActionTemplate" >
      <!-- Header -->
      <aura:set attribute="title" value="Relacionar Lead/Contato " />
      <!-- Footer -->
      <aura:set attribute="footer">
       <lightning:button variant="Neutral" label="Cancel" title="Cancel" onclick="{! c.close }" disabled="{!v.blockButtons}"/> 
       <lightning:button variant="brand" label="Salvar" title="Save" onclick="{! c.handleSave }" disabled="{!v.blockButtons}"/>
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
