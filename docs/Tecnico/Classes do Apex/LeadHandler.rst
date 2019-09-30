#################
LeadHandler
#################


executeTrigger()
---------------

Assinatura
    **public static void executeTrigger(Map<Id, Lead> pMapOldRecord, List<Lead> pListRecord, 
                                        FLTriggerEntity pFLTriggerEntity)**
Ação
    Ao deletar uma Lead verifica se tem algum Contato Falae relacionado, caso tenha, atualiza o nome do Contato Falae
    para o nome original
Exemplo

    .. code-block:: apex

        Map<Id, Lead> mapResult = new Map<Id, Lead>([SELECT Id, LastName, Company, Status FROM Lead]);
        List<Lead> lstChanged = mapResult.values().deepClone(true, true, true);
        FLTriggerEntity entity = new FLTriggerEntity();

        entity.beforeInsert = true;
        entity.beforeUpdate = true;
        entity.beforeDelete = true;

        LeadHandler.executeTrigger(mapResult, lstChanged, entity);
