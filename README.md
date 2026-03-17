Detta projekt skapar och konfigurerar infrastruktur i google cloud automatiskt med terraform. 
Det startar en VM och har ett hardeningscript som ser till att installera säkerhetspaket och fail2ban men också aktiverar branvägg och aktiverar automatiska säkerhetsuppdateringar. 
Terraform init förbereder projektet, Terraform plan visar ändringar och Terraform apply deployar.
Varför vi har brandvägg är för att begränsa anslutningarna och varför vi har fail2ban är för att minimera tex bottar som försöker gissa lösenord. 
Automatiska säkerhetsuppdateringar kan ha fördel att patcha sårbarheter och det minskar också behovet av manuella uppdateringar. 
Att ha snapshot policy kan ge snabb åsterställning vid olika incidenter. 
