# Jour 1 

* devops
* ansible 
    * comamndes ad hoc => 1 action / tâche spécifique 
    * fichiers nécessaires :
        * inventaire 
            * liste de hosts 
            * peuvent etre groupés 
            * peut contenir des variables 
                * sur les hotes ou les groupes 
    * actions à effectuer 
        * ciblage des machines :
            * soit avec un motif 
            * soit avec --limit (plutot dans les playbooks)
            on peut savoir les machines qui seront touchées avec `--list-hosts`
        * on appelle un module + des paramètres associés => une tache
        * on devient superadmin (escalade de priblège / privelege escalation) avec --become / --become_user
    * dossier host_vars / group_vars pour stocker les variables 
    * explication des concepts des playbooks