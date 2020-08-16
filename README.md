# kabug-rb
Repositório do projeto Kabug com Cucumber, Capybara e Ruby

## Como executar o projeto

 * Importante ter o ruby instalado (versão 2,5 ou superior)
 
###Instalar o Bundler
'

gem install bundler
'

### Instalar as depencencias do ruby (projeto)
'

bundle install
'

### Executar localmente
'
bundle exec cucumber
'
### Executar no servidor de CI (gerando reports JSON)
'
bundle exec cucumper -p ci

