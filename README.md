# SOSL\

List<List<sObject>> x=[find 'ya' IN ALL FIELDS RETURNING book__c(Name),Yazar__c(Name)];
List<book__c> a=x.get(0);
for(book__c b:a){
     system.debug('book__c name ' +b.name);    
}

List<Yazar__c> c=x.get(1);
for(Yazar__c d:c){
    System.debug('Yazar__c name '+d.name);
}
